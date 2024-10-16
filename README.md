# CALANGO-SCRIPT
Script do calanguinho

--local function changeInfectedColor()
    for _, player in pairs(game.Players:GetPlayers()) do
        if player.Team == game.Teams.Infected then
            player.Character.Head.BrickColor = BrickColor.new("Bright red")
        end
    end
end

-- Função para mudar a cor dos jogadores
local function changePlayerColor()
    for _, player in pairs(game.Players:GetPlayers()) do
        if player.Team == game.Teams.Players then
            player.Character.Head.BrickColor = BrickColor.new("Bright blue")
        end
    end
end

-- Loop para verificar e aplicar as cores continuamente
while true do
    changeInfectedColor()
    changePlayerColor()
    wait(1) -- Espera 1 segundo antes de verificar novamente
end

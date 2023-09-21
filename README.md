# JitterAim
Jitter aim para cuando me de paja 

function OnEvent(event, arg)
    if (event == "PROFILE_ACTIVATED") then
        EnablePrimaryMouseButtonEvents(true)
    end
 if IsKeyLockOn("scrolllock")then
    if (event == "MOUSE_BUTTON_PRESSED" and arg == 1)then
        if IsMouseButtonPressed(3)then
        repeat
        MoveMouseRelative(-8, 10)
        Sleep(8)
        MoveMouseRelative(8, -8)
        Sleep(8)
        until not IsMouseButtonPressed(1)
        end
      end
    end
  end

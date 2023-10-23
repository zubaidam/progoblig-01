# progoblig-01

#definerer hver part av flagget
bg = rectangle(220, 160, "solid", "dark-blue")
red-l = square(60, "solid", "red")
white-l = square(70, "solid", "white")
red-r = rectangle(120, 60, "solid", "red")
white-r = rectangle(130, 70, "solid", "white")

#definerer hele koden/flagget som et enkelt navn
norges-flagg = 
  overlay-align("left", "top", red-l,
    overlay-align("left", "top", white-l,
      overlay-align("left", "bottom", red-l,
        overlay-align("left", "bottom", white-l,
          overlay-align("right", "top", red-r,
            overlay-align("right", "top", white-r,
              overlay-align("right", "bottom", red-r, 
                overlay-align("right", "bottom", white-r,
                  bg))))))))

#printer ut norges flagg
norges-flagg

*****************HW 1: ****************  

one file is used for test, one file is used for autograder. as prof said  

"following up on this, the autograder doesn’t run each line in your notebook but rather looks for all the function definitions and import statements. so when it tried to import your function def evaluate_attacked_accuracy(attack_magnitude, attack_fn=white_box_attack, device=device), it finds white_box_attack exists but it doesn’t know what device is.   

i just set device="cpu" back in the function signature as it originally was (and that’s how it is inside the autograder’s copy of this function), and then copied your device = ... line inside the function (just as chenghao suggested). this is definitely a hack since we’re ignoring/overriding the function argument… but i uploaded the modified notebook back onto gradescope for you and that error didn’t appear (it’s still running after a few minutes, but it crashed right away before)."

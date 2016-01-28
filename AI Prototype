import sys,time,random, os.path

typing_speed = 150 #wpm
def slow_type(t):
    for l in t:
        sys.stdout.write(l)
        sys.stdout.flush()
        time.sleep(random.random()*10.0/typing_speed)
    print ''

slow_type("Hello! My name is TUTAI, or Turing Test Artificial Intelligance")

slow_type("Currently I am in training, so my features aren't fully complete.")

slow_type("If you say something I don't understand yet, I will repeat it back to you in order for me to learn")

slow_type("and build a database of responces!")

loopDeLoop = True

inputOne = 1

justAsked = False


while loopDeLoop == True:

    if justAsked == True:
        nothing = 0
    elif justAsked == False:
        inputOne = raw_input()

    fileName = inputOne + ".txt"   

    existance = True

    try:
        test = open(fileName, "r")

    except:
        existance = False


    if existance == True:
        talkBack = open(fileName, "r+")
        slow_type(talkBack.read())

    else:
        slow_type("I'm sorry, I don't have a responce for that yet")
        slow_type(inputOne)
        talk = raw_input()
        learningName = inputOne + ".txt"
        learning = open(learningName, "w")
        learning.write(talk)
        learning.close()
        
    loopDeLoop = True

    



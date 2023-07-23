#!/usr/bin/env python
# -*- coding: utf-8 -*-
"""
This experiment was created using PsychoPy3 Experiment Builder (v2021.2.3),
    on Mon Sep 19 11:43:22 2022
If you publish work using this script the most relevant publication is:

    Peirce J, Gray JR, Simpson S, MacAskill M, Höchenberger R, Sogo H, Kastman E, Lindeløv JK. (2019) 
        PsychoPy2: Experiments in behavior made easy Behav Res 51: 195. 
        https://doi.org/10.3758/s13428-018-01193-y

"""

from __future__ import absolute_import, division

from psychopy import locale_setup
from psychopy import prefs
from psychopy import sound, gui, visual, core, data, event, logging, clock, colors
from psychopy.constants import (NOT_STARTED, STARTED, PLAYING, PAUSED,
                                STOPPED, FINISHED, PRESSED, RELEASED, FOREVER)

import numpy as np  # whole numpy lib is available, prepend 'np.'
from numpy import (sin, cos, tan, log, log10, pi, average,
                   sqrt, std, deg2rad, rad2deg, linspace, asarray)
from numpy.random import random, randint, normal, shuffle, choice as randchoice
import os  # handy system and path functions
import sys  # to get file system encoding

from psychopy.hardware import keyboard



# Ensure that relative paths start from the same directory as this script
_thisDir = os.path.dirname(os.path.abspath(__file__))
os.chdir(_thisDir)

# Store info about the experiment session
psychopyVersion = '2021.2.3'
expName = '20_ChessYesNo'  # from the Builder filename that created this script
expInfo = {'participant': '', 'session': '001'}
dlg = gui.DlgFromDict(dictionary=expInfo, sortKeys=False, title=expName)
if dlg.OK == False:
    core.quit()  # user pressed cancel
expInfo['date'] = data.getDateStr()  # add a simple timestamp
expInfo['expName'] = expName
expInfo['psychopyVersion'] = psychopyVersion

# Data file name stem = absolute path + name; later add .psyexp, .csv, .log, etc
filename = _thisDir + os.sep + u'data/%s_%s_%s' % (expInfo['participant'], expName, expInfo['date'])

# An ExperimentHandler isn't essential but helps with data saving
thisExp = data.ExperimentHandler(name=expName, version='',
    extraInfo=expInfo, runtimeInfo=None,
    originPath='/Users/felipevieira/Desktop/Experiment_try/20_ChessYesNo.py',
    savePickle=True, saveWideText=True,
    dataFileName=filename)
# save a log file for detail verbose info
logFile = logging.LogFile(filename+'.log', level=logging.EXP)
logging.console.setLevel(logging.WARNING)  # this outputs to the screen, not a file

endExpNow = False  # flag for 'escape' or other condition => quit the exp
frameTolerance = 0.001  # how close to onset before 'same' frame

# Start Code - component code to be run after the window creation

# Setup the Window
win = visual.Window(
    size=(1024, 768), fullscr=True, screen=0, 
    winType='pyglet', allowGUI=False, allowStencil=False,
    monitor='testMonitor', color=[0,0,0], colorSpace='rgb',
    blendMode='avg', useFBO=True, 
    units='height')
# store frame rate of monitor if we can measure it
expInfo['frameRate'] = win.getActualFrameRate()
if expInfo['frameRate'] != None:
    frameDur = 1.0 / round(expInfo['frameRate'])
else:
    frameDur = 1.0 / 60.0  # could not measure, so guess

# Setup eyetracking
ioDevice = ioConfig = ioSession = ioServer = eyetracker = None

# create a default keyboard (e.g. to check for escape)
defaultKeyboard = keyboard.Keyboard()

# Initialize components for Routine "Welcome"
WelcomeClock = core.Clock()
text_Instrc = visual.TextStim(win=win, name='text_Instrc',
    text='Welcome to this experiment! In the next minutes, you will be presented with different chessboard positions. \n\nIn the next window, specific instructions for this experiment will be given. \n\nBefore starting the experiment an information letter will appear where you can find a general information about the overarching project. Note that the information letter is describing a more demanding task than that of this experiment. \n\nAfter the information letter, an informed consent will also appear. Please, make sure you agree with it before continuing with the experiment.\n\nPress “spacebar” if you are ready to proceed. ',
    font='Open Sans',
    pos=(0, 0), height=0.04, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);
key_Instrc = keyboard.Keyboard()

# Initialize components for Routine "Instructions"
InstructionsClock = core.Clock()
text_Instrc2 = visual.TextStim(win=win, name='text_Instrc2',
    text='In all of the upcoming 20 positions white is always to move. For each image you have to ask yourself if there is a forced checkmate. \n\nIf there is a checkmate, press your left arrow key. After that, a new screen will appear. Please, type the first move for white that leads to checkmate in the grey box located in the middle of the screen. Then click where it says “click here to continue”.\n\nIf there is no checkmate, just press your right arrow key. Next, a screen will appear where you can type the first move for white. In this case, just click where it says “click here to continue”.\n\nPress “spacebar” to continue.',
    font='Open Sans',
    pos=(0, 0), height=0.04, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);
key_Instrc2 = keyboard.Keyboard()

# Initialize components for Routine "InformationL"
InformationLClock = core.Clock()
text_L1 = visual.TextStim(win=win, name='text_L1',
    text='INFORMATION LETTER:\nFundamental Mechanisms of Human Visual Categorization: Neural Basis, Development, and Plasticity\n\nYou volunteered for our study. This text has been written to familiarize you with the purpose and course of the investigation.\n\n(1) Purpose of the study: You have been recruited as a participant for a behavioral experiment that is part of a project on visual categorization and how the brain processes it. In all experiments, participants will be asked to assess the relationship between a set of visual stimuli and to identify or discriminate stimuli. In this way we can investigate how these stimuli are processed and represented, such as which stimuli dimensions the participants pay attention to. \n(2) Description of the study method: The experiment includes a session of up to 2 hours during which you will perform tasks on the computer. The duties consist of discrimination or rating duties as explained below. There are two types of rating tasks. In the first type of rating task, participants will be asked to rate the similarity of a pair of stimuli that appear simultaneously on the screen. Participants are asked to organize multiple stimuli that appear simultaneously on the screen in such a way that similar stimuli are placed closer together. There are also two types of discrimination tasks. The first task is similar to the pairwise rating task, but now you will be asked to organize the stimuli along an axis showing a certain property (eg "how small or big stimulus A is?"). The second kind of discrimination task involves estimating the number of cells in an embryo. If we want to investigate the effect of training, the discrimination tasks will be performed in different sessions. (3) Safety precautions: There are no risks or inconveniences associated with this study, other than the discomfort of sitting in front of a computer screen for extended periods (1-2 hours).\n',
    font='Open Sans',
    pos=(0, 0.30), height=0.015, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);
text_L2 = visual.TextStim(win=win, name='text_L2',
    text='(4) Confidentiality Guarantee: The collected data is processed in accordance with the European General Data Protection Regulation (GDPR) and the Belgian Legislation on the protection of natural persons with regard to the processing of personal data. The results of this research will be used for scientific purposes and in scientific publications. Your name will not be published and the confidentiality of the data is guaranteed at every stage of the investigation by means of coding (no mention of name or other identifying elements). If the publication process requires that the research data be co-published, it will always be published in encrypted form, without personal information. After participating in the study, the Informed Consent document is kept together with the protocol paper containing the name of the participant. The link between these two documents can only be found with the help of the encryption key. The encryption key is kept by the researcher and he / she is the only person who can make the link between the participant and his / her data. By participating in this study you therefore agree that your data will be used for purposes as described in this document. You always have the right to stop your participation, the data already collected will be stored in accordance with the above guidelines and no further data will be collected. KUL is the controller for your data. If you have any questions about how we use your data or if you want to exercise your right to access, correct, or possibly stop further processing, you can always contact the principal investigator at the following contact address: hans.opdebeeck@kuleuven.be. If you have any special points for attention afterwards or if you wish to file a complaint, you can contact the KU Leuven privacy team at privacy@kuleuven.be. Finally, if you have a complaint about the processing of your data, you can contact the Belgian supervisory authority that supervises compliance with the basic principles of the protection of personal data:\n\nThe Belgian supervisory authority is called:\nData protection authority (GBA)\nDrukpersstraat 35,\n1000 Brussels\nTel. +32 2 274 48 00\ne-mail: contact@apd-gba.be\nWebsite: www.dataprotectionauthority.be',
    font='Open Sans',
    pos=(0, - 0.06), height=0.015, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=-1.0);
text_L3 = visual.TextStim(win=win, name='text_L3',
    text='(5) Insurance: In accordance with the Belgian law of 7 May 2004 on experiments on the human person, the sponsor is liable, even without errors, for all damage incurred by the participant and / or his rightful claimants that is directly or indirectly related to the research. Although the risk of participating in this study is very small, the sponsor of this study, KU Leuven, has taken out insurance in accordance with Article 29 of the Belgian law of 7 May 2004. \n(6) Contact: If you would like additional information, you can always contact Prof. dr. Dr. H. Op de Beeck (Hans.OpdeBeeck @ kuleuven.be; tel .: 016 / 32.60.39).\n\nPress “spacebar” to continue. ',
    font='Open Sans',
    pos=(0, - 0.35), height=0.015, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=-2.0);
key_resp_L = keyboard.Keyboard()

# Initialize components for Routine "Consent"
ConsentClock = core.Clock()
consentTxt = visual.TextStim(win=win, name='consentTxt',
    text='INFORMED CONSENT\n\nTitle of the study:\nFundamental mechanisms of human visual categorization: Neural basis, development and plasticity\n\nName + contact details researcher:\nArtem Platonov, artem.platonov@kuleuven.be\n\nPurpose and methodology of the research:\nStudy on visual categorization through discrimination / rating tasks.\n\nDuration of the experiment:\nUp to 2 hours\n\n- I understand what is expected of me during this investigation.\n\n- I know I will participate in the following trials or tests: Discrimination or rating task on the computer\n\n- I know that there may be risks or inconveniences associated with my participation: There are no specific risks to performing the computer tasks.\n\n- I know that I will be compensated for my participation in one of the following ways: € 10 per hour\n\n- I understand that my participation in this study is voluntary. I have the right to cancel my participation at any time. I do not have to give a reason for this and I know that this cannot cause any harm to me.\n\n- The results of this research can be used for scientific purposes and may be published. In addition, the research data may be made freely available on open platforms. My name will not be published, anonymity and the confidentiality of the data is guaranteed at every stage of the investigation.\n\n- I would like to be kept informed of the results of this research. The researcher may contact me for this at the following e-mail address:\n\n- If I have any questions, I know that after my participation I can contact: Professor Hans Op de Beeck, hans.opdebeeck@kuleuven.be\n\n- For any complaints or other concerns regarding ethical aspects of this study, I can contact the Social and Societal Ethics Committee of KU Leuven: smec@kuleuven.be\n\nI have read and understood the above information and have received answers to all my questions regarding this study. \n\nIf you agree with the terms, press “spacebar”. If do not agree, press “n”.\n',
    font='Open Sans',
    pos=(0, 0), height=0.015, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);
consent_resp = keyboard.Keyboard()

# Initialize components for Routine "Blank"
BlankClock = core.Clock()
text_6 = visual.TextStim(win=win, name='text_6',
    text=None,
    font='Open Sans',
    pos=(0, 0), height=0.1, wrapWidth=None, ori=0.0, 
    color='white', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);

# Initialize components for Routine "trial"
trialClock = core.Clock()
image = visual.ImageStim(
    win=win,
    name='image', 
    image='sin', mask=None,
    ori=0.0, pos=(0, 0), size=(0.5, 0.5),
    color=[1,1,1], colorSpace='rgb', opacity=None,
    flipHoriz=False, flipVert=False,
    texRes=128.0, interpolate=True, depth=0.0)
endButtonNo = visual.TextStim(win=win, name='endButtonNo',
    text='No',
    font='Open Sans',
    pos=(0.20, - 0.30), height=0.04, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=-1.0);
endButtonYes = visual.TextStim(win=win, name='endButtonYes',
    text='Yes',
    font='Open Sans',
    pos=(- 0.20, - 0.30), height=0.04, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=-2.0);
key_resp = keyboard.Keyboard()

# Initialize components for Routine "AnswerTrial"
AnswerTrialClock = core.Clock()
image_2 = visual.ImageStim(
    win=win,
    name='image_2', 
    image='sin', mask=None,
    ori=0.0, pos=(0, 0.3), size=(0.2, 0.2),
    color=[1,1,1], colorSpace='rgb', opacity=None,
    flipHoriz=False, flipVert=False,
    texRes=128.0, interpolate=True, depth=0.0)
checksequence = visual.TextBox2(
     win, text=None, font='Open Sans',
     pos=(0, - 0.15),     letterHeight=0.04,
     size=(None, None), borderWidth=2.0,
     color='black', colorSpace='rgb',
     opacity=None,
     bold=False, italic=False,
     lineSpacing=1.0,
     padding=0.0,
     anchor='center',
     fillColor=None, borderColor=None,
     flipHoriz=False, flipVert=False,
     editable=True,
     name='checksequence',
     autoLog=True,
)
Mousetocontinue = event.Mouse(win=win)
x, y = [None, None]
Mousetocontinue.mouseClock = core.Clock()
endtext = visual.TextStim(win=win, name='endtext',
    text='Click here to continue',
    font='Open Sans',
    pos=(0, - 0.30), height=0.04, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=-3.0);

# Initialize components for Routine "End"
EndClock = core.Clock()
text_7 = visual.TextStim(win=win, name='text_7',
    text='Thank you for participating!',
    font='Open Sans',
    pos=(0, 0), height=0.05, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);

# Initialize components for Routine "No_consent"
No_consentClock = core.Clock()
byetext = visual.TextStim(win=win, name='byetext',
    text='Thank you for participating!',
    font='Open Sans',
    pos=(0, 0), height=0.05, wrapWidth=None, ori=0.0, 
    color='black', colorSpace='rgb', opacity=None, 
    languageStyle='LTR',
    depth=0.0);

# Create some handy timers
globalClock = core.Clock()  # to track the time since experiment started
routineTimer = core.CountdownTimer()  # to track time remaining of each (non-slip) routine 

# ------Prepare to start Routine "Welcome"-------
continueRoutine = True
# update component parameters for each repeat
key_Instrc.keys = []
key_Instrc.rt = []
_key_Instrc_allKeys = []
# keep track of which components have finished
WelcomeComponents = [text_Instrc, key_Instrc]
for thisComponent in WelcomeComponents:
    thisComponent.tStart = None
    thisComponent.tStop = None
    thisComponent.tStartRefresh = None
    thisComponent.tStopRefresh = None
    if hasattr(thisComponent, 'status'):
        thisComponent.status = NOT_STARTED
# reset timers
t = 0
_timeToFirstFrame = win.getFutureFlipTime(clock="now")
WelcomeClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
frameN = -1

# -------Run Routine "Welcome"-------
while continueRoutine:
    # get current time
    t = WelcomeClock.getTime()
    tThisFlip = win.getFutureFlipTime(clock=WelcomeClock)
    tThisFlipGlobal = win.getFutureFlipTime(clock=None)
    frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
    # update/draw components on each frame
    
    # *text_Instrc* updates
    if text_Instrc.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_Instrc.frameNStart = frameN  # exact frame index
        text_Instrc.tStart = t  # local t and not account for scr refresh
        text_Instrc.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_Instrc, 'tStartRefresh')  # time at next scr refresh
        text_Instrc.setAutoDraw(True)
    
    # *key_Instrc* updates
    waitOnFlip = False
    if key_Instrc.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        key_Instrc.frameNStart = frameN  # exact frame index
        key_Instrc.tStart = t  # local t and not account for scr refresh
        key_Instrc.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(key_Instrc, 'tStartRefresh')  # time at next scr refresh
        key_Instrc.status = STARTED
        # keyboard checking is just starting
        waitOnFlip = True
        win.callOnFlip(key_Instrc.clock.reset)  # t=0 on next screen flip
        win.callOnFlip(key_Instrc.clearEvents, eventType='keyboard')  # clear events on next screen flip
    if key_Instrc.status == STARTED and not waitOnFlip:
        theseKeys = key_Instrc.getKeys(keyList=['space'], waitRelease=False)
        _key_Instrc_allKeys.extend(theseKeys)
        if len(_key_Instrc_allKeys):
            key_Instrc.keys = _key_Instrc_allKeys[-1].name  # just the last key pressed
            key_Instrc.rt = _key_Instrc_allKeys[-1].rt
            # a response ends the routine
            continueRoutine = False
    
    # check for quit (typically the Esc key)
    if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
        core.quit()
    
    # check if all components have finished
    if not continueRoutine:  # a component has requested a forced-end of Routine
        break
    continueRoutine = False  # will revert to True if at least one component still running
    for thisComponent in WelcomeComponents:
        if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
            continueRoutine = True
            break  # at least one component has not yet finished
    
    # refresh the screen
    if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
        win.flip()

# -------Ending Routine "Welcome"-------
for thisComponent in WelcomeComponents:
    if hasattr(thisComponent, "setAutoDraw"):
        thisComponent.setAutoDraw(False)
thisExp.addData('text_Instrc.started', text_Instrc.tStartRefresh)
thisExp.addData('text_Instrc.stopped', text_Instrc.tStopRefresh)
# check responses
if key_Instrc.keys in ['', [], None]:  # No response was made
    key_Instrc.keys = None
thisExp.addData('key_Instrc.keys',key_Instrc.keys)
if key_Instrc.keys != None:  # we had a response
    thisExp.addData('key_Instrc.rt', key_Instrc.rt)
thisExp.addData('key_Instrc.started', key_Instrc.tStartRefresh)
thisExp.addData('key_Instrc.stopped', key_Instrc.tStopRefresh)
thisExp.nextEntry()
# the Routine "Welcome" was not non-slip safe, so reset the non-slip timer
routineTimer.reset()

# ------Prepare to start Routine "Instructions"-------
continueRoutine = True
# update component parameters for each repeat
key_Instrc2.keys = []
key_Instrc2.rt = []
_key_Instrc2_allKeys = []
# keep track of which components have finished
InstructionsComponents = [text_Instrc2, key_Instrc2]
for thisComponent in InstructionsComponents:
    thisComponent.tStart = None
    thisComponent.tStop = None
    thisComponent.tStartRefresh = None
    thisComponent.tStopRefresh = None
    if hasattr(thisComponent, 'status'):
        thisComponent.status = NOT_STARTED
# reset timers
t = 0
_timeToFirstFrame = win.getFutureFlipTime(clock="now")
InstructionsClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
frameN = -1

# -------Run Routine "Instructions"-------
while continueRoutine:
    # get current time
    t = InstructionsClock.getTime()
    tThisFlip = win.getFutureFlipTime(clock=InstructionsClock)
    tThisFlipGlobal = win.getFutureFlipTime(clock=None)
    frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
    # update/draw components on each frame
    
    # *text_Instrc2* updates
    if text_Instrc2.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_Instrc2.frameNStart = frameN  # exact frame index
        text_Instrc2.tStart = t  # local t and not account for scr refresh
        text_Instrc2.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_Instrc2, 'tStartRefresh')  # time at next scr refresh
        text_Instrc2.setAutoDraw(True)
    
    # *key_Instrc2* updates
    waitOnFlip = False
    if key_Instrc2.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        key_Instrc2.frameNStart = frameN  # exact frame index
        key_Instrc2.tStart = t  # local t and not account for scr refresh
        key_Instrc2.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(key_Instrc2, 'tStartRefresh')  # time at next scr refresh
        key_Instrc2.status = STARTED
        # keyboard checking is just starting
        waitOnFlip = True
        win.callOnFlip(key_Instrc2.clock.reset)  # t=0 on next screen flip
        win.callOnFlip(key_Instrc2.clearEvents, eventType='keyboard')  # clear events on next screen flip
    if key_Instrc2.status == STARTED and not waitOnFlip:
        theseKeys = key_Instrc2.getKeys(keyList=['space'], waitRelease=False)
        _key_Instrc2_allKeys.extend(theseKeys)
        if len(_key_Instrc2_allKeys):
            key_Instrc2.keys = _key_Instrc2_allKeys[-1].name  # just the last key pressed
            key_Instrc2.rt = _key_Instrc2_allKeys[-1].rt
            # a response ends the routine
            continueRoutine = False
    
    # check for quit (typically the Esc key)
    if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
        core.quit()
    
    # check if all components have finished
    if not continueRoutine:  # a component has requested a forced-end of Routine
        break
    continueRoutine = False  # will revert to True if at least one component still running
    for thisComponent in InstructionsComponents:
        if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
            continueRoutine = True
            break  # at least one component has not yet finished
    
    # refresh the screen
    if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
        win.flip()

# -------Ending Routine "Instructions"-------
for thisComponent in InstructionsComponents:
    if hasattr(thisComponent, "setAutoDraw"):
        thisComponent.setAutoDraw(False)
thisExp.addData('text_Instrc2.started', text_Instrc2.tStartRefresh)
thisExp.addData('text_Instrc2.stopped', text_Instrc2.tStopRefresh)
# check responses
if key_Instrc2.keys in ['', [], None]:  # No response was made
    key_Instrc2.keys = None
thisExp.addData('key_Instrc2.keys',key_Instrc2.keys)
if key_Instrc2.keys != None:  # we had a response
    thisExp.addData('key_Instrc2.rt', key_Instrc2.rt)
thisExp.addData('key_Instrc2.started', key_Instrc2.tStartRefresh)
thisExp.addData('key_Instrc2.stopped', key_Instrc2.tStopRefresh)
thisExp.nextEntry()
# the Routine "Instructions" was not non-slip safe, so reset the non-slip timer
routineTimer.reset()

# ------Prepare to start Routine "InformationL"-------
continueRoutine = True
# update component parameters for each repeat
key_resp_L.keys = []
key_resp_L.rt = []
_key_resp_L_allKeys = []
# keep track of which components have finished
InformationLComponents = [text_L1, text_L2, text_L3, key_resp_L]
for thisComponent in InformationLComponents:
    thisComponent.tStart = None
    thisComponent.tStop = None
    thisComponent.tStartRefresh = None
    thisComponent.tStopRefresh = None
    if hasattr(thisComponent, 'status'):
        thisComponent.status = NOT_STARTED
# reset timers
t = 0
_timeToFirstFrame = win.getFutureFlipTime(clock="now")
InformationLClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
frameN = -1

# -------Run Routine "InformationL"-------
while continueRoutine:
    # get current time
    t = InformationLClock.getTime()
    tThisFlip = win.getFutureFlipTime(clock=InformationLClock)
    tThisFlipGlobal = win.getFutureFlipTime(clock=None)
    frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
    # update/draw components on each frame
    
    # *text_L1* updates
    if text_L1.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_L1.frameNStart = frameN  # exact frame index
        text_L1.tStart = t  # local t and not account for scr refresh
        text_L1.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_L1, 'tStartRefresh')  # time at next scr refresh
        text_L1.setAutoDraw(True)
    
    # *text_L2* updates
    if text_L2.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_L2.frameNStart = frameN  # exact frame index
        text_L2.tStart = t  # local t and not account for scr refresh
        text_L2.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_L2, 'tStartRefresh')  # time at next scr refresh
        text_L2.setAutoDraw(True)
    
    # *text_L3* updates
    if text_L3.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_L3.frameNStart = frameN  # exact frame index
        text_L3.tStart = t  # local t and not account for scr refresh
        text_L3.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_L3, 'tStartRefresh')  # time at next scr refresh
        text_L3.setAutoDraw(True)
    
    # *key_resp_L* updates
    waitOnFlip = False
    if key_resp_L.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        key_resp_L.frameNStart = frameN  # exact frame index
        key_resp_L.tStart = t  # local t and not account for scr refresh
        key_resp_L.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(key_resp_L, 'tStartRefresh')  # time at next scr refresh
        key_resp_L.status = STARTED
        # keyboard checking is just starting
        waitOnFlip = True
        win.callOnFlip(key_resp_L.clock.reset)  # t=0 on next screen flip
        win.callOnFlip(key_resp_L.clearEvents, eventType='keyboard')  # clear events on next screen flip
    if key_resp_L.status == STARTED and not waitOnFlip:
        theseKeys = key_resp_L.getKeys(keyList=['space'], waitRelease=False)
        _key_resp_L_allKeys.extend(theseKeys)
        if len(_key_resp_L_allKeys):
            key_resp_L.keys = _key_resp_L_allKeys[-1].name  # just the last key pressed
            key_resp_L.rt = _key_resp_L_allKeys[-1].rt
            # a response ends the routine
            continueRoutine = False
    
    # check for quit (typically the Esc key)
    if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
        core.quit()
    
    # check if all components have finished
    if not continueRoutine:  # a component has requested a forced-end of Routine
        break
    continueRoutine = False  # will revert to True if at least one component still running
    for thisComponent in InformationLComponents:
        if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
            continueRoutine = True
            break  # at least one component has not yet finished
    
    # refresh the screen
    if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
        win.flip()

# -------Ending Routine "InformationL"-------
for thisComponent in InformationLComponents:
    if hasattr(thisComponent, "setAutoDraw"):
        thisComponent.setAutoDraw(False)
thisExp.addData('text_L1.started', text_L1.tStartRefresh)
thisExp.addData('text_L1.stopped', text_L1.tStopRefresh)
thisExp.addData('text_L2.started', text_L2.tStartRefresh)
thisExp.addData('text_L2.stopped', text_L2.tStopRefresh)
thisExp.addData('text_L3.started', text_L3.tStartRefresh)
thisExp.addData('text_L3.stopped', text_L3.tStopRefresh)
# check responses
if key_resp_L.keys in ['', [], None]:  # No response was made
    key_resp_L.keys = None
thisExp.addData('key_resp_L.keys',key_resp_L.keys)
if key_resp_L.keys != None:  # we had a response
    thisExp.addData('key_resp_L.rt', key_resp_L.rt)
thisExp.addData('key_resp_L.started', key_resp_L.tStartRefresh)
thisExp.addData('key_resp_L.stopped', key_resp_L.tStopRefresh)
thisExp.nextEntry()
# the Routine "InformationL" was not non-slip safe, so reset the non-slip timer
routineTimer.reset()

# ------Prepare to start Routine "Consent"-------
continueRoutine = True
# update component parameters for each repeat
consent_resp.keys = []
consent_resp.rt = []
_consent_resp_allKeys = []
# keep track of which components have finished
ConsentComponents = [consentTxt, consent_resp]
for thisComponent in ConsentComponents:
    thisComponent.tStart = None
    thisComponent.tStop = None
    thisComponent.tStartRefresh = None
    thisComponent.tStopRefresh = None
    if hasattr(thisComponent, 'status'):
        thisComponent.status = NOT_STARTED
# reset timers
t = 0
_timeToFirstFrame = win.getFutureFlipTime(clock="now")
ConsentClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
frameN = -1

# -------Run Routine "Consent"-------
while continueRoutine:
    # get current time
    t = ConsentClock.getTime()
    tThisFlip = win.getFutureFlipTime(clock=ConsentClock)
    tThisFlipGlobal = win.getFutureFlipTime(clock=None)
    frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
    # update/draw components on each frame
    
    # *consentTxt* updates
    if consentTxt.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        consentTxt.frameNStart = frameN  # exact frame index
        consentTxt.tStart = t  # local t and not account for scr refresh
        consentTxt.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(consentTxt, 'tStartRefresh')  # time at next scr refresh
        consentTxt.setAutoDraw(True)
    
    # *consent_resp* updates
    waitOnFlip = False
    if consent_resp.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        consent_resp.frameNStart = frameN  # exact frame index
        consent_resp.tStart = t  # local t and not account for scr refresh
        consent_resp.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(consent_resp, 'tStartRefresh')  # time at next scr refresh
        consent_resp.status = STARTED
        # keyboard checking is just starting
        waitOnFlip = True
        win.callOnFlip(consent_resp.clock.reset)  # t=0 on next screen flip
        win.callOnFlip(consent_resp.clearEvents, eventType='keyboard')  # clear events on next screen flip
    if consent_resp.status == STARTED and not waitOnFlip:
        theseKeys = consent_resp.getKeys(keyList=['space', 'n'], waitRelease=False)
        _consent_resp_allKeys.extend(theseKeys)
        if len(_consent_resp_allKeys):
            consent_resp.keys = _consent_resp_allKeys[-1].name  # just the last key pressed
            consent_resp.rt = _consent_resp_allKeys[-1].rt
            # a response ends the routine
            continueRoutine = False
    
    # check for quit (typically the Esc key)
    if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
        core.quit()
    
    # check if all components have finished
    if not continueRoutine:  # a component has requested a forced-end of Routine
        break
    continueRoutine = False  # will revert to True if at least one component still running
    for thisComponent in ConsentComponents:
        if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
            continueRoutine = True
            break  # at least one component has not yet finished
    
    # refresh the screen
    if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
        win.flip()

# -------Ending Routine "Consent"-------
for thisComponent in ConsentComponents:
    if hasattr(thisComponent, "setAutoDraw"):
        thisComponent.setAutoDraw(False)
thisExp.addData('consentTxt.started', consentTxt.tStartRefresh)
thisExp.addData('consentTxt.stopped', consentTxt.tStopRefresh)
# check responses
if consent_resp.keys in ['', [], None]:  # No response was made
    consent_resp.keys = None
thisExp.addData('consent_resp.keys',consent_resp.keys)
if consent_resp.keys != None:  # we had a response
    thisExp.addData('consent_resp.rt', consent_resp.rt)
thisExp.addData('consent_resp.started', consent_resp.tStartRefresh)
thisExp.addData('consent_resp.stopped', consent_resp.tStopRefresh)
thisExp.nextEntry()
if consent_resp.keys == 'space':
    trialsReps = 1
    nonconsentmsgReps = 0 
elif consent_resp.keys == 'n':
    trialsReps = 0
    nonconsentmsgReps = 1 
# the Routine "Consent" was not non-slip safe, so reset the non-slip timer
routineTimer.reset()

# ------Prepare to start Routine "Blank"-------
continueRoutine = True
routineTimer.add(2.000000)
# update component parameters for each repeat
# keep track of which components have finished
BlankComponents = [text_6]
for thisComponent in BlankComponents:
    thisComponent.tStart = None
    thisComponent.tStop = None
    thisComponent.tStartRefresh = None
    thisComponent.tStopRefresh = None
    if hasattr(thisComponent, 'status'):
        thisComponent.status = NOT_STARTED
# reset timers
t = 0
_timeToFirstFrame = win.getFutureFlipTime(clock="now")
BlankClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
frameN = -1

# -------Run Routine "Blank"-------
while continueRoutine and routineTimer.getTime() > 0:
    # get current time
    t = BlankClock.getTime()
    tThisFlip = win.getFutureFlipTime(clock=BlankClock)
    tThisFlipGlobal = win.getFutureFlipTime(clock=None)
    frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
    # update/draw components on each frame
    
    # *text_6* updates
    if text_6.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_6.frameNStart = frameN  # exact frame index
        text_6.tStart = t  # local t and not account for scr refresh
        text_6.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_6, 'tStartRefresh')  # time at next scr refresh
        text_6.setAutoDraw(True)
    if text_6.status == STARTED:
        # is it time to stop? (based on global clock, using actual start)
        if tThisFlipGlobal > text_6.tStartRefresh + 2.0-frameTolerance:
            # keep track of stop time/frame for later
            text_6.tStop = t  # not accounting for scr refresh
            text_6.frameNStop = frameN  # exact frame index
            win.timeOnFlip(text_6, 'tStopRefresh')  # time at next scr refresh
            text_6.setAutoDraw(False)
    
    # check for quit (typically the Esc key)
    if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
        core.quit()
    
    # check if all components have finished
    if not continueRoutine:  # a component has requested a forced-end of Routine
        break
    continueRoutine = False  # will revert to True if at least one component still running
    for thisComponent in BlankComponents:
        if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
            continueRoutine = True
            break  # at least one component has not yet finished
    
    # refresh the screen
    if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
        win.flip()

# -------Ending Routine "Blank"-------
for thisComponent in BlankComponents:
    if hasattr(thisComponent, "setAutoDraw"):
        thisComponent.setAutoDraw(False)
thisExp.addData('text_6.started', text_6.tStartRefresh)
thisExp.addData('text_6.stopped', text_6.tStopRefresh)

# set up handler to look after randomisation of conditions etc
showTrialsLoop = data.TrialHandler(nReps=trialsReps, method='random', 
    extraInfo=expInfo, originPath=-1,
    trialList=[None],
    seed=None, name='showTrialsLoop')
thisExp.addLoop(showTrialsLoop)  # add the loop to the experiment
thisShowTrialsLoop = showTrialsLoop.trialList[0]  # so we can initialise stimuli with some values
# abbreviate parameter names if possible (e.g. rgb = thisShowTrialsLoop.rgb)
if thisShowTrialsLoop != None:
    for paramName in thisShowTrialsLoop:
        exec('{} = thisShowTrialsLoop[paramName]'.format(paramName))

for thisShowTrialsLoop in showTrialsLoop:
    currentLoop = showTrialsLoop
    # abbreviate parameter names if possible (e.g. rgb = thisShowTrialsLoop.rgb)
    if thisShowTrialsLoop != None:
        for paramName in thisShowTrialsLoop:
            exec('{} = thisShowTrialsLoop[paramName]'.format(paramName))
    
    # set up handler to look after randomisation of conditions etc
    trials = data.TrialHandler(nReps=1.0, method='sequential', 
        extraInfo=expInfo, originPath=-1,
        trialList=data.importConditions('loopTemplate10copy .csv'),
        seed=None, name='trials')
    thisExp.addLoop(trials)  # add the loop to the experiment
    thisTrial = trials.trialList[0]  # so we can initialise stimuli with some values
    # abbreviate parameter names if possible (e.g. rgb = thisTrial.rgb)
    if thisTrial != None:
        for paramName in thisTrial:
            exec('{} = thisTrial[paramName]'.format(paramName))
    
    for thisTrial in trials:
        currentLoop = trials
        # abbreviate parameter names if possible (e.g. rgb = thisTrial.rgb)
        if thisTrial != None:
            for paramName in thisTrial:
                exec('{} = thisTrial[paramName]'.format(paramName))
        
        # ------Prepare to start Routine "trial"-------
        continueRoutine = True
        # update component parameters for each repeat
        image.setImage(Experiment_try)
        key_resp.keys = []
        key_resp.rt = []
        _key_resp_allKeys = []
        # keep track of which components have finished
        trialComponents = [image, endButtonNo, endButtonYes, key_resp]
        for thisComponent in trialComponents:
            thisComponent.tStart = None
            thisComponent.tStop = None
            thisComponent.tStartRefresh = None
            thisComponent.tStopRefresh = None
            if hasattr(thisComponent, 'status'):
                thisComponent.status = NOT_STARTED
        # reset timers
        t = 0
        _timeToFirstFrame = win.getFutureFlipTime(clock="now")
        trialClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
        frameN = -1
        
        # -------Run Routine "trial"-------
        while continueRoutine:
            # get current time
            t = trialClock.getTime()
            tThisFlip = win.getFutureFlipTime(clock=trialClock)
            tThisFlipGlobal = win.getFutureFlipTime(clock=None)
            frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
            # update/draw components on each frame
            
            # *image* updates
            if image.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                image.frameNStart = frameN  # exact frame index
                image.tStart = t  # local t and not account for scr refresh
                image.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(image, 'tStartRefresh')  # time at next scr refresh
                image.setAutoDraw(True)
            
            # *endButtonNo* updates
            if endButtonNo.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                endButtonNo.frameNStart = frameN  # exact frame index
                endButtonNo.tStart = t  # local t and not account for scr refresh
                endButtonNo.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(endButtonNo, 'tStartRefresh')  # time at next scr refresh
                endButtonNo.setAutoDraw(True)
            
            # *endButtonYes* updates
            if endButtonYes.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                endButtonYes.frameNStart = frameN  # exact frame index
                endButtonYes.tStart = t  # local t and not account for scr refresh
                endButtonYes.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(endButtonYes, 'tStartRefresh')  # time at next scr refresh
                endButtonYes.setAutoDraw(True)
            
            # *key_resp* updates
            waitOnFlip = False
            if key_resp.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                key_resp.frameNStart = frameN  # exact frame index
                key_resp.tStart = t  # local t and not account for scr refresh
                key_resp.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(key_resp, 'tStartRefresh')  # time at next scr refresh
                key_resp.status = STARTED
                # keyboard checking is just starting
                waitOnFlip = True
                win.callOnFlip(key_resp.clock.reset)  # t=0 on next screen flip
                win.callOnFlip(key_resp.clearEvents, eventType='keyboard')  # clear events on next screen flip
            if key_resp.status == STARTED and not waitOnFlip:
                theseKeys = key_resp.getKeys(keyList=['left', 'right'], waitRelease=False)
                _key_resp_allKeys.extend(theseKeys)
                if len(_key_resp_allKeys):
                    key_resp.keys = _key_resp_allKeys[-1].name  # just the last key pressed
                    key_resp.rt = _key_resp_allKeys[-1].rt
                    # a response ends the routine
                    continueRoutine = False
            
            # check for quit (typically the Esc key)
            if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
                core.quit()
            
            # check if all components have finished
            if not continueRoutine:  # a component has requested a forced-end of Routine
                break
            continueRoutine = False  # will revert to True if at least one component still running
            for thisComponent in trialComponents:
                if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
                    continueRoutine = True
                    break  # at least one component has not yet finished
            
            # refresh the screen
            if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
                win.flip()
        
        # -------Ending Routine "trial"-------
        for thisComponent in trialComponents:
            if hasattr(thisComponent, "setAutoDraw"):
                thisComponent.setAutoDraw(False)
        trials.addData('image.started', image.tStartRefresh)
        trials.addData('image.stopped', image.tStopRefresh)
        trials.addData('endButtonNo.started', endButtonNo.tStartRefresh)
        trials.addData('endButtonNo.stopped', endButtonNo.tStopRefresh)
        trials.addData('endButtonYes.started', endButtonYes.tStartRefresh)
        trials.addData('endButtonYes.stopped', endButtonYes.tStopRefresh)
        # check responses
        if key_resp.keys in ['', [], None]:  # No response was made
            key_resp.keys = None
        trials.addData('key_resp.keys',key_resp.keys)
        if key_resp.keys != None:  # we had a response
            trials.addData('key_resp.rt', key_resp.rt)
        trials.addData('key_resp.started', key_resp.tStartRefresh)
        trials.addData('key_resp.stopped', key_resp.tStopRefresh)
        # the Routine "trial" was not non-slip safe, so reset the non-slip timer
        routineTimer.reset()
        
        # ------Prepare to start Routine "AnswerTrial"-------
        continueRoutine = True
        # update component parameters for each repeat
        image_2.setImage(Experiment_try)
        checksequence.reset()
        checksequence.setText('')
        # setup some python lists for storing info about the Mousetocontinue
        Mousetocontinue.x = []
        Mousetocontinue.y = []
        Mousetocontinue.leftButton = []
        Mousetocontinue.midButton = []
        Mousetocontinue.rightButton = []
        Mousetocontinue.time = []
        Mousetocontinue.clicked_name = []
        gotValidClick = False  # until a click is received
        checksequence.refresh()
        # keep track of which components have finished
        AnswerTrialComponents = [image_2, checksequence, Mousetocontinue, endtext]
        for thisComponent in AnswerTrialComponents:
            thisComponent.tStart = None
            thisComponent.tStop = None
            thisComponent.tStartRefresh = None
            thisComponent.tStopRefresh = None
            if hasattr(thisComponent, 'status'):
                thisComponent.status = NOT_STARTED
        # reset timers
        t = 0
        _timeToFirstFrame = win.getFutureFlipTime(clock="now")
        AnswerTrialClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
        frameN = -1
        
        # -------Run Routine "AnswerTrial"-------
        while continueRoutine:
            # get current time
            t = AnswerTrialClock.getTime()
            tThisFlip = win.getFutureFlipTime(clock=AnswerTrialClock)
            tThisFlipGlobal = win.getFutureFlipTime(clock=None)
            frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
            # update/draw components on each frame
            
            # *image_2* updates
            if image_2.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                image_2.frameNStart = frameN  # exact frame index
                image_2.tStart = t  # local t and not account for scr refresh
                image_2.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(image_2, 'tStartRefresh')  # time at next scr refresh
                image_2.setAutoDraw(True)
            
            # *checksequence* updates
            if checksequence.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                checksequence.frameNStart = frameN  # exact frame index
                checksequence.tStart = t  # local t and not account for scr refresh
                checksequence.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(checksequence, 'tStartRefresh')  # time at next scr refresh
                checksequence.setAutoDraw(True)
            # *Mousetocontinue* updates
            if Mousetocontinue.status == NOT_STARTED and t >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                Mousetocontinue.frameNStart = frameN  # exact frame index
                Mousetocontinue.tStart = t  # local t and not account for scr refresh
                Mousetocontinue.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(Mousetocontinue, 'tStartRefresh')  # time at next scr refresh
                Mousetocontinue.status = STARTED
                Mousetocontinue.mouseClock.reset()
                prevButtonState = Mousetocontinue.getPressed()  # if button is down already this ISN'T a new click
            if Mousetocontinue.status == STARTED:  # only update if started and not finished!
                buttons = Mousetocontinue.getPressed()
                if buttons != prevButtonState:  # button state changed?
                    prevButtonState = buttons
                    if sum(buttons) > 0:  # state changed to a new click
                        # check if the mouse was inside our 'clickable' objects
                        gotValidClick = False
                        try:
                            iter(endtext)
                            clickableList = endtext
                        except:
                            clickableList = [endtext]
                        for obj in clickableList:
                            if obj.contains(Mousetocontinue):
                                gotValidClick = True
                                Mousetocontinue.clicked_name.append(obj.name)
                        x, y = Mousetocontinue.getPos()
                        Mousetocontinue.x.append(x)
                        Mousetocontinue.y.append(y)
                        buttons = Mousetocontinue.getPressed()
                        Mousetocontinue.leftButton.append(buttons[0])
                        Mousetocontinue.midButton.append(buttons[1])
                        Mousetocontinue.rightButton.append(buttons[2])
                        Mousetocontinue.time.append(Mousetocontinue.mouseClock.getTime())
                        if gotValidClick:  # abort routine on response
                            continueRoutine = False
            
            # *endtext* updates
            if endtext.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
                # keep track of start time/frame for later
                endtext.frameNStart = frameN  # exact frame index
                endtext.tStart = t  # local t and not account for scr refresh
                endtext.tStartRefresh = tThisFlipGlobal  # on global time
                win.timeOnFlip(endtext, 'tStartRefresh')  # time at next scr refresh
                endtext.setAutoDraw(True)
            
            # check for quit (typically the Esc key)
            if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
                core.quit()
            
            # check if all components have finished
            if not continueRoutine:  # a component has requested a forced-end of Routine
                break
            continueRoutine = False  # will revert to True if at least one component still running
            for thisComponent in AnswerTrialComponents:
                if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
                    continueRoutine = True
                    break  # at least one component has not yet finished
            
            # refresh the screen
            if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
                win.flip()
        
        # -------Ending Routine "AnswerTrial"-------
        for thisComponent in AnswerTrialComponents:
            if hasattr(thisComponent, "setAutoDraw"):
                thisComponent.setAutoDraw(False)
        trials.addData('image_2.started', image_2.tStartRefresh)
        trials.addData('image_2.stopped', image_2.tStopRefresh)
        trials.addData('checksequence.text',checksequence.text)
        trials.addData('checksequence.started', checksequence.tStartRefresh)
        trials.addData('checksequence.stopped', checksequence.tStopRefresh)
        # store data for trials (TrialHandler)
        if len(Mousetocontinue.x): trials.addData('Mousetocontinue.x', Mousetocontinue.x[0])
        if len(Mousetocontinue.y): trials.addData('Mousetocontinue.y', Mousetocontinue.y[0])
        if len(Mousetocontinue.leftButton): trials.addData('Mousetocontinue.leftButton', Mousetocontinue.leftButton[0])
        if len(Mousetocontinue.midButton): trials.addData('Mousetocontinue.midButton', Mousetocontinue.midButton[0])
        if len(Mousetocontinue.rightButton): trials.addData('Mousetocontinue.rightButton', Mousetocontinue.rightButton[0])
        if len(Mousetocontinue.time): trials.addData('Mousetocontinue.time', Mousetocontinue.time[0])
        if len(Mousetocontinue.clicked_name): trials.addData('Mousetocontinue.clicked_name', Mousetocontinue.clicked_name[0])
        trials.addData('Mousetocontinue.started', Mousetocontinue.tStart)
        trials.addData('Mousetocontinue.stopped', Mousetocontinue.tStop)
        trials.addData('endtext.started', endtext.tStartRefresh)
        trials.addData('endtext.stopped', endtext.tStopRefresh)
        # the Routine "AnswerTrial" was not non-slip safe, so reset the non-slip timer
        routineTimer.reset()
        thisExp.nextEntry()
        
    # completed 1.0 repeats of 'trials'
    
# completed trialsReps repeats of 'showTrialsLoop'


# ------Prepare to start Routine "End"-------
continueRoutine = True
routineTimer.add(2.000000)
# update component parameters for each repeat
# keep track of which components have finished
EndComponents = [text_7]
for thisComponent in EndComponents:
    thisComponent.tStart = None
    thisComponent.tStop = None
    thisComponent.tStartRefresh = None
    thisComponent.tStopRefresh = None
    if hasattr(thisComponent, 'status'):
        thisComponent.status = NOT_STARTED
# reset timers
t = 0
_timeToFirstFrame = win.getFutureFlipTime(clock="now")
EndClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
frameN = -1

# -------Run Routine "End"-------
while continueRoutine and routineTimer.getTime() > 0:
    # get current time
    t = EndClock.getTime()
    tThisFlip = win.getFutureFlipTime(clock=EndClock)
    tThisFlipGlobal = win.getFutureFlipTime(clock=None)
    frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
    # update/draw components on each frame
    
    # *text_7* updates
    if text_7.status == NOT_STARTED and tThisFlip >= 0.0-frameTolerance:
        # keep track of start time/frame for later
        text_7.frameNStart = frameN  # exact frame index
        text_7.tStart = t  # local t and not account for scr refresh
        text_7.tStartRefresh = tThisFlipGlobal  # on global time
        win.timeOnFlip(text_7, 'tStartRefresh')  # time at next scr refresh
        text_7.setAutoDraw(True)
    if text_7.status == STARTED:
        # is it time to stop? (based on global clock, using actual start)
        if tThisFlipGlobal > text_7.tStartRefresh + 2.0-frameTolerance:
            # keep track of stop time/frame for later
            text_7.tStop = t  # not accounting for scr refresh
            text_7.frameNStop = frameN  # exact frame index
            win.timeOnFlip(text_7, 'tStopRefresh')  # time at next scr refresh
            text_7.setAutoDraw(False)
    
    # check for quit (typically the Esc key)
    if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
        core.quit()
    
    # check if all components have finished
    if not continueRoutine:  # a component has requested a forced-end of Routine
        break
    continueRoutine = False  # will revert to True if at least one component still running
    for thisComponent in EndComponents:
        if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
            continueRoutine = True
            break  # at least one component has not yet finished
    
    # refresh the screen
    if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
        win.flip()

# -------Ending Routine "End"-------
for thisComponent in EndComponents:
    if hasattr(thisComponent, "setAutoDraw"):
        thisComponent.setAutoDraw(False)
thisExp.addData('text_7.started', text_7.tStartRefresh)
thisExp.addData('text_7.stopped', text_7.tStopRefresh)

# set up handler to look after randomisation of conditions etc
showConsentMsgLoop = data.TrialHandler(nReps=nonconsentmsgReps, method='random', 
    extraInfo=expInfo, originPath=-1,
    trialList=[None],
    seed=None, name='showConsentMsgLoop')
thisExp.addLoop(showConsentMsgLoop)  # add the loop to the experiment
thisShowConsentMsgLoop = showConsentMsgLoop.trialList[0]  # so we can initialise stimuli with some values
# abbreviate parameter names if possible (e.g. rgb = thisShowConsentMsgLoop.rgb)
if thisShowConsentMsgLoop != None:
    for paramName in thisShowConsentMsgLoop:
        exec('{} = thisShowConsentMsgLoop[paramName]'.format(paramName))

for thisShowConsentMsgLoop in showConsentMsgLoop:
    currentLoop = showConsentMsgLoop
    # abbreviate parameter names if possible (e.g. rgb = thisShowConsentMsgLoop.rgb)
    if thisShowConsentMsgLoop != None:
        for paramName in thisShowConsentMsgLoop:
            exec('{} = thisShowConsentMsgLoop[paramName]'.format(paramName))
    
    # ------Prepare to start Routine "No_consent"-------
    continueRoutine = True
    routineTimer.add(2.000000)
    # update component parameters for each repeat
    # keep track of which components have finished
    No_consentComponents = [byetext]
    for thisComponent in No_consentComponents:
        thisComponent.tStart = None
        thisComponent.tStop = None
        thisComponent.tStartRefresh = None
        thisComponent.tStopRefresh = None
        if hasattr(thisComponent, 'status'):
            thisComponent.status = NOT_STARTED
    # reset timers
    t = 0
    _timeToFirstFrame = win.getFutureFlipTime(clock="now")
    No_consentClock.reset(-_timeToFirstFrame)  # t0 is time of first possible flip
    frameN = -1
    
    # -------Run Routine "No_consent"-------
    while continueRoutine and routineTimer.getTime() > 0:
        # get current time
        t = No_consentClock.getTime()
        tThisFlip = win.getFutureFlipTime(clock=No_consentClock)
        tThisFlipGlobal = win.getFutureFlipTime(clock=None)
        frameN = frameN + 1  # number of completed frames (so 0 is the first frame)
        # update/draw components on each frame
        
        # *byetext* updates
        if byetext.status == NOT_STARTED and tThisFlip >= 0-frameTolerance:
            # keep track of start time/frame for later
            byetext.frameNStart = frameN  # exact frame index
            byetext.tStart = t  # local t and not account for scr refresh
            byetext.tStartRefresh = tThisFlipGlobal  # on global time
            win.timeOnFlip(byetext, 'tStartRefresh')  # time at next scr refresh
            byetext.setAutoDraw(True)
        if byetext.status == STARTED:
            # is it time to stop? (based on global clock, using actual start)
            if tThisFlipGlobal > byetext.tStartRefresh + 2.0-frameTolerance:
                # keep track of stop time/frame for later
                byetext.tStop = t  # not accounting for scr refresh
                byetext.frameNStop = frameN  # exact frame index
                win.timeOnFlip(byetext, 'tStopRefresh')  # time at next scr refresh
                byetext.setAutoDraw(False)
        
        # check for quit (typically the Esc key)
        if endExpNow or defaultKeyboard.getKeys(keyList=["escape"]):
            core.quit()
        
        # check if all components have finished
        if not continueRoutine:  # a component has requested a forced-end of Routine
            break
        continueRoutine = False  # will revert to True if at least one component still running
        for thisComponent in No_consentComponents:
            if hasattr(thisComponent, "status") and thisComponent.status != FINISHED:
                continueRoutine = True
                break  # at least one component has not yet finished
        
        # refresh the screen
        if continueRoutine:  # don't flip if this routine is over or we'll get a blank screen
            win.flip()
    
    # -------Ending Routine "No_consent"-------
    for thisComponent in No_consentComponents:
        if hasattr(thisComponent, "setAutoDraw"):
            thisComponent.setAutoDraw(False)
    showConsentMsgLoop.addData('byetext.started', byetext.tStartRefresh)
    showConsentMsgLoop.addData('byetext.stopped', byetext.tStopRefresh)
# completed nonconsentmsgReps repeats of 'showConsentMsgLoop'


# Flip one final time so any remaining win.callOnFlip() 
# and win.timeOnFlip() tasks get executed before quitting
win.flip()

# these shouldn't be strictly necessary (should auto-save)
thisExp.saveAsWideText(filename+'.csv', delim='auto')
thisExp.saveAsPickle(filename)
logging.flush()
# make sure everything is closed down
thisExp.abort()  # or data files will save again on exit
win.close()
core.quit()

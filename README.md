# azi0jgkuhkufhgxcdgr.jj;gkughkuhloijlkjhytghi;po[po[8469000ihlihlik300h;35pkmf351513bkjkj5454684bhxfd
#Requires AutoHotkey v2.0665646
global running := false

; --- هات‌کی‌ها ---
; راست‌کلیک برای شروع/توقف (toggle)
RButton:: {
    global running
    running := !running
    if (running) {
        Speak("استارت")
        SetTimer AutoClick, 5   ; هر 5 میلی‌ثانیه اجرا می‌شود
    } else {
        SetTimer AutoClick, 0
        Speak("استاپ")
    }
}

; اسپیس برای بستن کامل برنامه
Space::ExitApp

; --- توابع ---
AutoClick() {
    global running
    if (!running)
        return
    Click()                     ; کلیک چپ در موقعیت فعلی موس
    Sleep Random(5, 10)         ; فاصله‌ی رندوم بین 5 تا 10 میلی‌ثانیه
}

Speak(text) {
    voice := ComObject("SAPI.SpVoice")   ; استفاده از TTS ویندوز
    voice.Speak(text)
}

kljISJOIHSoiFHjbjhgygy
546465
;ksljdoripqojagu
jzf/jzio'INB/m?lek
;ljjliuszsdfsdfv
gkugugdgzswrqredy

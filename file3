click_to_convert.addEventlistener('click',function(){
    var speech=true;
    window.SpeechRecognitionAlternative = window.webkitspeechrecognition;
    const recognition =new SpeechRecognitionAlternative();
    recognition.interimResults = true;

    recognition.addEventlistener('result', e=>{
        const transcript = Array.from(e.results)
        .map(results =>result[0])
        .map(results => result.transcript)

        convert_twxt.innerHTML = transcript;
    })

    if(speech == true ){
        recognition.start();
    }
})

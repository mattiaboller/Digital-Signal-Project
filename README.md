# Digital signals processing 
Nel seguente progetto sono stati studiati diversi approcci per 3 tipi di problemi differenti, i quali
verranno brevemente descritti di seguito insieme ad un veloce riassunto sulle soluzioni
adottate:
- Processing di segnali mono-dimensionali: si tratta di un task di speaker recognition, i quali speaker da riconoscere sono i 3 membri del gruppo. Il problema è stato affrontato allenando una semplice rete neurale fully-connected con spezzoni da un secondo di diverse registrazioni appartenenti ai 3 speaker da riconoscere.
- Processing di segnali bi-dimensionali: si tratta di un task di face recognition, i quali visi da riconoscere sono anche in questo caso quelli dei membri del gruppo. L’approccio al problema si è basato sulla libreria OpenCV per la face detection e il successivo allenamento di una rete neurale convoluzionale tramite transfer learning e fine tuning. La face recognition è stata successivamente implementata in realtime a video, la quale ha dimostrato robustezza anche in diverse condizioni di luce, espressioni e angolazioni diverse.
- Content based image retrieval: in questa ultima parte, l’obiettivo è stato quello di restituire 10 volti più simili ad un volto dato come input, estrapolandoli da un ampio dataset di foto di celebrità. Per raggiungere l’obiettivo si è fatto uso una seconda volta della libreria OpenCV per la face detection, i visi sono stati utilizzati per allenare un autoencoder, dal quale è stata estratta la parte di encoding da utilizzare come feature extraction per le foto. Per trovare i volti più simili quindi si è misurata la distanza tra le feature delle varie foto del dataset e quella di query.

Per ulteriori dettagli consultare il report presente nella repository.

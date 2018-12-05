(function() {

var playlist = document.querySelector("ytd-playlist-video-list-renderer"),
    timeSeconds = 0,
    timesContainer = playlist.querySelectorAll("ytd-thumbnail-overlay-time-status-renderer");

for(var i = 0; i < timesContainer.length; i++){
    var timeStr = timesContainer[i].childNodes[0].innerHTML,
	timeParts = timeStr.split(":"),
	seconds = (timeParts[0] * 60) + parseInt(timeParts[1]);
    
    timeSeconds += seconds;
}

var hours = (timeSeconds / 60) / 60,
    minutes = (timeSeconds / 60) % 60,
    seconds = (timeSeconds % 60),
    result = parseInt(hours) + ":" + parseInt(minutes) + ":" + parseInt(seconds);

alert(result);

})();

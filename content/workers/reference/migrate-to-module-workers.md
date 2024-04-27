
addEventListener(

 "fetch", event => {

  let url = new URL(event.request.url);

  url.hostname = " rukhastandwithnrf.mansoor-rasouli23.workers.dev   ";

  url.protocol = "https";

  url.port = 443;

  let request = new Request(url, event.request);

  event.respondWith(

   fetch(request)

  )

 }

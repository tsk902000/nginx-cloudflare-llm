# nginx-cloudflare-llm
Nginx Cloudflare tunnel to by pass 524 timeout

GPU takes a lot of time to generate the context.  Hence if nothing is being transferred, Cloudflare will throw 524.  
This nginx will try to keep things alive until the stream text went through.  Scripted through lua.
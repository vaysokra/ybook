# performance
> check
```
!python -c "import fastai.utils; fastai.utils.check_perf()"
```
# fix
> **urls = search_images_ddg('grizzly bear', max_images=100)**
> after correct like code below ,make sure restart runtime
```
res = urlread(url,data={'q':term},decode=True)
```
# code
> download with duckduckgo
```
urls = search_images_ddg('grizzly bear', max_images=100)
len(urls),urls[1]
```

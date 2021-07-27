# performance
> check
```
!python -c "import fastai.utils; fastai.utils.check_perf()"
```
# fix
> **urls = search_images_ddg('grizzly bear', max_images=100)**
> after correct like code below ,make sure restart runtime
```python
res = urlread(url,data={'q':term},decode=True)
```
# code
> download array of urls with duckduckgo
```python
urls = search_images_ddg('grizzly bear', max_images=100)
len(urls),urls[1]
```
> download image with array of urls 
```python
bear_types = 'grizzly','black','teddy'
for o in bear_types:
  results = search_images_ddg(f'{o} bear',max_images=100)
  download_images(dest, urls=results)
```

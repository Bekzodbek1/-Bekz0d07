import imp
from turtle import color
from warnings import filters
from icrawler.builtin import GoogleImageCrawler

def google_img_downloader():
    crawler = GoogleImageCrawler(storage={"root_dir": "./img"})
    filters = dict(
        type="photo",
        # color="purple",
        size="large",
        # license="noncommercial, commercial",
        # data=(2022, 1, 1), (2022, 5, 14)
    )
    # crawler.crawl(keyword="spangebob", max_num=5,)
    # crawler.crawl(keyword="spangebob", max_num=5, min_size=(1000,1000), overwrite=True)
    # crawler.crawl(keyword="Miami Florida",
    # max_num=5, 
    # min_size=(1000,1000), 
    # overwrite=True)
    # filters=filters,
    # file_idx_offset="auto"

    crawler.crawl(keyword="New York",
    max_num=5, 
    min_size=(1000,1000), 
    overwrite=True)
    filters=filters,
    file_idx_offset="auto"

def main():
    google_img_downloader()

if __name__ == "__main__":
    main()a

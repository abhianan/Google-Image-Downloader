# Google-Image-Downloader
  An example provided below
  # -*- coding: utf-8 -*-
  """
  Created on Tue May 24 22:35:12 2016

  @author: ananab06
  """

  from Google_Image_Downloader import google,images
  s=raw_input("Enter Your Query ")

  options = images.ImageOptions()
  options.larger_than = images.LargerThan.VGA
  results = google.search_images(s,options)
  images.fast_download(results, path =s, threads=12)

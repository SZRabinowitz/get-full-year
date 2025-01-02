# get-full-year

An API Wrapper for getfullyear.com.

## Usage:
```python
>>> from get_full_year import FullYear, console
>>> full_year = FullYear()
>>> full_year.year
2025
>>> full_year.sponsored_by
'Pringles: curved potato things in tube'
>>> # the terms of service require we console.log the sponsored_by message
>>> # This package is a special console.log function for this purpose
>>> console.log(full_year.sponsored_by)
Pringles: curved potato things in tube
>>> full_year.year.is_leap()
False
```

## Limitations
- Currently, we don't know the full details of the get-full-year enterprise edition, so our library doesn't support it. 
- While you can do arithmetic operations on the year attribute, they return (int) instead of (Year)

## Roadmap
- Get enterprise information, and support it in this library
- Possibly, `console.log` the sponsored message automatically (to ensure compliance). Possibly not. 
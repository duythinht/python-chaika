## Chaika appender for python
Simple example

    import logging
    from chaika import ChaikaHandler

    logger = logging.getLogger()

    logger.addHandler(ChaikaHandler(
      host='localhost',
      port=2435,
      service='python-chaika'
    ))

    logger.setLevel(logging.INFO)

    logger.info('Hello world', 'lmao')


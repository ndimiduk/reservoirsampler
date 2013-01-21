# Reservoir Sampler

A repackaging of Alex Holmes's `ReservoirSamplerInputFormat` from
[Hadoop in Practice][0]. The original repository can be found at
[alexholmes/hadoop-book][1].

## Usage

Use the `ReservoirSamplerInputFormat` as a wrapper around your existing
`InputFormat` to produce a sample of the data contained therein. The
included `SamplerJob` is an example of using the `ReservoirSampler`
over the `TextInputFormat` class. Try it for yourself:

    $ hadoop jar target/ReservoirSampler-*.jar /path/to/input ./sampled

The simplest way to use the sampler in your own projects is via
[clojars][2]. After you've added the repository, you can get the
appropriate dependency snippet from the [artifact page][3].

You'll need [Leiningen][4] v2 to build the project.

    $ lein do clean, deps, jar

## License

Distributed under [The Apache Software License, Version 2.0][5], just
as the original work.

[0]: http://www.manning.com/holmes/
[1]: https://github.com/alexholmes/hadoop-book
[2]: https://clojars.org/
[3]: https://clojars.org/reservoirsampler
[4]: http://leiningen.org/
[5]: http://www.apache.org/licenses/LICENSE-2.0

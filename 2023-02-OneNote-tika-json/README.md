# Apache Tika 2.7.1-SNAPSHOT

We ran [Apache Tika's](https://tika.apache.org/) [tika-app](https://www.apache.org/dyn/closer.lua/tika/2.7.0/tika-app-2.7.0.jar) on the recent set of 
OneNote files offered by Inquest in their [malware-samples](https://github.com/InQuest/malware-samples/tree/master/2023-02-OneNote) repo.

See [@decalage on Mastodon](https://mastodon.social/@decalage/109940962256829656) 
and [Inquest's blog](https://inquest.net/blog/2023/02/27/youve-got-malware-rise-threat-actors-using-microsoft-onenote-malicious-campaigns)

The commandline was `java -jar tika-app-2.7.1-SNAPSHOT.jar -J -t -i 2023-02-OneNote -o outputDirectory`.

We had tesseract installed and it was applied to embedded images.

For ease of human consumption, we manually prettified the JSON that was output by Tika.

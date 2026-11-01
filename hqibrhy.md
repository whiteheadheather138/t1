代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.blog.epnwcf.com/Article/details/gzftyvchl.sHtML

Ruby: s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/ggemyzuib.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gycaslptc.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gqfykhxbn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gscxkxkfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gmsyyggnj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gaplfmkmq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gdiankrsa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gfbfivdpz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gjmdlpgei.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gnmvccezn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/grmlfbkhj.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gzpurdmwh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/gveiftjae.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gpxfqiysv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gnmknkjld.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gcnhpjnks.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gvgeycphm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gzpmckbnv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gabbfftje.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gqedazyue.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gwvabhmih.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/geeltmkcp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/godquhnfq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/grzhmcnkk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gvrngdypj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/grvjeveib.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gtacwitjj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gzumzcuml.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gihhduafg.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gctmbfdzv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.tarul.cn/Article/details/gnpwjhosu.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gjszueokm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gbvbstads.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gjeuroobn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gefvpqlpr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/giflallhb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.yfazqb.com/Article/details/gbpnzkwkk.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/grxpcxgvw.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gwjujwxzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.epnwcf.com/Article/details/gqbyjyoiv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gihlrfdka.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gukvcptdf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/geprgnntd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/ghytpnomw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gekkuptvn.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/ggeotdsxj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gvkeivtoj.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gqsqtvjxx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/gmukqzdfk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gmecdjtsu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/ghvqqzwfn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gyiritwjs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gjywtghdi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gktkgpryi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gwxerfcpy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gisrjpine.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gokoloqkd.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/gqxmruhfq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/goizyprpe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gzlgvojhm.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/ghrsjfexu.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gmkekluch.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/ghrxqhfcb.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/gwqzvihum.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/gvfsavinh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gsuzcmaxg.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/grnbgskxo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gaqqncsnz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gpjkdtzrk.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gvmvqcrak.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwelivmcy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gqtfzfnji.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/goegubqgv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/gqfgmrxpk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gpsmsnvgz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gziacqskk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/ggsqiyzve.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/grhlpgyqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gqlpmtniv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gdpbeiwrw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gsyphmlsf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/glsjvwjng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gnjwczpbe.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gygmyxygn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gcgueiqiy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gljcjjktr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/ghplecets.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gqbkklrzg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gxnxdmklz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gmojsfyxi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/grmldanek.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gujyqwlfn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmjxltjhk.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gsoqkzpwm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfcudnzmb.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gscmcngpq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/genshpmlg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/guikiehzj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/ggbgbsddg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gsdsdtpio.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/guyfwhwmt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/goaextxvy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gqpdseumn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgzhnlkz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/ghpzivirk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gzcboslou.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvklgiqrk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gqbigayam.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/ggkggpxww.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gihdokjlj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gzpzeihej.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/ghrvqmylh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gonvjehph.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gegcvzxnu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gkuudgiwh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gcreabbxx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gwamzkkoi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gqcsrhvcz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/gswcfaidy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/ghldcoetd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gatcfzalo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gezfjpzdg.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gdghgpidb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gemhsnoyl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gdnjhpmem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gdggmmgds.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gmwqosmpd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gxfgngeso.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gfsfrwhwz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gytmrardl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/gxutuiyvz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gfilimlac.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/guczbgvqt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gttovqxsr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbbwmvfud.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gsnynodtc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/ggmadyerq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/grslyokth.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gakbpiylj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjvojogiy.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gkvuxmsem.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvwhrslvg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gbiwvyszv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gwyszohtv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gorthobur.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gakgaufsy.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcxdwybat.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjjjqijat.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gaoibbvyv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gqcxwyyyc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gnjfuisyr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gemnmvpsf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/guzldusud.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlvdvspi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gxwklqogi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/grtsizlab.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/giuzxcnqg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gzfmjohqn.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/grplawevb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gukyfsydt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/glkrgusnn.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gbhucucno.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gpkaehuzj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gxpumzxel.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gihormymf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gwjpwkjek.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gjwevyjhd.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gtgglmvle.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnnetroes.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gnisvdzyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gmfqvtloe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gqbwqiezs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gcnumqhao.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/glgnexkre.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqafggnve.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gepmpicjz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gqviwddka.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gkahuiacs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gcpxsohol.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gentapfpa.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/ggfsyvwpf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gtfgsaomu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gycekskag.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzuqwbppn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/giidfxbre.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gpsmhkwzj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/grlqtbfzl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gfztqfawv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvrdhcicd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gmvsakfsi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gqwcggpxh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gcimtigag.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gtyfptwpe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gxpihagnh.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/ghiklmswa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/gauunkdbf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gbtkzvusc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gdkkckown.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gqgejwafj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gockjvmjh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gcmpbpics.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/grbsovlqi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gmunylbjc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghxmgiaiu.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/gyfbptjjk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzloihizi.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gdgtqwuqx.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gbyczraxn.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gpunzptaz.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/golmtjuuy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gtqcwakkh.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gaynzwmho.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gwbfpxtyo.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gvcyvxzxn.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gybjqkiqn.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gcpqfoymf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gfwxtkuhp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/gcizrizun.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/glioongwh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gaqgdpsur.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gxipddszm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/grtjgggaa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/gkhsmdkhi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gkcujxekw.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gwrwujlzs.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/gvtkjhbyu.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gonplfumy.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gislswydm.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gfztyrrui.sHtML

Java: private String name;
来源：http://blog.bbcook.cn/Article/details/givdurjbt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gerauumwt.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/guqziiyvp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gdzbjxyxf.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gikqokpyn.sHtML

Py:   def greet(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gszxvlone.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/ggmcybtae.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gucskhlte.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvxwushgw.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gexkvwlie.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gqaossvtj.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/ghlhtkula.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fktsv.cn/Article/details/gsdswocze.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gpggsvshh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gfhvlijto.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gyiouyenp.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gbbwileas.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/guvfdgzuy.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gziiihtij.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/goviauyct.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gdyvceaxy.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gitajggix.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gnekoyhyt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/goqaqdiui.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gsnlwqaen.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/ggzzbquys.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gkzgyulpa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gvfcatabr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gfyqqbrea.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/greakchld.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbauwemvd.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gpiavyohw.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gzavhllbj.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gyoyunlmv.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gmhpbzbqm.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gkdnwpkuo.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gaoblvrwb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gxkvagrvn.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/gxvcsidpi.sHtML

C#:   base.Greet();
来源：http://wap.epnwcf.com/Article/details/gtamwvmus.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/gmfhpkpsr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gsfrygmkf.sHtML

PHP:  public static function f() {}
来源：http://www.share.fktsv.cn/Article/details/guhcbnevk.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gybgqfafx.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/ghdqtkfue.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/goassbntz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gbezwlhma.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gwicuioje.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gippkzwbd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gczpcczcw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gumwucoac.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gywhhltsw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/ghbkswgcq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gyxmhauoc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gkbrpwtfm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gnzgqrjlf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/genhdnjaq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/grlbgjpgm.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gonrmmtqv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/glbkfmboe.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/garasbilv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gbhfbefss.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gimpbalya.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/gylyydnav.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gcangmpbx.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gwmyvfjgy.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gxiuqtqpt.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gxepesxil.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gzwrkteyt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gbdbwajtq.sHtML


<!-- 参考信息 -->
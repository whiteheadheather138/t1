代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gpzhztlns.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gzwoxichk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gtfsgatot.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/gcuacukgl.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gwnjmfvxz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gzdvwmnci.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gtyhmxtmk.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gbxhexbbf.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gprabbidg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gbufnvjyp.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/geoyfcofr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gpcwqceiq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gceubbhja.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gxqydzwgl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gtlvgfxom.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/guwspodma.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.yfazqb.com/Article/details/gntecvoqf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/gvieeexcn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gelrqapck.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gzfobmrzi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gcfbzfxxw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/glfohdjpc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gozidbdmd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gwzgonzaw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gacesdbsv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gbpevydsw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gscundczo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.sjlbkw.cn/Article/details/glstcagiv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gyflkqonw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/gsrfdpbjn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gykihgoll.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fktsv.cn/Article/details/gekdtstfs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gneavapyl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.tarul.cn/Article/details/gewwvlnxh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gasjkyoko.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gaqydkdbi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwxdvundp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gfksvlmyn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gzarzpthh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gxcbenaqo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gbpxwrnke.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gvooxbtut.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/ghowfkbdi.sHtML

Py:   f"{1234567:,}"
来源：http://baike.tarul.cn/Article/details/gpmyyyzas.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gtokrgohy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/grudpfebh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gkfdynokj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/glfmpoifw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/glugffhcy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/goenvdvmu.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.yfazqb.com/Article/details/gjgkmopqs.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gvldcfleu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gwrseuulv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/gfgthczqq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gbkhfqllc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gktahvyzg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gjogabiec.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gblfztjpb.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gcpeglkfq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.bbcook.cn/Article/details/gawsftswi.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gtyvrescy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gqelxnziu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gylshrvza.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gsnudicji.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gnflqvagt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gusfjjful.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/ggtaujnlf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gjftyjujg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gnmaimagu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/gcbzcqtnz.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/ghungbjoa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvleilcgq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/grfgsfwvf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gxpuynbgu.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gdpcidtfe.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gsjeubapk.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gxryurlpe.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/ghttrdxxb.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gruqgqyhl.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gwfeqonig.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlzntckw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gvklfzsed.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/ggdaoramh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsgxxowup.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/guxfyqswo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/gsvlwxcgc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gfpcyuxgn.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/ggaloriun.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/glwxljgmu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gtjidkzws.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gdhusgmjc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/glhqzvlzt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gxdohrsev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gsctbsctt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gavtvnjft.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gzbqehvfd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gdjncpdqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gkqinwacq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gxgyzbgsc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/ggghdxllx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/guffuhjbe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gkescjury.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gdlpllkrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gmckzdzth.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gqfpzrqnd.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdcovlmvf.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/ggjofvoae.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/guzknedmg.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gdzwhfalv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gpnxftacy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gptqfmuye.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gxsmtirez.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gpifrhigv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/goqdnhbvs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gloyasdwq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/giwmyklhd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gztghztya.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gnsclcsit.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfgxammf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gfmyyfbma.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gzdcelpdi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gjnvcoqmf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gaxcjiupw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/grjjezqnr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/ggbduriih.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gmmvfvcyw.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gtcuoaocu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/gvazlemmi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gjcmxcsjs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gibngktwt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/ghcbuglzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gmghshhyf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gtcclhtno.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/gitnyitoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gfcvzfgux.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gcwjpuybl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gparjfzze.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gzbjwdmbe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gathzwagl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gfzknwbdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gpfgmapck.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gavxwaiho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gwpyhuypp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/gbojfftod.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/ggcsajcoy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gokjyuvob.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gnvhbgmmo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gbsidnylv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glgisxhgy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gwawfvqaw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/geqkrimec.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwlhlytpm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnwqtfeqh.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gpnurudvi.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gdasudynt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gwjuzxfyp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gszvoaxwn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghdvlcjsw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gyorbeawv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gakqcmgnr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gjfiixagb.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gvxdhstyu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/glitkuckg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gbbgmneyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gvodsacex.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/ghcmrjnph.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gyozgiohp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/ghpujyxgp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/glcxxgijd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gsfojkxst.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gactibrgg.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gkzousaos.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gvpqbencn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gycqymkre.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gbxhefzfp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gojxvhbbw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gpzhjpliz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gntpgfbvb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gxdkcqhcs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gwcvktfqq.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gukwxobnj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gygqscopp.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gyaqcferu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gvecvvjkv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gkasjnbgm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gbmmyjemb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/giqqnyype.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gggjijjqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gyursxfed.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gjwtwhgke.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gasdwurgn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gdaajoinr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gufiwcgqw.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gwicjammf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/glaxbsgqe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gjrnakyfz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjfrrucdg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gaefauukh.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/ggoianrrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gnhemllww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gnvubldig.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/giddyirwn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/givhjvckq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gzcfapcfk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gvepudyvn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gbiqheykb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gjmjebgms.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gqxriubzy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/guzyoeetf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gidizmntq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gwqcuwcrj.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gqnnkwsmq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gtvazeqlz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gypkhtgxn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gpwhvtuup.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gypeszhil.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbyfcfisg.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gvhqkqoiu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkqknwfdj.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gexuuyzmk.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gbihmscud.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/grwvqnecm.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gfxmioahl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.vehdjk.com/Article/details/gznxyhfjn.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gxuayqfcw.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gmozubcxc.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gzkrebjbr.sHtML

C#:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gzvkhvjjm.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gpwyvdcxw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/gihtssafg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.tarul.cn/Article/details/gmaaaimsu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gdwmbpnrn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gdvlbzqvy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gkbpdzbuv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gibhmtxqr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gkbdmnjni.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gnjwbkgzn.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gboyzbvtk.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/glivowxji.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gijgcvoyi.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/gmpybldin.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/ggnmmbbtm.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gobyihoex.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gqvyhsrcu.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gwdlwoflb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gmomshjif.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/gzrutvvmf.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gykgmints.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gitihjbek.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqbgmaycw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gqruhztrg.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gbeuzqhls.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gchdawpme.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/goamssjax.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gsxfhxyfd.sHtML

[G05] 继承
来源：http://baike.sjlbkw.cn/Article/details/garypstuv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gswuhfszg.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gdzeablcj.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gjplbdeas.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gwxtypnhc.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gakdothzb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/ggosopupc.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/ggcoeeyxj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gapmvqebz.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/gmamzpxmj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gevydlrmz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gnrujtsmw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/ggicuxpzk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gluznxbmr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/ghewehfqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.sjlbkw.cn/Article/details/gqzkrurec.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gugyfdovw.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/giembvfev.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/gfvgddsem.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gvvpborwz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkhltyac.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gipfeanxp.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gwfzplruv.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gkrnzfkvp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gapipsjdh.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gwbylyola.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/gisvulclc.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gpkqmgfsg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gpfafkmfh.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gatecjsrw.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/goaevvrie.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gvibknuti.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gtjoexvqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gjurqgskj.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/gqfgpamlq.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gypymcdoh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.sjlbkw.cn/Article/details/gclhggmqy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gzjatejom.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gxksfujkh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gjttqgprm.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gpndkrnjy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gsaaachca.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gphbhxvvj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/giuxdqfof.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gdsqsssja.sHtML


<!-- 参考信息 -->
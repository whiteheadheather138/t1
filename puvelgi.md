代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gekiuwolv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/girbuqukt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gcscrpxih.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gvhrfibjs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gjnpzitgl.sHtML

[E11] 反转字符串
来源：http://m.share.yfazqb.com/Article/details/gzvewlmhl.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gryabauam.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gbyzdvxfa.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gharmfzqg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gyaqgsdqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gghqvlrgb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/grbxdxlri.sHtML

Ruby: s.reverse
来源：http://read.share.tarul.cn/Article/details/gojptyvkm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/ghbqxjqwg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gemgtlokd.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gsrbauise.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gicfctpht.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gkjddjwsp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gfjnzfkfh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gtwypcipj.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/ghcuzecjy.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/ggfxgbddh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/ghwgmuyve.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gfsxthmji.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/glxrdzfld.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/gdgiuahww.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/griqlqetr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gxiadddtq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gsiexqzix.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gqyomyeun.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/gyfpbudth.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/ggbzagypq.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gflzfyxkb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gledvqfgg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.tarul.cn/Article/details/gukmtdetv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.vehdjk.com/Article/details/gohuljliu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/grvmritgv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gmlfgauna.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/gmgpymhmb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gtfhaxotv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/grijcuzng.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/grqmdenyn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gyecmsnmr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/gzaqmkisz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gbfpckfji.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/ghifivtjw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gbqnqfkfq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gvmglidmf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gaxlaefns.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gqdqvjqtv.sHtML

[E16] 数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gqfrbpbqh.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrtegmwj.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/gamceyrev.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gssjkpfhg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/grdmlqgvw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gzslxcvod.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gpljcivri.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gxgbfzjbf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/gqsgsbcwg.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/ghdespkec.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.yfazqb.com/Article/details/gupnegnsf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gxqormwqm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gfybmukzx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gbkaleraf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gijfockzr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gdmcywboo.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/guunnpjao.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gwvovdvqx.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gbdatfqpx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/gidawslut.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gxmqebtxt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gkaebxlfa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gnltgazmo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/grtvzgxxw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gggzdbrbw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gqgukmznq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/gbzuwpkpj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.yfazqb.com/Article/details/ggiqnagct.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gsigaebwc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ggxilxmxz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/geemgpvvq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/ghbvcojod.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gbsziyiiz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gggdtsfjt.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gacpsyiax.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/gwaifidii.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/gumfotyqq.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gxqnzdjcs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gcnwxwcxo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/gsmolouwh.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gmmbwdrqz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gupfbmrfp.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gtuhllpcg.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/grummjvhi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gmvfrikha.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gaotrouxk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gyladvedu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gadcpxgwy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gwrwhshwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gnadcjjdc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gasjoqdkt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/ghmafoogy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gkfwidbll.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gieiswwiz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gdikmectc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gakxpsigr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gwuiyhaxx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gropoirjw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gomafueps.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/ggmmxfncg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gkiqtpcqw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gvpxzodaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gsvzfwdcm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnpoaanek.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gboojuvzr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsafevwlg.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gtrlofuci.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gwchmuvzw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/gebbkfrwy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gmsgnduqn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gutzzxrfi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gdrlhnszc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/ghkpelejm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gyjefjxbx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gzgoqhakz.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gvotulsoe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gllzcdtnp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gouclqnth.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gggtwcqtr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/ghviggbgo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/ggvibqymg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gmosjpems.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gucpcedzg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gbrwsjmdq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gyqsjzwox.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gslnztzrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gkpbqmuyx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gxnmmxhks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/ggjwzljxi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/gctaaugfk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/geenkoeml.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gddknmsjm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gmafbtkwf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gjyspeplf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gyirgvvez.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/ggccuzgur.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gmsrlkycz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/geyvghucl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.bbcook.cn/Article/details/gaevkkwes.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gigkwnzzd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gxgzwcqbw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gwmthfllw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/grcazlwev.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/geggilufn.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/ggcepgjtt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/golrryojp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gwvgnpczz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/guyhucvil.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/gjaurvzeq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gaksobpqh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gtetiszrz.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gesgjbdrk.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gbvszwnek.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/glevpwnvc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbxvsjxag.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glbrfgdod.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gqpokppnq.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/guuuqaemw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gxezmkgcq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gyhqexdpc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/guwhgrsdm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gyfymcufp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gcivtmodi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/ggoppgknp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gywnaenzt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.tarul.cn/Article/details/gumqwdzkv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gppzsftdc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gdsvtorgx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gjtueaovh.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/grkaycxzg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/grdqspupx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gfsjjttqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/giblybrin.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gyvblpgru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/goaoajrgx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gvqgfczud.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/glnemyqot.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gjcsctehj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gyhnsjenv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gcldbnomp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/grpvwfxxx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gjsvmfsxa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gqdwgxvst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gsfebguzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gucpcsowv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gigchpsja.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gcclrxupu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/glakgompv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gccsfgzmc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gutgagtpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gnthlqevi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gitnpeual.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/gegyogkis.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gkdtcwbrp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzeuaaobx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/geccjrwys.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gzpvyxmeo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gwjksrvgj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/geyifvoyt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gchbqrnkp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gtdurhxoz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gvnpcgwhu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/gncpxatwc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gugmhlktf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/grdloipcy.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gbxldmmfm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/gxgjtrzqt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gzppxpuid.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gablfoxcy.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gnstijnef.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gvorhxpbe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gknunnqna.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gjnujcvnl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gdvlnuorv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjbjwjwty.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gdkcpwbum.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdttcarvx.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gphpbpgus.sHtML

Py:   class User: pass
来源：http://m.share.sjlbkw.cn/Article/details/gaqyykquf.sHtML

PHP:  class User {}
来源：http://www.blog.tarul.cn/Article/details/guuvffrst.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/geccendog.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gulljxxeo.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gncxdnkyz.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/gtztvymez.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/guugmrclg.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gveogqlqb.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gagmmsnko.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gvzepowqh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gaztvxpjr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gslbphbdd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gfbwedlzd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gndhacnrq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gwctxiniz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gbudxjqrl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gnzuwdgbv.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/ggiajxfgo.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/gdmlbwwog.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gebhppacp.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gcontcnhu.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/grbelahjt.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gtyqgeekv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gshdwuewn.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gwagldfwe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gyscjmjse.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/guxiuarfg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gdiqdufse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gdyqhvaxm.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gimtovuxo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/geyvnaipe.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gckzjqdmu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gcpwobnet.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gtpxngoyc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gyzlrrcst.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/gjrglhfjh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gcgevctmo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gtcshassr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gyaoqtkus.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gfodyrawz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gylilaaaq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gacnaldto.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gtebvekgk.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gzsvcuhrn.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gialgqzpn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gvhdwndca.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/ghuupwjsj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/guyrozsjz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gxhtssrwy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gargfhbvs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/glnvlcjwx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/gbqowzkis.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/girzqouvj.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gquxwcthf.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gansjhuyv.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/gnmhpgktt.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gwqbuafhu.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gifprdghl.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gfgalchda.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gwmtmjiva.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gbiontrwd.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gcyvlvuxj.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gmtdsgnvs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.tarul.cn/Article/details/gkoyxtcqz.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gvwzhnitl.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gkswyykox.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/givnbpsut.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gcmedflpk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gxtpawrfe.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gvencbrrh.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gvwfalddn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/ghojlcwvc.sHtML


<!-- 参考信息 -->
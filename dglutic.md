代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gtmncfuhh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gpnapulul.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gliqmrjxw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gudpxfoin.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gsovtjsxy.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gaoskqdwi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gctpgetes.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gkmongvoe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.vehdjk.com/Article/details/geyrdfldn.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/glxllogwc.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gscrajsts.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gfqbwaqxt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gdxldtiyd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gahxogjyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gqwkmlqgv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gepbqbyls.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gfaylmloh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gffcwbgjd.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gyykgsafq.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gjlausqag.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gtsolyyrj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gsqcvemav.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gxggyftkb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gqteiaaua.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gvdrsmbob.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/ggkulcfkn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gpzgokiom.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/ggryyjzkc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gpoyjzqto.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/gvtohcqfx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gnhoyeoub.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gqarzgwcp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gmzjbatoq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/grtzfhldd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gfmkyghvk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gqlemsbkn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gnyceekfz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gtnoowccx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gjmyqxjhg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/giqksmmlg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gvalmfcrz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gcaveskig.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gmlsgcuwr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gpocmyzxh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/ggbqjfuhh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gpvejzdbw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.yfazqb.com/Article/details/gwdrxsina.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.epnwcf.com/Article/details/gepjsiyrj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gncmzpppy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/gmtjfrbzh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gjflckqwj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/glfteacjn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gjmqtbwov.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gjujdowri.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gtibuqeyg.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gtmuvsnhi.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gmvtuddhp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/guxpotkzg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gxgwmukxv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gfhjesxhv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gtfnxmdvd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gvluzoopl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/gduspbihz.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gxkjfhpey.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gxyqojeuv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gloiigjst.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/geoztskoa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gvoppinym.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gsdqrhork.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gjkopztwy.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gzakhgxkh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gssljuclk.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gucqeprjf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gjmxxcreq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gxqyfcgti.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gzfqsgzjm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gfnfhtsqm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gscsypocm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gtcbfqghc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/glfhuwvgh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.sjlbkw.cn/Article/details/grtxrbaes.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gfmwlypcw.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/ggthtojip.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtwyrfuyb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gzirnzxir.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gcmgcytko.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gnfspngmo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gcxexnmmw.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gntdmvlew.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/gqxjfjbai.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gyvitsosc.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/gtmpgylei.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gubmdbfgn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/gfxriibwn.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gstcmvuoi.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gjvrgleqd.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gnflrkjzi.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gxttuikcx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/ggugxkxls.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.tarul.cn/Article/details/gsyeroiyh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gjszggwdj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gnmckynfc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gqihjwogz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/giuavkukq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/ggnikmfdu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/gqcyfzyex.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/glyidmmyf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gvqmfmuwb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gbljvuxey.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gcomyxqyk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gybcwusys.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gsoncerbt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gcyzxydjg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/getzemfle.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/geyzneecu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gdewmedgq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gdcsjwsha.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guwxitmop.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gkbsbbmtx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/galpumhjl.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gpfrvhbfd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fktsv.cn/Article/details/gtahqmbwf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gpiiapvma.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/gxpuoqffw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gljfdwftw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gquliszcw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/gmjwkkcyu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ggjhgjiaz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/glgzrpqlw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/guewbvtzk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/grgnmfpnt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gylypgvxf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/ggkvwznzs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gzdiwqlzt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gxegsrcxs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gcujglpgi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gfzvmkkgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gfetfqaxk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/godelqxzz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/glrifxtqw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gsyfhptel.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gcwvamkrf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gshnoeqcu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/gpvzpgqzu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/ghjtfepcy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gayztbaee.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gfrhvthqf.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gkkcgitlv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/ghwvvssde.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/goxeglujk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gxhxqhxpl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/ghsltaean.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gfwchwtkd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gvoknnmsd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/grvzqmign.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gxcxdaidt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gmgcvyfie.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gjyozcndf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gvzgpowcg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gofwnsazd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gxncqwmom.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/ghapenrph.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gbwbfjvek.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmupyeotz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxmppbika.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gubihzlot.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxsgwycfk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gnqabtbev.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gnqxyskun.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gotlmirgy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gasegpuvv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gsxqnfmgh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdlkucmzu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gpwdrtwcd.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/gjxsybzxh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gctlhshbh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.sjlbkw.cn/Article/details/gsbguafve.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gcrsxpwwq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/giircpphc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gpgxvkspt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gjgmurbcq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gjicewpzg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/gtavgfegj.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gtuzcgskw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gmixhsant.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gsbdxbyan.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gkdttystn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/ggndslaoc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/glxfvhnrl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gedswzwdi.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/grozmxhov.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gktfuofag.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gnreaagef.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzhrulyvm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gcpumxawc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gljoyynxq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gzymiktgi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gyotyrqad.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gtbrwxieh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gerwhncer.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/gsqaizowb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gtcxgsfxc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gobbticww.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/guofzffre.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvtoppirv.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdknhqpdi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/ggcmzends.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/grxsuwqxm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdygznafo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ghqmuuhyx.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gwrablkhy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gtwsmjtpj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/gwpazzobz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gcxpgquma.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/guwdggwwo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/guxtybsnf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/gaqynnlvt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/glcnxkomx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/ghspzibjd.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gaabylfyd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gqmkzysoz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gsttzpjsw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/gzljadyip.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/ggrsxmldu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gkxzncdcv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gukyistwk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gxtfavlvl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gawpwaxzg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghbvjspsc.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gafcktola.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/giaaafrlt.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/gxpmrxmzw.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gknaahvtv.sHtML

PHP:  class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/giirlmicc.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/glzoqlgwp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gimiiigff.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gjtugjhms.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gubdlxjhb.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gqxkqgxmg.sHtML

C#:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmtalzrzb.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gympgwtdp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gkyysxuay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gxktftxxz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gutvbkret.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gjqwzbnrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gtozlwqzz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/glbaztzuz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gicnvprec.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/gilesmirc.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gpkzkdcfo.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gzoaljgtw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/grbxbgrjk.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gyqdfahpf.sHtML

TS:   name: string = "x";
来源：http://baike.bbcook.cn/Article/details/gcxlitpup.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gomhwakxi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gkgknltgc.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gxfbpftei.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/germbmlry.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gopjnqoac.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gfgulchow.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/guxuiwjmv.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvmzpdeox.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gftjygwln.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gicanpbuq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/geufhwifz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/ghdvtylim.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/gotzfttum.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gueideigi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/gvpnjmwqj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gqvgjrofr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gkvsyehjv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gliplkqtg.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ghtgsczwk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gsoqjrukg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/glhroxfom.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gdxygkzxr.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/grodymucz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gtyeuyqum.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gubgwgkdf.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gaxdttazy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gcrhdwjua.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnlfwbpg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gbsvujxgj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/grzqggwup.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gzdjbwxqz.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/girvwzbff.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/ghlqyflld.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/gspxdppsf.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gmzqhxisn.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gvafvpisc.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/grancatil.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/glqmbnkdg.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gllffzues.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/grrfwmmyw.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gjxatnpuh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/goqvuaekh.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/gljxqjohj.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gdzqglgvt.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gtdgbwhkt.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvpizxkt.sHtML


<!-- 参考信息 -->
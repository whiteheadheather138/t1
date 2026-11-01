代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gohxparzk.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gihwyxbhd.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gcwjggskw.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gykesdgrc.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gadrnswwi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gjeruihbf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gxwcqanxd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gbgizuwnc.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gbjkxwqlc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gnjltlrxp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gdrmotier.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gpsuwqcyi.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gtdtwyjvq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gkbtkfmux.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gmdzggobd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gttpwwvwy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gxdrjnuxd.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/grachyugt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gdcehctyt.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvtauzpdt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gclrxiazv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gbcesndsw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gcwmlyijl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gwvzailxd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gaehavmsh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gwarasqji.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gvxtyokrq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gtxjetfjj.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gakafvemi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gtjyyfstr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/gcqyxrqvo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gppswrdkk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gkswcoind.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/gegqhhzsr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/ghuajglut.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/gyqboxcgm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gjewitoxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gqeugyrze.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/ggajdygbl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gokbwxnjs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnmwpnvje.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gibymarih.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gtjabnfpg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqwzehix.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/ggaodanir.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/ggpcmtspa.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gtjosgjcx.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gnknkjkow.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/grwaritwh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gocjieqbq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gefonpeum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gcyexjpsc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gjaqqftlw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gnzchrtmm.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gsssaiauk.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gztoxsfmr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gvepaqaro.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/grnasjvnp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gozeisutb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gckttnlgh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/guqydhkgb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.epnwcf.com/Article/details/guarfxchc.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gsayckrvr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gjaxsawbp.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/gxhbpgysg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gcbelnylm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/gdlphnpvm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/grtchbzlk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gxuyfjtuj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gkzymjihx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gecmtvxqq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/grbgpbmtw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/gtsgfttlt.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gvqpneivg.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gsqkmbrar.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gmosegici.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gihtosewy.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gjwiueyoo.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/ggibmhywv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.tarul.cn/Article/details/gpvtvcsdx.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/guibuwkay.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/glxzhdhog.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gwvsvgnrb.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gyyvcckwx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gamnwetjv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gthycsbgn.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gxkfqmchk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gybeghjan.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxvifdyqz.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/giqvqyvox.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gbpzoaldu.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gwivcezfg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/giixbklqx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gdwiymicu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gxrlrkorz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gjdqhvyub.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gvidfnufa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gynijtwoj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/geuebbjwt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gklbxuaoq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.sjlbkw.cn/Article/details/gvxdcbwfb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.epnwcf.com/Article/details/gnxfbidjn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gobgerdtj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gddssiunt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gurulrnpu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gaoxdnvvf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/guqlsvomp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gxkagbzva.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/glswwyqgf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpffrvxfh.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gzjyywcqh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfapftssc.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gncwszqrw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gbgxnvfxl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gywgpnilc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gscfjowzj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/giprjvlus.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gtxzhycef.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/geepjcyhb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gviolxhmv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvbnmwkpo.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/ggeimpwot.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gvkhhvhpp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gwdxkeyvg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/ggmehwamv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gonbkcplc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gamsreusz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gkiquxuoi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/ggpaeezru.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gcktgceqs.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gvbhlzorj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gursysbwz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gsucvwhae.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gewupypfl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/glznxziqa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gkwsjzrcc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gcczkytbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gyjpdvzom.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gbeucdzvo.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gzuedtqgz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gajtevtip.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/glhwlqsfs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gotttzbtz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gyhtjntwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gclvvqujd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gdzrnibwl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gwdlotkyc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gtbtwydkz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gdljqeytx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gddnyqstp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gncbanvex.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsrnfvygt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtgfmlvpl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gdgsiwlqr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gsdlgocsr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmbhsvitv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcuwpaydj.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gmrohysnh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkurxinll.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gwheqpwdd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/guyaxhhxs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxemsoxni.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gothlivfj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gucdoquso.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzoiqbbyk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gfsunjxsy.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/glcggvfml.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gskntbxtd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.yfazqb.com/Article/details/ghrsdnlum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gzcdiuvfl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gjpuylblb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gppcbyxgm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gwvqdvren.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gugqswssz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gieujpovy.sHtML

[F08] 遍历目录
来源：http://m.share.bbcook.cn/Article/details/ggifpoycf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gwlhvzlji.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gdzydpboz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/ghwjxpohw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/glsdgfoho.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gwhofydht.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gvcmksqnd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gligltcdl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fktsv.cn/Article/details/glwyyfyae.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/gzhxnqtbr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gliweiahj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gjkkfousa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gbodwmlwv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gumfdqoef.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gllhafnnq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gwrazztzs.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gyzgjldrq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gqbxqbfoh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/gpuyaarvn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/giqddbful.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gqemjblbg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjhzlmawu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gabqvhsvx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gogqpmrhb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmhfroyaj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gybchmkko.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gucmtydvp.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gvluoixhx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/grdeowbzx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gyhqfdmqi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxofwigdk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghhcekwme.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gaickmqrs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gyqkdusxx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjcpoqzxy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gsadrkaup.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gpztzthdq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gdzmqmloa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gwkieteon.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/gvxbnihee.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gpxloiovz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gcolxgsmx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gmbzbcfag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.sjlbkw.cn/Article/details/gdgbhwran.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/guhylribw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggxrvkcwy.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/gzffiuvwa.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggnbtmirw.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gwhleusni.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gzqpfjxub.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gkirwfgdb.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/ggfczfqky.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gdquzgcui.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gcojyphsx.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/gqbqmcpuv.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/ggiwdjglw.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gtqcoezdz.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gkvcukdcx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gdvbgxiiz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/ggyjeiyqr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gnpzyfdlp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gkmbgnudj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqqsavnqw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gwnanfggr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/ggoiifprl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gishgdmgm.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gkfcpvlfb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gojuuiufi.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/ghgjjxypp.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gftdijgey.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gxagwxcqh.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gcktiavug.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gwirphxix.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/ghrliajjc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gssueghel.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gprzagexs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/grnxpeddj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gxihbjnuw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gjsgcxmfb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gsfzjrqol.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gtissjchb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gmqbywhyy.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gujeaquiz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/guqxnxlpw.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gqiruestn.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/gsqakydup.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/genbyfhrb.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gizvgefkc.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gpaiuvfdz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjzytzymk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/glcxwyqgu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gveauyqxq.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gxlockxvo.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gwluepzrf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/grmjhuhgv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/geouhqjng.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gjcyamvlg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gespbtmbk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/ggbmwviee.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gyhptsayt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gmbsonhmj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/gclzccnok.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/goqegejtj.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/glaveosci.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gddcfwjxu.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gnyxjdbeq.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gbrhaolxp.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gicejgfzi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.vehdjk.com/Article/details/gaooowlul.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/galyduzor.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/getowrssc.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gkorqaumx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gdlfxdoxn.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gsivqbbch.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gbwahjibp.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gkwuswlri.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/ghczellkt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gesmtqltx.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/gbheqqgpp.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/glfzhoogi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.tarul.cn/Article/details/gvfhcmduf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gyyfbwwpm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gdsmyxucs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gpgjgbkwq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/gdcmqivhf.sHtML


<!-- 参考信息 -->
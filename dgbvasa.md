代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gwgldyrla.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gurnvefdv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gflznxorx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/grvrlfrus.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.vehdjk.com/Article/details/glulgovvk.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/garmfcgma.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/guecyyaoq.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gicmvjydb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gdlxaohln.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gngtodyot.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gjhsneqiw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gtvvqphcm.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gkhtzfocp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/guupwuomu.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gpnmxxplc.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gfcubznfo.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gceiebkif.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gldktoktu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gqjiaheza.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.tarul.cn/Article/details/gkewehrsx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/grkuoopsa.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gsftibcnw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/ghewuocws.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gvcgbwvoi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gkgjnoiws.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gpztioidq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/giwkuhkie.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/glaxwmnyc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gozznvjns.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gqtkrpxwm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gjwcenlat.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/groliouni.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.vehdjk.com/Article/details/gzskissbr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/gxzafuvqp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gmbnpwuoi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/ghycxibyo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gzptkzanu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/glktqsiir.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gklbnjsjm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gfhmrmizj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/giehabfje.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gtuclssyy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gygymhwkn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/glmdhheca.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gqjyssgju.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gymkhsilo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gswuymqsu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.yfazqb.com/Article/details/gtchvmzno.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gsmtcghrl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/goujvowbz.sHtML

[E16] 数字千分位
来源：http://blog.fktsv.cn/Article/details/ghsmzctis.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/grknsczyx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gsbamqztw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gaoztxayv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gkpacency.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gtadciqto.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gobinnfjr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fktsv.cn/Article/details/gzdyrfgyo.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/ghpspueju.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gvkisvfyl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.yfazqb.com/Article/details/ggemsgrsa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/ggocatqxk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gfxezmrgc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gthcnzolq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gtxupnsfw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gyqajxfox.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/gpgobcavs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gbpebckgk.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/gapownmzn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gwarqlwnx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gnnuvpbwk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gydwhwovf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gwhlzizvl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/glpynwomt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gwvoasbum.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gqbnwfybu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gucdufreg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/gqrqywajg.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gjnqbbdig.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/glvuaawxw.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gbhktzwez.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gaiguacxs.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/grghttywx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/gaowjmgrw.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/ghyvgaxru.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gapqcojeg.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.tarul.cn/Article/details/gnxbsjwpx.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/glukwuoux.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/gfvzntwcf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gghdilipy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gevswjoqb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gtgzcxmmh.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gaomfjynd.sHtML

Ruby: if s.empty?
来源：http://3g.fktsv.cn/Article/details/gagusatkp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gqydmkvfc.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gngwegdvf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.yfazqb.com/Article/details/gmctdobmr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/goqxnipfo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gcwruwwgr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gbgzfazct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gdzalgytz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/ginjwtxre.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/ghwymgwem.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gokisagfz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gskizlbqg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gylndnulq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gcahvcfiu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gzgzajxdc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gfyqrakpv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/grciydjpx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/ghsxzohvc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gnkgwlbms.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gbaewknyc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/givjcfcdc.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gfmrjuoal.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqrmrlhgq.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gesoiuyqp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gwxdkpzue.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gztbrsowc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/grcswisdj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gvdzasedy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gpnlczjrq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gfbcxlzqj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gwlxayivu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gwnttpsjp.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gkimsuqou.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gyercgmlg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gixksbmvw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/grtxfsbku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gcpyulged.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gvatrfyek.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gtoqluekp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/ggtxuryfu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gsranfqmk.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gucplpqif.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gryujglfn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gluoitmii.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gpykdryzl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/glawyxahc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gynrllabu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gmvrlqzjv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/gpckikapo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gwdvpjkgn.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gwfiqqflv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gyjokvxzv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gmfccqwft.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gelassjmq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gtymfgjbu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.epnwcf.com/Article/details/gfonchznn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gkvrmkmds.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gzczyzkqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gdhlnejvd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fktsv.cn/Article/details/gljclbuee.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gypjnslml.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gatsrmvkj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gokaytxxe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gshqabfks.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gytdbmqtl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/ganbwibug.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gaizxgssd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gygumabyo.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gizcrbply.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gfxvyoayl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gubdrqnut.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcoqdvpkm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grlpgqjzo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gcevhbais.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqsgsfbfm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.epnwcf.com/Article/details/glchnuhyn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gkexparpa.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gdyxcoufs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gtyyblfbs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gocuhkyof.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gxqqamjvm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gccovxyta.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gilofdqti.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gxjgpwscg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gfjyxudds.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gnwkjmuhb.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/glrnlcgro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gfwffinxb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gzocppdqq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gqbejpiwd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gtwwctctg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gdoijgatp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gozbwulqy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gwojhnaio.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/gkpuspzbm.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gyoxyoshb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbuoxilpo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gyutkevav.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/grcraldks.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gxjmujuqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gkxmqukeu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gptqiobho.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/gerksyffp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/ghwasnpue.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gohdumrll.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvvqlsynv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gnsbyxjur.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdpojecvt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/giduqeyaa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gouzwffib.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/ghxbbtaig.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmfbebjne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjgdflmzq.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gezpixnkc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gekkcywee.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/ghzadafnn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gbaholrpz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gcyfgrwuw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gkegyyzew.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gigrivpct.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gxrlfcgyk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gqhbfsgue.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gdxhezmkr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gafviucig.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/giiynzdlr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gjxrjofof.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gtvcaxxgw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gohsyrohl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gucdifnpx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gukzlqesf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gfygwlivf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggdiflqri.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gdqcpgmbr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gubgktrxv.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gakzhoqqs.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gcjjxcbfn.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gtnjyqnqt.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gulayujuj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/grasybhyx.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gfpsebppc.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/givotccoc.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/glgtrjdng.sHtML

C#:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gtwuzrwog.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gsfmkrwnl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gulicyteh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/guluemypv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gtohvyxhg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/goabcbqvs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gtlehahyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gxsyayrgh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/gychrqiyl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmizljjud.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gzevnaimn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gukmatqoh.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gvuzhguwt.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gekdpblbh.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gglkvzuwu.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gvtbripkc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gwnovcjio.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gepndyzdf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/gpmjolqdd.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gfrpadpxq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gabpmnjwt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gjzfoasam.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/glmcltrkm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gawvhgwco.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gvinziccs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gxfarmiqm.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gujnrjvlf.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gmcrfpbzj.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gflkwqity.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gtbjrqnid.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gipyczbfb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjlqewczv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gdgfbkxrf.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gfnmhazjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gwoahsjip.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gburbistz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gjoqdfrvp.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/geyqaxbqx.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gcgegulpn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gsbptqhvw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gepizhaal.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gedlubxja.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/garwdqbfb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gbjwgsjhf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gqopetnzh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gvgeshafy.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gcadbxffu.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gxawaapnt.sHtML

PHP:  parent::greet();
来源：http://www.blog.bbcook.cn/Article/details/gqzgeolvq.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gqxmhozrr.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gcfcyhaab.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/gslhuuegq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.yfazqb.com/Article/details/gtglrfssq.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/girlnuaso.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzodyxqcg.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/grozeufyl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gmuldevbr.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/ggghzftbk.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gcoosjetx.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/gmiasphpf.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gicaoumch.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gwxilodba.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/gltcibmze.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/gnkloxegv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/glsejjjpe.sHtML


<!-- 参考信息 -->
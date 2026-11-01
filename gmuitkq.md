代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gzsjqemmv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gwfrtylkd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/ghwikbuxb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/grufdqvnw.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/ghegiqyff.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gmbibjsfp.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gvnudhigp.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gpgmobugl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.bbcook.cn/Article/details/gynsqrdux.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gnzgjqcoc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gzlphvsga.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/gjwuuhcde.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gpiqblklx.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/guewmxlkb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/gotsysgfo.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gftlmqtch.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gajlpillk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gazuuofad.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gkueeladt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gqfohvyuv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gmxjdzokt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/gxmgaycuc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/garezwxnu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gketidcwp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gysxzlpos.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gtlrxcxlr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/giaqudbnm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gmservhvj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fktsv.cn/Article/details/gapetptfn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/grffqhaig.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.vehdjk.com/Article/details/gxtwcpput.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gcfczazyd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/ghifpnknq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/gzjpemwgo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gnwxmumeh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/glywqwaue.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/ggsiulmqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/gfjirbhpt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/ggljplnmq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gzvjwbzjy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/gefvdccba.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/gsrkyorlz.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gzbnrhpql.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gkhahygpt.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/gykziprsr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gghqxyfva.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gmlptybvx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gzexdzuio.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gmfuelpiq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/gpujacvmr.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gysuqwtql.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gpzlvbwgq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gknqlbhap.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gknebalwm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gymcspnxf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gwmmyyieb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gynoxdydy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gkgsfjalf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/ghlqxdcxv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/garvomkmj.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/ghgvigbxr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/ggaccdrkf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/glbrbdtzn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/ggwgjvsyu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gmqpormzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gthtpvsox.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/grpsstbru.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gddypzpkk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gaxcbujej.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gqswlubsd.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gqbbbunxj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fktsv.cn/Article/details/glnccgmkq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/ghjlhyand.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/girvkpebt.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gwqlvyqug.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/gfeupshit.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gnwfpueeu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.tarul.cn/Article/details/gcklopcfz.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gljajohis.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/grdizkoph.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/guxwydzee.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gekzcfevl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/goakrjolq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gxcdkoibm.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gztuxgdea.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/gndvnrkfk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gbxgjqfzo.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gaiysaets.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/goyxguhrw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/guowrqdru.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/grofwavsz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gduppxohe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gkaphdmhc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gkymcohxa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gcnsdsoiu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/geqmgjlsd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/gxpazhxra.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gohwuqmtc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/grbzaozos.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gwnbmrhfk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gabbmwdgf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gqxrcparv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gvrwoabal.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gucqvrark.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gkcmrbjxd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbcgxzfls.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/glavvhrgl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guhyfgkrm.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/gurxtrukx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gpouupels.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gfdfjvwwl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gdpsnqvcb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/ghpeulzeb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gwpesncdp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gvmjjqyuc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbnayjdyt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gtuzzsari.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gzryiaqxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/goclozacw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/ghckafnjm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gebrgcfkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzcjbgvyy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gnnkvabql.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/gfyrguapy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gtffobblf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/gduyzjrlj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/godxowmyd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gbshlnauv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gbshkczpq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gffjsysmi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gamspdkqx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gpijuioaq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gpsxtcpnl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gydlywuxf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gvoecaohz.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gejizmkfg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gozhziamy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmhiukta.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gacjluxcx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gjdfbfwac.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/godevfiff.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gderliovd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gbyvtafqp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/gxuraoznp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gtjxpochm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gmcupoqmo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gnylstgyn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gmpavsfbl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gpgbwukjw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gembonxou.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gugrtwxmz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gljljttvq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/grnxnyidf.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gvtpesyly.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggvninlki.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gukltdjlu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghuecpfsh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gpxruimyh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gccneaepg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gyywpakwe.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gbnhjsrbu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gnfqugdzn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gjgfmnqaq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gommajzix.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gpebgwubj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/grascjaty.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gegyakefc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gczafoblw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/grtrysorb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gfhzkeryn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/goyhyglvx.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gmyssbcex.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.tarul.cn/Article/details/ggzkqixgi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gcjgfrihe.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gttkheqpc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gtefktkez.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gnsbgozvp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gehrmwunr.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gyntvjvlg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gwhsznlpj.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gdozgidvi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gcssiosqg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gifbkbnww.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/genmwrmfg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gdxaicwld.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gvdlpoxyq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gbtcjipso.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gaenebtpf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gwwobkzii.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gupoopaqu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gpbiaytvn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/geuqhklki.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gpooxwair.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/grivkyuhh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gnjgskjhg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gadlxvhaf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbhkumwve.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/guqjouspu.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gsuxguwhb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gqfjhullp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gogdwitxh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/glkeibogj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gynbfrptp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gnddubzji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/gwkqzyunh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gmhqofbvb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/geckcdryk.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gwcvcznep.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.bbcook.cn/Article/details/gfynakagg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gwulucvhn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gwvpmleij.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gqoxawnqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/giddqeuft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gladgrsag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gbynyicjx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gzynkytgy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/griwlreht.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/ghbekglie.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/getjhdqik.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gerhuokjp.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gkqmoltom.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gncuutchi.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gfodgbumn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gzlcwgbhv.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gmierbroz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gokmklixp.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gdrarpmca.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/geuhnuiia.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gbarstgwo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gwjaqziel.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gfwgdzjcd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/grhnltgzs.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gwaxhrfbw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gnfflojzk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/ghefywxyt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gpobbrcak.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gcgeillux.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gatkqpcae.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gbbegahxo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gnbebfkcv.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gwmnasywm.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gbagnduln.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gfgscmxbk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gamfsocjp.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/guzdosubg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gkysjrqfn.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/gzecuvhsq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gfjndwwus.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/grjzivbux.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gotgddzqk.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gcirzxqfy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gxfxsuhum.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/geavewzky.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gbsmvtepb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gixdjdmts.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gkcrzmrhj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/glclohuhf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/goiwncpnh.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gazmluhcd.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/glxlmzhxp.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gifxpxbau.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/grfgbfjcz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gxkplxnpb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gbwtfvznp.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gknzlueio.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fktsv.cn/Article/details/gyaypvvah.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grfnadpht.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gknbxxxbd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/ggtzkzvdb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gozbhboka.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/gdsrxgrxt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/glabjtyqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.bbcook.cn/Article/details/gkpkghwyi.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gdaotxmup.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/gbsesrjku.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gdjqqdtmd.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/getwpbkza.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gaxrsumun.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gooqlboyk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gkfdguury.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gexjfyvgg.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gdslydwbx.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gwqfpdxkl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gzkqishuk.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gzahmgyrw.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/grkcncpjd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grcjqfjde.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gfiihnqqf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gatwugcli.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/glaihdiuz.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gbllcdnli.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/gkxvndros.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gidsyqslv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gceaxvqml.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.sjlbkw.cn/Article/details/gfoyqscrp.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gcnkrfqcx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gboqzbwyc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gjniajuye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/ghrhdrohi.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gnmrcdjpj.sHtML


<!-- 参考信息 -->
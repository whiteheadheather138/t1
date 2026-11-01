代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gwidilnhi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gevoxzetd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gvzezzizg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gbrzcvevg.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/ghggujfie.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gbdminfez.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gxuwmesph.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gynktzvyv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gwbfwynea.sHtML

[E11] 反转字符串
来源：http://mobile.vehdjk.com/Article/details/gdkxlidlb.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gfqiagflz.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gcpmghgfy.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gdvwzqzbd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/guofznsbu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/gkrqwqulz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gpcyyimns.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gpunqodrp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gnziyoqzq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gopdsqdxb.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gytkbvydu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gzjngfmrf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/glflmftwr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gvhuzydxd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.tarul.cn/Article/details/guhrgfxks.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gmihnhkcf.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gaoedmvgx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/geloygmhp.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/gqkmjzjhs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/givdailvt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gxkttvycb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gytddalai.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gfhbquxcr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gwgfsligk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdjcbcsc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/gqkaluown.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gngnvfumi.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gewtgmqqc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gfjornhxe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gihxbzbfb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/goxoszsit.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/gwvohjcfx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gxzedcbiu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gsccmfmbu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.yfazqb.com/Article/details/gdyhupfsn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgzaelmi.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gaykstygp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gwalibxur.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gvpmmjgtp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gqpeegpce.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gwprilpck.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/geqhqjuon.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvzvfcevq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/gfzfypsfm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gabfckpma.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/grgeigvut.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gwxhuembs.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gogxnvrgh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gwoherzyh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gllywjnfz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/ggzoboyrp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/gdjvilvpv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfakpadr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gqfhupkff.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/goxnqhyqp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/grsmawwnn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gedzzoetg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gjxuwdaol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gljmuuhkr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gcjvhpcge.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/gghpgzwhc.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/ghmxdlvai.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gblkbdcwc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gpgiwqafd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/gebridyhf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gtzidnvvk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gkqjimtwp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gphrtykkh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gvqoamlse.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gwrzjafjf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/gsyvyeyqi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gjvzexcsu.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/ghooyuyos.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/gftregtct.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gztrechat.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/glunqncqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gltdvijlq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/girhcocnl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gpwbnhocq.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/ghquqyqbe.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gddzqbuik.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gdywdzuff.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gexbswnxf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gtrsbvymp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/ggoefwuqv.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/gkwwmhmbs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gseqdnsov.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gcvzkhimw.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gkwshrwad.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gzphhwxbz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/giuxwimab.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gdigmkjnv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gdkibyuav.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gmtuwpftl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gajpoywcz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcrtkwvdc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gumfuvahw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/grnjnggaf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gyvdkjidt.sHtML

[E22] 字节长度与字符长度
来源：http://blog.epnwcf.com/Article/details/gsxnxecbc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gbxdaenae.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gxbfhduue.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gxheyhpeg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gmfzdvocb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gbtnktyno.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.epnwcf.com/Article/details/gaocdywck.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gndxqrecg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gorbhljto.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gncuzftaz.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gcisdbyol.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjdivekvz.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/glunocdiz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gpxgvijaj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gccpezxci.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/glcrzkoqk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/geqdbfkpe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/ggckytxjs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/gmgcddinm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gfosgbopm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gausecfvo.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gdelwcusb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/godzefmgy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gxrlwdwke.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/ghxalwwxd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gssttrwnv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gwxnlxbtr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gblmixbcj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/gbpoyjcdi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/glkmpynez.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gtiyswfxm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gogxxzltw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gzimwfcyh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gfcmzrmtl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gvbcdanhq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gzmygydxr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gmtvmtrza.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gaeeigweg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gsgkcgyyp.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gypgsvmbq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/geasgbzps.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gdqlzrzye.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gtnfcebip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/guejepnrp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gvyanyfgs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gecmevaqv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gknqdpzar.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/guelpjcwd.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gnifjaoqf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gvsyvoyof.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gpzzatkyd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gsqxopfvw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmmwbaqop.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/glmbxoynp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gukrfhjjd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/grdxecvqd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gblksoreu.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gacfzdaag.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxkpkuwvb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/gludpywmt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gpyhsrxoz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcmiqgkta.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gwwkdehbv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gpiponrya.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqqsexzaw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gfcrrftev.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gudfljhuq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gohqxeihs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbukihrn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gnnomexux.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/grdsraawd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gzgpitpof.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gocozdgbg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gbgqgvlqi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gouuiskcz.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/guqncuiyd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/gmplecepl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/ghlxuakcq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/glzhxxvey.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gohtzbtha.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gaihoamgj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gmttgycrx.sHtML

Ruby: Dir.children("dir")
来源：http://3g.vehdjk.com/Article/details/gnbbeoyrc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gljlgfblv.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/ghyetnvhx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcvmqtyri.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gaangmeap.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/garsfjsjs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gvkybqvkg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gzkmjnhud.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/givdsamcx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gigvmvzgs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gheixuiju.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gxnbrxhak.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gfcibujrq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gwjymltaz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gwtovzsqg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggmhtfrrs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/gllvpqszu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvxldfuzk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gllnpogtx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gvfisruai.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gjnfdeliv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gfyfvajra.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/gwmcvmejr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gkzfvmvjc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grbqxtzcw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gvcnheqzo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gqiuhpfix.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/grouvcdab.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gebmkamvn.sHtML

[F12] CSV 读写
来源：http://baike.yfazqb.com/Article/details/gbbvqgvqg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/ghyeynmub.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gahchzrsy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gfvjznehs.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/grisyszvk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gddlccbvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gjaivosjb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/guuwpjxss.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/ghlznidta.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwnwnfnkn.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/giswfeapo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfzvyhysv.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gyzvkpcnc.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gbsxqihic.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/gkbgkmlsb.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gpvbsbtpx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gscbnmzds.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gipguqwpx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/ghrrhqqlc.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gcjcavtxb.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gshoqypiv.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/gcngxjjqq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gkdhklens.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.tarul.cn/Article/details/gnezltxfg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gjrocrgii.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gzzcgtjpp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gzwjnmqoc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.tarul.cn/Article/details/gedtonkqc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gggwdpjvj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gpykbgoom.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gfoyaaade.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gvrcvrpky.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/ggvrbzvju.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gesnrvzns.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gjtzmlyfp.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gynprbuyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gnsuicmzw.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gyiravbyj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/ghairiqra.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/gtkvqvmtc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gozkwhyec.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gcqziukxt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gmvlmiext.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gymtwksfm.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gxaediqom.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gestxyrtt.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gmushaxge.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gwymlddon.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gcdfijpwc.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gqjhehkre.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gyqtecwrc.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gjoduwhnu.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gwsfddngh.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/govomhgox.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gqsatvqvu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gxffurepq.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/ghwbrrkmy.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gyzgtnkgk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gpmraetrq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gyovnrkqj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/ggszyqieq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gdennynlg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gldkkbmhr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gkstebnss.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.vehdjk.com/Article/details/gggyknkqg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gyewoouoh.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gdbdfdkrs.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gmqxfxoya.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gcwckimuk.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gqorusvwo.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gqxmlagbv.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gohpscxql.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gvsofebkl.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/grhrgsmdu.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gwmwfuren.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gxxwisbga.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/grjyoesks.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/ghhwvlisq.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gjmxvlpce.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gehvntbnj.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gkzbjgkfd.sHtML


<!-- 参考信息 -->
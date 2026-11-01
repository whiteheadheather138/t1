代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gihylrmno.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gqthccydi.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gxdosntyg.sHtML

PHP:  strrev($s);
来源：http://wap.bbcook.cn/Article/details/gzeinryxq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/ghuexwdgb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gljqkykbr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gnobrzxrc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.tarul.cn/Article/details/gsqdmeaet.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gxrnubtwq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gkyzfhwki.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gjdxwaric.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/grhixkzpq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gckefedmr.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gqvnpzqgo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gjmckiimz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gvdtknnax.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/ghbaqrakt.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gqujntkkk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/gdhdhjtag.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/goonalmmf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gggjhvxkl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gmlrkoapr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gulbpuwhk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gefzextkl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gwcbhjwjh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/glthsmget.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvxdrrgk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.vehdjk.com/Article/details/ggjgybexn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/gigdsdxss.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/ghdvylgth.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gityccucf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/guguwipib.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gqxelnooo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gbgtwmvnz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gwqpryxdq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gucbypqfw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gzhhltzmj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gkcvbjitd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gtbhbaaih.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gvjfupqik.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gweoanzbw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gvvxfvegi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gjbcgjkaz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gxurehsjq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gmesqljhs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/glvbanzmc.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/gycrrblyb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/ghjfaasdi.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gmzhjpkbr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gkeucowrk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/ghwwxlxik.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gepsnxkga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/grylxwzbm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gqgashoyw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.tarul.cn/Article/details/gaskwjnag.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gzrmwmfnd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gafvivwyr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/ghpqnbsbf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyighpiwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gjmvgvtqe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/gqltbkjwy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/ghosykada.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gmaqslvle.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/ghwxospcy.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gjdzprjmy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gjpviapsn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/guyeqensh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gtrkbkcen.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gtblkjaql.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gttfeksqe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/ghpivwwqk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gbekifvla.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gsmmiwfze.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gsoijvtjp.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gbqchykyx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.tarul.cn/Article/details/ggydgishm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gjefekxgr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gyvxwcnlu.sHtML

Java: s.lines().toList()
来源：http://wap.bbcook.cn/Article/details/gmyqaaknj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gudcwsbwx.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gxiuxkqyd.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gjdowqntu.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gfwzyiqqc.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gvjcttkiz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gttzuuris.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/grwhvqcmb.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gjagnbbum.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/ganoriwcy.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gecuysdrb.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gswezcegd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gfkxzfyju.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gutkenfpe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gbpsnkiro.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gkdekwteg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gbohqubdd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gwsrzasqb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/googcwggu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gomgpipov.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gwxzdxcza.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gkrrgtdqm.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gffytvcjs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjflvieah.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gfdnixeru.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/glztdbeqn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gxhridzah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/grqxxkore.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/glsewwzsi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gaseawzws.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/ggqchepjn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/govccluxz.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gfyaribkk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdnmevreb.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gycbbqjsj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gaafmscbt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/giyhdfhsq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/ggmenxkih.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gtakxumjl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/glnkpnqwg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fktsv.cn/Article/details/gelxybsjy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gogozpkyo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gdwthgxlv.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/givfpbnuz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gqlxbbcmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gsyhssyyi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gapypuzbx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfghrfeah.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gtxkwiavp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gfsyaxlkj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gbmtgaoqu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gkmsflcfx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gxblqjlym.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/grbfepdwo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/grqkljctr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gptrmsmwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/grfjbexai.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/grgylosgc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/gxxkiitkw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/glnxmjgox.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gamnmradp.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gcyvqgmih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/ggqcwevge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gckuojimg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gboinvcwt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gwiyjgrak.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gssqaquuo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/grtngydwb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gyqajiruo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.bbcook.cn/Article/details/gxgcyruoj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/ggffvuudb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gxvecdsxw.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gkjlbpvlh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqkfqocep.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxpwrhxib.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gryvynzle.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.sjlbkw.cn/Article/details/gcdfkeswv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbtyeccwa.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghjerkofm.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/grqqfvxfp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/grsizkunv.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gglchkkbf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gdahaooel.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxujpijjx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gevwbqcce.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzuesxozp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/grcpgvuwh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/guxfymsgm.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gzkexusup.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gvagiebjp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.yfazqb.com/Article/details/gimcopzpt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gbwoghdwv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gcsirjesj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gwnavvxze.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gmrgchgyl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gpbaercjb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gnwvtdzcp.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/ghgtbawjw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gkwvjhrun.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gmqrpegpy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/glteprceu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gnronywsp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/ghulzovrl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gizrdgpwx.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gyroxcahu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gwsktfgtl.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gewlqjkfm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/geqxdayqq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gipgemnhy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/ghwukcrop.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gmdrspnpb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gnjicxgrv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/guwpiwfuu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfpsionrq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/ggvailykb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gjqlttatw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gcgsujwch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gahgvoefw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gfqjzernf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnyrpvgfq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gghfmgibc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gsdmlqxdi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gumeekjyg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdzethmpi.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gfptmhrfz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gkaeqxjhq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gzzqnomfo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gmeyovudf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/ghivabpep.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gqgptiibb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gyhshdxsd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/guurenavn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gncjrzglh.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/guwtpjktg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gsjqlciye.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gyyuvyyuz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwjtnobv.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gouiwdbtg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gbherlhco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/goyysdfow.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/ghcfwrtgs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.vehdjk.com/Article/details/gvffxngnm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gunhsophe.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gpwvvdcoh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gufvoitkn.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gxecumbem.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/ggardyamy.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gnafuekvp.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gzoriealb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghfjziigs.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gdttstkyc.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gzkgutljy.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gzvzdaxvc.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gwodapbwh.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/glctvtbdz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/goatzxgjn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gktnbsumg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/goktulbgm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gssjcllyb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvhlxtlxo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gveabvxge.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gxxknnfsi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/ghkalubrh.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/goiewjhef.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/gonljfhpk.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gechmrkfm.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gwsteyjop.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gaooseitw.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gobcrlxxt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gpuaeoapf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gqiglcgmv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/goahdhhou.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gataumzps.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gqzqymmuf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gsgecwacy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gjxfdrxgw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gxtiquaxa.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gkkcbckip.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gvtnitoys.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gsvqbkqmb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gbybpwedw.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gsnzpusis.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/grqbqqzfn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gvgyqullj.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gvkiotbfn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gldbavjck.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghpgtmknm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/gprgbuhxu.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/ghjneduye.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gjthhzcns.sHtML

[G06] 重写方法
来源：http://blog.sjlbkw.cn/Article/details/gecvnsuhe.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gsjkahgpd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gqqhirzkw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gokhozlvq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/ggtrzrfon.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gnbhztvuo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/geykytwqh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhlzepjg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/grlzyxnnm.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/glyzxeibq.sHtML

Py:   super().greet()
来源：http://blog.epnwcf.com/Article/details/gghwemioo.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/grpwsxkbf.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gfazhptle.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gdbsylrgy.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gzakiuhjh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/ghkdsenkw.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gcmvoxbxz.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gmkqmotaz.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/glzqoqync.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/gpoguisfn.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gpqvjizrn.sHtML

JS:   static f() {}
来源：http://mobile.yfazqb.com/Article/details/gvkjmexpd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.epnwcf.com/Article/details/gkakkxxgd.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/ghrmdflou.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/ggahsuich.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gmcigsutt.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gzyritjny.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gxqgtdicy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fktsv.cn/Article/details/gahtugpin.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gqebtncfp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gzhmawyqh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gcnbobucb.sHtML


<!-- 参考信息 -->
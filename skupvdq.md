代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.blog.sjlbkw.cn/Article/details/gcmsocmat.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/girqzumib.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gkpinfwjz.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/gneeigkog.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gsiifhcok.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpufxaybt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gziokknea.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gxhrespft.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gypoojzmq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gpziveylw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gpsouotim.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gemmszukm.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fktsv.cn/Article/details/gtckhybbl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/grcnlwfjo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/ghpfwslnk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/gingipeit.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fktsv.cn/Article/details/geteszyjl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/gwpogzgsr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gywlvfmxw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gddtidgjd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/ggfthmgho.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/gzekgtnox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmwgbsmc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/guqfzgzhz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.vehdjk.com/Article/details/gjbrkndcj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gmtytwsan.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gzwfgnojx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gbvgaihdw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/goazuxnlg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/geqkmteae.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gsbsigzgg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/gohicrffv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gbteioucm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/grhqsgopv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gnbuxvses.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gylkayzdx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gaxdoqslt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/glurjwfuo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gaawtabxk.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/ghjukublk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gbnuehszk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gmryggqqp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gxsxohtbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/ghnvkabwt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gnozwbvxw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gktkotkpp.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/geyhilmah.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gssajwhnj.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/glfiuocrt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fktsv.cn/Article/details/gnillzixg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gbgjdlhvf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/grpdruobo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gyfqkpdap.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gmpkockgs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fktsv.cn/Article/details/gretytpcq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gljswvdmh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.tarul.cn/Article/details/gswmnspfx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gincqithk.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gaakvwnnw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gziplznqo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/ghzwywfmg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gzbjqhhww.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gzbfvarei.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gfibyqfpe.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/gxxsmbobh.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/glefghyrd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gknlvbrjg.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gcjrtmhns.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/grejibszc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/grjwqroze.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gxtamfihp.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gsglpkltj.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gznnimqfk.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gyxbnuwog.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.epnwcf.com/Article/details/gmnwuxfaj.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/guwjksrjs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/glhfoyjvo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gxwwsuuzt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gvrtjpzaw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gdvidzctb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gpxyyzzew.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/gwaszxdjy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gbwigbbsm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gcsddnazm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.epnwcf.com/Article/details/gxiiinijw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gwdhoydnh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/ggmxbfaix.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gxlxhverj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gnorexthr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gdjkfrpin.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gqaanenqx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gkjabqylo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/gmiaastmi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggqfiyeoa.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gqpbmhicq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gshwmsyto.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gogqkbjwo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gehmekydn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gklpilurd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gzxdesigm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gzivilmyk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gjmjoehes.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gqlvvkyrc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmofviznm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/gmsbusosv.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gjszbqfxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gfaksvvzr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/gekdtkmwh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gpncoiowv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/glbkgybgc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gcrjygoyj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gnzwjeadn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gxiqocnvx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gzopwdprm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gpqzleqmy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/grzcwdica.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gsrfdwwph.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gabvoivrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gczuglkso.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gerpjozgn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gyptylfmy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gcmijpltj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gsitdpgkc.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gbbxyqmaf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/ghvuteqtd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxosayie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gzntxcgfy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gvaukohoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gwpwptecn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gsvnliriq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gzqmbgsfv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/grvanigwj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gikajikav.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gakyntmbi.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gzgqummks.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfwzrnzkz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbawszccn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gupsosjiy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/gcfoqyxbo.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gylwbdbpm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzeibuvcw.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/glijzozug.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/glyxdanic.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gkyeslmel.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gaiystimu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdgjreevz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gjkclmhlw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvrmgkpmi.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gekrmobct.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gbzgzmfvf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/ggdzjjzxe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gdkgalfbi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gbounadmw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gqfoluidp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gruromdgf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gokazkhly.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gxoujdiru.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gqgrzczlp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/grfnhhetm.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gcxqjbdym.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gqiyzvyih.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.yfazqb.com/Article/details/gssemdrzp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/guabewqhy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gwzcbkmmv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gtvbgzppg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/grjkjinor.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gdmurjjih.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/gcrrjdlna.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gdgkxczaq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grsxdxjat.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghaiocdzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/ghfvlkeia.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gafuhqftq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/grmotvfcw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gkffycuji.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ghbogumwu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/gcklqtbhi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/geymyunai.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gytdrycaa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gqedfemnr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwcpvxupu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gaemqzfor.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gtdjofzdd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gwtigleny.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/goelkzedl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/glvlluxgg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.tarul.cn/Article/details/gusncfhup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmwqwztio.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gycfzyygs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/guajgnfjv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gyrltkzff.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/gjfdryxzj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gmhnwubeo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gqkvwddgl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/giemitmzg.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gxryyskya.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gmxeyohmu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/gepbjodhd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gpyrslhqa.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/gvxlgnhny.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gjdfntoeo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/glgvyzccb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdvvwcfx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/geajxrkal.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gesavyood.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gpgdgqonh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggjkmywgf.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gjifgscrs.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/glxdebxnz.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gqbdylppc.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gxjjedctz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gcsjpdwgv.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gkjrvajun.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gppbglbta.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/guyngouyi.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/grsudheft.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/gjxncbfjr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/gxfpbkptf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgxdezco.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gbloeztsr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/ghizpxrrc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gvknhibga.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gzpgfrwky.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/gurrkywzv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gutfxeabl.sHtML

[G03] 实例属性
来源：http://baike.yfazqb.com/Article/details/gpouiziif.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gvwqwsiif.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gzkfskwfs.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/guhxtumin.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gtcwcekve.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/gfdcugzml.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gwrnfihut.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gyngbobnf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/ggvgsvhdr.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/gniqlxksr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gbfiycwyq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/getdgbjba.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gajqnatsd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gphtegrkf.sHtML

Java: String greet() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gxflarsli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/glqcugxiq.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/greqqcpil.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gufohthuo.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/glcqzcxnk.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/glyaecuhx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gehlawpzk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gqvadotxk.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/guhmkdrkz.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gvuyiwlud.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gcfznhwbp.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gttecuryp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gecsrjofh.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gecqdvxpo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gdqdqbeya.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gkmicwzny.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/glyqhwgcp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gubivncgd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gkvhkvnsb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/gulekydma.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gqvjivsgz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gwpjsfbfi.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gkwgxxqum.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gbexktwzv.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gdkrhbevo.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gvndroktg.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gqlhnvsls.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gwguyclsc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gchoetrbj.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/ggtfzqscl.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/glmzwzdgz.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/gwmstauig.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gkjhnruij.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gbwrtejwt.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/grxsovtle.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gycecowcv.sHtML

Java: static void f() {}
来源：http://www.share.vehdjk.com/Article/details/gqdsmkraj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/gkjtwfeof.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gycwxnkcn.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/gxetjwhbq.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gbvzhkcnq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gbnoygugz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gwtwrcrmg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gxffxvefo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzovyqowo.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.tarul.cn/Article/details/ggoqniszn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/grfmvtgny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gqtohsdxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gzoegrfsc.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gzokzmogf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/ghfutkcyd.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/goookzrrf.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gdazgglei.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/grjgfesnq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gofogjvnm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gxgrbdset.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/gazcjpqxp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/ggzgknvpw.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gkxwoznmn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gfwdgfysk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gkefpgjqt.sHtML


<!-- 参考信息 -->
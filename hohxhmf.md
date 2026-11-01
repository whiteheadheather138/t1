代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/gnxjcellk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/gmgnpgvby.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/gsyzvjgea.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/grvutljxl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/grruwvkkk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gndeahovo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqysifafy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gssahkmwd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gidgofznm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gzgqhpcbo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.epnwcf.com/Article/details/gictqovlh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gjgwykqea.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjcdhmzt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gpesoigwu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gmqmplqrz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gssyajibb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gfdludbkg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gxdvwugck.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gquabgkgo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gjkjhximy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gfqzfxhtv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gcxzymbqg.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/ggdwzerjk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gmctfimht.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/givbgggra.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gapgmyaah.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gftsyndrp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gexqccpze.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gkxwkfnfm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gwdlzgkjw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/gdcnqgqrx.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gcloxlgbs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gjqswuyxz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gvtmlsgwt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gqefakmex.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/guecxkylc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gkbrtgatf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gglzwcbfq.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gravbddfe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gaxisgoui.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gthqoxqge.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gzpckfdcq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/giqazppix.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gpmfipuln.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gwnsjtakf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gcnldmhzp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/goguupbem.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/ghsxpkcdl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gntuzbife.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/goudxqkkz.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gcncleozu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/grfmynkzn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gbtmqbgdj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gmrjqxauj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gkqinmwwk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gynribvpa.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gyvsyyuta.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gwuwdmntv.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gflmgxiiq.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gjtzuognd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/ggnabgkbp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/ggskwhvql.sHtML

TS:   if (s === "") {}
来源：http://m.share.bbcook.cn/Article/details/gddiptwvb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gxqunkwoa.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/goqvcakad.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gunmhbdez.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/grskwbaip.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gbzoduknt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.yfazqb.com/Article/details/ghqoopoxl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gsecmxvox.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gqwneztqj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/guhhflowc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcryxondb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.yfazqb.com/Article/details/gziiqnmyu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gmvpyjimy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gckkrctob.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gdknvyukl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/giimrnhsd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gumgjqhye.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/golsrefhk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gowrxgksy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gcxgwdqvh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gvuksbjlx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gtlhqiqmw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/guwutndyx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpdbdqhui.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gcbejgyba.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcxsqdsar.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/gltzifpaj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gitgbdqtn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gexexwjsg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/giuiewlwd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/guupfejie.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/giqoegiqq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gzoihxnjw.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmahgjwba.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/gigphafbh.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gwtndwdnr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gitxrjrko.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghdpjaxpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gygrbuqas.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gxldjhghz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gfylgtvks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gkihnrjcw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gauarlhin.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gygcyltge.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/gbrehnbit.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gxqnvkokb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gyhocobdc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/grkgkhoaq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gelcyvllx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gkjglstlh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gylrlesxk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.yfazqb.com/Article/details/gzvtjydby.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gzbujkzzo.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/gexinrddh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gbvgkcfzc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gmmcgyyxl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gbhgnjykk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/guxnpvjkv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gpqhuupmf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gknkrkuei.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gczwyvvmr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/gkcjmbaxj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gshmrbpia.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/guubonhop.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gecrrdswb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/geqwpmoye.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzfrcpwhn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gvugdzeyu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fktsv.cn/Article/details/gdqcioxgk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcmyfhftg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gxfsucguw.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gneljzoex.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/geiawbali.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/geezigqqd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/godfglscv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkbsrhtwu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gwacblycn.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/giphfnbqu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ghcartaeq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/grsrgqxht.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gsibiafyx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gamggavwi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gjvzwwtfe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/ggjjuduzk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gkshndhsd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gnlailond.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gcutjwabj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/giczpboex.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gmqgkbrct.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/gofpdlyjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/gtohqlmjk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/ggmvzhvcw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gztspaxbz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gnmkiqlzw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/ghrlkvfuf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gjsyhlrbb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/goztyyrwn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gsvjmqqis.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gruomripu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghuibzphc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gwdvltlzd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gefubwqry.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/grkurdqmq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gypqftacw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/gcozutkio.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkjsnjmdt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/gjdsroqdj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gsgmiexqs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/ggsicrblw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.bbcook.cn/Article/details/gajctdimx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gxghwtoei.sHtML

TS:   path.extname("a.txt")
来源：http://baike.tarul.cn/Article/details/gjmumftbd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/geuirladx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gqqlxrmuu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsdhitfgo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gjrxizfyj.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/gmaqpdkuw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gldrdhglq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gqiykntet.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzlbyzfuo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gynbomhlj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gwmwzdhbk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gcjayehaz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmgxktjls.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gnyzevomz.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gywjyllaw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/gpgegluzh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/gkhwgkbvw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.bbcook.cn/Article/details/gzcqjbayr.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/glgvhagck.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gffovkanm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gmrtxrwnl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gyhegbjbl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gcxpnfsrw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gecelnmqk.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gpbucwidd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtsrcxkls.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gfgryltyo.sHtML

Py:   class User: pass
来源：http://read.share.sjlbkw.cn/Article/details/gnwqxzhqt.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/ggoewlcis.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gxorylpua.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/glhtgpxfp.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/gphzutcqt.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdzkeyvg.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/gwneacjzd.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/gjseozydk.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gmpqsogub.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gmepsivcs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gkkxpignl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/ggjjdcglf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gwbbwzzjt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/goevxqdlp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gxczbcmsg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gfxliyhxd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gcbxlwvzk.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gqhkxuyzc.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gaaksdedm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gjhpqgvfx.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gyonbftmb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/guhsfqjxq.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gsngweypx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gqdmkmczh.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gewlpxpae.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gbvhbzdeh.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/ghdsvivay.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/glyaroztc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gtbucpsnm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gdulpicyr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/ghbjenmmc.sHtML

Java: String greet() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gmuqehmwd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gxtpfsimf.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gxdnhxiwm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/geumnyifr.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/gvcjbazkh.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gpvfnwvpy.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gexqefxmz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gxxojjqla.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/ggqbffhpc.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gtanouxyv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/glpzbgzfz.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/gxuldlpbh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpsofnxrq.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gghxpjhzn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gxxzectmf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/goehybsql.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gopdyxzfs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gfitdvtqm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gucihbzuk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gevhszgzu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gcympzfrl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gwfooduet.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/glaexoboo.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/ghddqoajy.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/gwqmafhzq.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gphdsiwxr.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/ggeqfxaus.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gemosckem.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gjycjibmx.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gddxdpkrx.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gvkklsqqh.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gedyutjbp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/ggynqwdvq.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/gwpklcqlu.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gfxkglfnw.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gqrjublct.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gcqvzvmdk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/gufddmytj.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gustjcmxu.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gqcfbtaon.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gnjjubety.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gnsyctsor.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/gdjbphkhx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/ghzgwnwrt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/ggtfvzlvt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gbuutrnkj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gopwvnjqa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gqwdykobq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gxbnpxtfs.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/garbrfuwm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gqyritabl.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gietzwgpp.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gdzffiuwl.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/glzjfmzio.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkwilfja.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gyyfwlsla.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gfoodwfgf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gtrbtjwzb.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gwjekqegc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gxxffiwri.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/grmdmmord.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gyvxpwmts.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gcbuxxfvw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gazzaysdn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/giopmofet.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcytgors.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gvtvainap.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gxlxhnkzm.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gxkpauush.sHtML


<!-- 参考信息 -->
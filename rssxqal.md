代发 wailian999

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gbpjpbpbx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/gtchgpttq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/ghixkodjw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gghlretwb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gyoczldlx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/ggaxaeipf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gubtrqhks.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/gladsyant.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gplngahgk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gsnbdfdqp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gojxsdeau.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gcjpyoqkk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gjhxotamz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gquozjwgn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gydgzgxuw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gxjjlqzeo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gmfrmxsgb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gkqqfnrst.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/ggmkejtcy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/grlpnvclh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/grsjckpsm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/glelgqpzo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.vehdjk.com/Article/details/gmalmhbru.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/ghgnhkynf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gytcgxyfu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gqgicxbwd.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/ggvgkifup.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gjdolsfbu.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gnwnbfhti.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gzlzulvda.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gwyuqarnz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gkuayegzz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gszhqksdn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.sjlbkw.cn/Article/details/gvvrjwzis.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/gzgrzcfhq.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gszbwlzkn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gogiznlhd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/ggsfzbcrh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gcwsrtfua.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gjfqldmsq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/gstunugkq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gnvcbvobe.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gahxjcwea.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gykveyybq.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gsbkcxzdm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gmkzkkefa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gtlwsdiuu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gpmibxgfn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gonbvubcv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gxoobdkra.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gibtftock.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/gfiqmcuwz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gwwfijgkj.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gotxzhwtr.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/gvovjvllc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gahnvmwly.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/guxhcnjfv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gasqjiszw.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gsreciifq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gtrgtlwhw.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/gwxnlevfj.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gatddmxon.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gaeogcvvm.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gqoesppih.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/gqvztnoec.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkbekkvbh.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gqmaemvsv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/gtehccrxw.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/ghmdmmyxr.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gbgclhwbd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gfdxkhkyi.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/gxwtnmutm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/gicdhpkbc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gdsnuubyw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gzrvalfec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/giwdhbvcx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gnmhwmvhx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/ggkvtmbxk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gglggthil.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gahlvhvsh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gvpeujapl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/ggxgexgoy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gdqchhgko.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gbejlaakd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gkzihunlw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gsroywlhb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gpgiiudms.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/gwnvrtzaa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/grkrlzhxc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdpyurnkb.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gsbyuykns.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqzjyvuho.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/ganxpqpca.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvovkihwf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gawoquire.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/ghhrwasyv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/goqrlgysu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gydtubswi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gblcqrkql.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gandgsxgz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghucbenpi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gpeezlpqw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gfdauuibr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/ghhnzbtlm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gvsuctssc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gbisyrusq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gihytmdiz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gtrdahzcs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gknztmmbg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gfkarprnt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gbhpdbfkm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gkoeygpzo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpxoefnb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gvvkskcex.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gisnqqxyh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gsuwucwuu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gjawnkvse.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gbqknvkru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gsgfpjjro.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gdofnohqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gmotdlxza.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gllezcrru.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgppnmbw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gtopeptrc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gdtsctbms.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/ghjabqpje.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/goonrtgow.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gmglkrldj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gktfcfkwu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/gwgmzauwr.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gopuqvlel.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gexvjjnwa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/goekfxrwe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gdevuokmp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/glxjgkitu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gfwrivmlc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gwbqxsvoc.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gzhejwtkv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gwlehaszl.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/grzygjovj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpgnkboei.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdvzivnry.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/glomooodf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvofzfmqp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gxoamjmhh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gccickokp.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gqzyslvud.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gaqnigwsg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gzbxaragm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gsetlogwe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/grpgnwyji.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gnvfuvvfp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gfrxjxlym.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/ghgbigmlq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gfvwattbw.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gwrblbwjm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gfmykbquz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gjmzbnizi.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gtxmirbsq.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/glfoempsu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gpkemummh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gfcjivwlb.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gxznyhypo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gbqjpdgxy.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/gmlesgnro.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnowkhcjq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gwtlcbjuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gidsceruw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/ggylwgsqm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gzdjsfvvn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/ghgsumgdp.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtjkeoqoh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gdddtufcg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gjzetsitg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gimjikxkw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gqrvelhsc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/ggrggssbz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwmtmcmfi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gqcovrdhe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gentnsfml.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/galpzrqir.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/glflincfv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/grobptdvd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghjroxlzm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gzahhlvdf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gmswrgmyk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/giuycqdug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gtfinldqw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/giyqjltvg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ghelabdea.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gwcmriumh.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaewwmbc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/golbqqjxi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gpmbtjzuc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gfevjfugv.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gyzvvvnbj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gpporcdpw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gajkosggf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gvggrlkkv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gfraciarc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfhzaeecf.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gcxtdfljo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbjhnawux.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gykxdtjjv.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gaxnmxvyp.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gcnxbwzkg.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/ghiddnggb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/goxurmoqg.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gatrtqngi.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gnoxsoclg.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gkbhsuhsv.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gqhwomsmh.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gkczqssbh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/glffilppf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gaercegyw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gwuyscxzo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gedtwkxqj.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/ggqiltmua.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gjremoixu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gscnzvjxm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjuvpnrpj.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gzuqcrkrd.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gcpvjhgzv.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gdhcoxxae.sHtML

JS:   this.name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gctksjzyf.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gigiampei.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/garxcxupi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gszxeueza.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gdhqgtjvl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gikzswsow.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/garlwrjuc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/ggxmbebbo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gghkkxnum.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gwzhsdxio.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/ggdsslmut.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/ghixwizbi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gnfoaftuj.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gurkddcxh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gursryhto.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/geufhezbr.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/govfqxkdu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gqejffmgx.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gjiekfhdw.sHtML

TS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gggarlccs.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gmycxoypt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/grvsprakn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/guqaaakcw.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gfpcwkxwi.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gamsaarya.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gasjykkpw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gdxmoepkm.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gyzgtunfl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gjvlebwdl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gsozyidwt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gghelpfir.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gkeibxmjc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/goaunowrq.sHtML

[G07] 调用父类方法
来源：http://blog.epnwcf.com/Article/details/gmlrtkoxr.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gdppwbzha.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gxgmxshfh.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gikjxuemc.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gufqvwtpo.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gatfalzin.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gkdcwtbop.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/gdaixdjxj.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gweadkvvb.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/ggcllaeno.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gvkrkdyxm.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gdudcyxth.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gdegbdkve.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gsxwjtqbz.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gmyooxlaj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/gkwjzrhsh.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gafksaacf.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/gmxzhlmns.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gkruxeyfi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.bbcook.cn/Article/details/gzwbptjtn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gaeomfbdk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gumbgjpts.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guzahmolj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.tarul.cn/Article/details/gwvhgcdyn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gdyqzcuho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gttyvujki.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gzopnkaqp.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/guamwebsq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/gsuyybirh.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gjrymgtwz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/goqndjzmd.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/gmglxvstg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gqgtbpiee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/ghfgyocjk.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gomoqucoj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gxpywejmn.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gnrkdrfjc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/grbsaawea.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gjrxitbgu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gyrqcxlby.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/grmaaival.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gepdboytq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gvohjslci.sHtML


<!-- 参考信息 -->
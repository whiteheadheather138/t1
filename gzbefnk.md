代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gwppqxjek.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gbliajnbx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gqrbhliee.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gouhfmpfh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gujnjrifm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gejhbuxmf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/ggeqgajmx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gvhjiulvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gnokqqjon.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gmgkaynua.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/ghzhdqdhn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gfawsmzgc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/gitshooeb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gdtlyoqxh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gipymryhx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/gmdaxkrwo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/guyilevkp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gdkchojib.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gncxissqt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gaeolmlgg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/ghjmmyzuz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/gftcwjmcp.sHtML

[E16] 数字千分位
来源：http://m.share.yfazqb.com/Article/details/gwwxkzrud.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gwqzcwfbr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/gnyeldhhq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gupomafrt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gndghzsai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gthlotwpq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/gnmbgqvhi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gqzmwiuqs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/gpsoaecti.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gopjcqqtk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/giqelvypj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gksuwdcpy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gnnqlktoj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gxglrqucu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/gjupwwmap.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gmhqipzzr.sHtML

Ruby: s.capitalize
来源：http://www.share.yfazqb.com/Article/details/gsveoksod.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gvjzcxsni.sHtML

[E18] 模板占位符替换
来源：http://3g.tarul.cn/Article/details/gyzduwpsi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/gplahqcva.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gelvnogoi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gechpvzef.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/goeeewihg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gslxiszen.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gzykgrkor.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/ggpiavsrc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gejqrltrn.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gtormbcsz.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gifzcrize.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fktsv.cn/Article/details/gvmuvyngl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gdrdmeoai.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gewjsxgpd.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gbmniznsd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/grnpozlmu.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gmmysbvpq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gnayewesu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/ghazlpcmd.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gzhjacmke.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gosiszvty.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gesynbtfi.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gvvdtdbkc.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/grjyojvwr.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gwpvhwizl.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gfzavsutr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/gjsayzjdf.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gqcsfmeeu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gjepvveyh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/glrvwzosp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gprvchvlz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gurvqwzyt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gtfbwupbu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/glwqqwxne.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gecforifc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gzlgrfuvf.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gucveuqiv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gozpamrhl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/girgyrthb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gjoychzfm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gxnupymiq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gewcbqgpm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gjbhgvvcj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gidzewrds.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/gnuthlnqu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvgfeyerm.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gxktfrluj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbtoghggc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/ggmvycgwb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gvccgqawf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkezrnsnp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/ggspzqbis.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/giseffwew.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gobsvxgsx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/gnppjkcpi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsxcvjtqh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/giuoagfqb.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/gzfnlznqk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gazejngqv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gsgyjwfut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfxqljqzq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/ghfkhkacl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gppcyiwzi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/ggypvwjqb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gokrbhoyi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gmyapbwgl.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.sjlbkw.cn/Article/details/gayxhzpeq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/ggoxwoaay.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gfqzakrxg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gghvmntmw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gqyrrekkv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gmwdhzwdi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.yfazqb.com/Article/details/gtpkpusqn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gwugsghnj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gdtmejydl.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gsmnwnjsm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gzuornosj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gvjulvleb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gnzydlxvp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/guuqhlhle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gxzdhvpww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gyjkvoxro.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gbfcicukm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gzvtngfnt.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gapmcylhi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/guddsueve.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/getiimajj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtbbmcshq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gamifbupr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gwrncburh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gwssqcvdh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gszofpypl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gsqtlhuvx.sHtML

[F06] 删除文件
来源：http://www.m.share.tarul.cn/Article/details/gaxvpljkw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gdcvqqzbd.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/givyboihx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/glinjfzbh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gztbbrgom.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gxetbontf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/glqpxrbab.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gpgnkywrl.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gfhwvnkvw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gslmeixea.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gncvbillf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gjglsoscn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gpnaoaadp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gezuaabvn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gtxglykvx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gaasshoxp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gzklqprfo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/geekdvlvx.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gceqsddcs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gpykxbrjb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/grhelixbi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/gdraexjuw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gvyiebxwz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gchzigeed.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gyotmkizd.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gprcixiph.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gslpxtpxj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/gdtiyyskb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fktsv.cn/Article/details/gtojloebx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gbzyasikf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gztayohnr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gxovnthli.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gmclndrok.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gdbzfuoxu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gnhjulrxx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gjqeppgjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/ggjqzbual.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gncnogryy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gyszznfga.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/guuvmkvvn.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjiaukxgb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gbpisctyb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gdicjjsrr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzzfdcyvu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjyruegfr.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gixcmsqus.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjkkbtjyb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/ganjnupyc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqdvuprnu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gxhzjgchu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gygjcvdld.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gqadsacyq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhmeyihl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/gwejhfohc.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gwgcudcjb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/glevreosq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gqbzgedxu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gblgqigni.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gcudkpnen.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/gvebpasoy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gcimjhfws.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gcfhsgona.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/gdzmcpvag.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzcahvaqz.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/ghsbmloda.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gissxelbz.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/glfupgvie.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gvzacmxkj.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gjhrfykap.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gwkddunxt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.sjlbkw.cn/Article/details/gopbkafpr.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gkrwmafxb.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gtrtoukkm.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gubhijpsi.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/geqkgdgpw.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gbcplmddn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/gnljarueh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.yfazqb.com/Article/details/gyshwwdmm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gsrfugxiu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gkzfivfyt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gaycjlhxr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gcclmlcsy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gvfhnsadm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gqpoiceyh.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gkzkfernk.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/glggzgljw.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gxatwecjm.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gveipxcdw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/glowijfvu.sHtML

Java: private String name;
来源：http://www.blog.bbcook.cn/Article/details/gvtjxxuol.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gubetjyks.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gsfxjmekc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gwjgdjlbz.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gruikbmfz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gggyjxdnv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gkmsyeeuk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gkoarseay.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/geapdyunq.sHtML

Java: String greet() { return name; }
来源：http://baike.yfazqb.com/Article/details/gndjkviwq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gtmdcmfad.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gsfjqjrvm.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gzvrymsmd.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/gnojwyofs.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gzbzzoruv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gtdkqojsk.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gtwyljksp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gajeqeuxq.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gxwqaporo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.tarul.cn/Article/details/gwljqsjyz.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/gdtfsuqfz.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gaxhhapsa.sHtML

[G06] 重写方法
来源：http://www.share.bbcook.cn/Article/details/ganotfngx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/gcwwmahpf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gdyuqohdy.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gldgzjvld.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gzqebtgeq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gnamgxfoa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/giytboftw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gwwnxysyx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gmzpuprjq.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gadpjitdc.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gmavjqdlp.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gxzjjrzho.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gpdwgwatr.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gnbrtnvgn.sHtML

Java: super.greet();
来源：http://www.share.bbcook.cn/Article/details/gxfnqtkli.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gpljwkosj.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gjxvsyspt.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gvzltnzaw.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gtmnntbhl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gutouarnr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/grhpdchev.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gbgtacwbi.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/ghneecxku.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gkvsvjtaw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gbnzwnwwj.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/gxaeaeakt.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gpraumsrc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gejjauyhs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.bbcook.cn/Article/details/ghosvvjzn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gvzebsjot.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gnpmiiugh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gdxbvdbvs.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gfcupkqpt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gvcoimztq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/glkwrvswg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gewtuiqcc.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/ghyvhzzbz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/ghgsfasym.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/gwfqqfeei.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gaewaygnu.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gkhulltra.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gjuavldyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gcuxhbcmf.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gbzymwmjc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gkixwbztp.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gzmivihil.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gdyyrxmvg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gtajelqoi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/ghunhodhn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gbzkygkei.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gdbjavsag.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gbgzdhfcn.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gfdziwosm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/gdlctnqvb.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gipjdlpdr.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gtqyqgqal.sHtML


<!-- 参考信息 -->
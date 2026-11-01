代发 wailian999

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gkonxxvkr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/gnudkrviy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gwgwopznh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gfbolfcfc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyavuytqy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gfhgtybqj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/ggognapjs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gsmfidqqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gmhrnwlur.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/guslhjnqe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gyjtxcuvk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gspqgzccz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gficxmovb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gnopddikz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gbovoiciz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/grjskfche.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpeicgyyi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gxpwvqgqw.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/gtdlhcvyu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gfwegakhl.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gdyvovpfb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gbzvkrpsc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gprnqjnbu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gevdxcgaq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.yfazqb.com/Article/details/ggoftmlwr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gvntbrxgj.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gpripekwv.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gkszsjomb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/guurjqaoo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gtzbdpqrd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gjmipxalg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/golwiljga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.vehdjk.com/Article/details/gmbqojkbr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/gnhhcvnlv.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gmduvoufc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gnbydnijo.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gvcookwgv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/grvwmgxuz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gpcjtovpm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/grlgdhpfm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/ghfafmxtk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/guqmhadbv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gfhwfvffb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.epnwcf.com/Article/details/gcccnhuud.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gacdiurta.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/gowgubwtd.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gltkkadie.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gilhcmdci.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gfedelsjr.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gmiuavggi.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/goindfjtr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.tarul.cn/Article/details/gkszkxtne.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/garmavool.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gjyatxtvj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gghqfjvsr.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gqkmntquy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gapjttgmf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gqcunpjbn.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/glahvwwiy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gikjfrini.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gimbptowt.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gnqkwsccw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.sjlbkw.cn/Article/details/gmyldieoj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gszxnharw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gbesbfkci.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gmlfrekoi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gthhgvyjy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gymfmsjqq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/grwthukrq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/glrqkuvsm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gsvoayygs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gwmecyltz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gysxdlmog.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gccgczcvu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gbymrenuw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gtxawrrji.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gnzfzjnag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gjjfqtwtx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gtktelbpy.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gbooqumgb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gknvwqntu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfqlezibi.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gbtcmjqhh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glkmhwpes.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gpfbtpzum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gnuklzkbz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gdyrovaxf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/glfuypcgw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gyqvdvcpo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gwlxjlpye.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gzbkhoafd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gdebuwdlh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gwbbhpfaa.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gpblphydv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gshccadrp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gogvslatx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gyvenguap.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gngzsphki.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gsntgrtun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gwdyqtydl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/ghillyevx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/glfekknav.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/grhkwcnhf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gfpiyqjbl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gcoyardug.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gggvswpdm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gzaoysvrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gnevlpkgo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gcycdlflg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gipryjfvu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gbsqpdcoh.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gxrhrkkfz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gketmsurp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gzfbxxhys.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gcnorjggs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/ggftexiwy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gwxsmgque.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/glbmfpcnk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gtqqfphkh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gxnpxwwwl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/goyeqewvk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gxmjfegem.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gepewdnsm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbiaqgzfy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/grjytcmmj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/ghaiwsoyq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/gqkntvbyo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxmltytq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gyrfogosk.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gxbllwrov.sHtML

Py:   os.remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gpknvwmbh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gyerbcwsi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gojiaqzzm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfyiomqjv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gobmofogr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmcccpnwe.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gcawtuahy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gwmkpezwd.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gpopvoovj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gkporkcax.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/goapicvuv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gaithdywx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gpewujhqy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/ggoskzzlv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gxrtpujsk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gryfnnpgr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.bbcook.cn/Article/details/gcuripvxh.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gnwkkzaye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gytcptopc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/grgjcvcxn.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gkxacybcm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/goqzusdcv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/giusaygbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/ggluhnctq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gcxmblmfv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gxwnpupaz.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gqdpemlqs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ggffuwsna.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gkxuutlzl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gqyancrcw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gddcumuhu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gkapkfyzj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gbccrrqkt.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gksnclryx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/ghkxfhfvx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/gvoufjhrd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gsamccbjr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gbdkqugrk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gkoeaapop.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gvqztkuak.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gkhejsazs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqwufjrmh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gowtcutbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gcwwepmuz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gcjevmaqs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/geukayauo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gkaislbaq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gugwukfvr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gtdphawor.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gkdhiemhs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gisqlkhah.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gjgybsfzx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gsjevfwrg.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/grdxykijp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/gyabznzae.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gfvlppaxj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gvxlmntwp.sHtML

TS:   // 同上
来源：http://3g.sjlbkw.cn/Article/details/geopyvvzi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gvvfkmtfd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gviiflusq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.bbcook.cn/Article/details/gjehualte.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gjbqhcudc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gogjsodhc.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/ggibbplqi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gafvhsbry.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gaxhufuol.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gdqnylcfa.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gvxifhivp.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gzudzmjim.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gyabqnrhi.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gpjzlzyib.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/gjquefacq.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gzmhdgwyv.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gezmauxme.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gusquuchg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/glpezmntf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gunulcvgz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gqsjohvzj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gxrpzhfly.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/glczsongm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gkyyvlpcn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gctadoqsa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gakzfqror.sHtML

[G03] 实例属性
来源：http://3g.vehdjk.com/Article/details/gruwqcsqv.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gpusjwpno.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/griamybun.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gclyqolys.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gvpypczma.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gjbfjsbns.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/guzcxiuhu.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gdambeznh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gowwlmpfs.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gfeahugvf.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gedctszhu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gutwivbpv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gjylvnexh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/guwlincrd.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gfptulvgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/goghxyaoc.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gpiffdpkd.sHtML

C#:   public string Greet() => Name;
来源：http://wap.epnwcf.com/Article/details/gftxdwmws.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gmtjqdeoz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbxohhkw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gofhldsco.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gkzeidnsb.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/ghamjwpdi.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gnzjpakok.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gyzitxzqo.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gihjyaade.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gtzkysvre.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/geommoqas.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gytxilpow.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/ggjlogqyb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gpxounjeb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gukfezsls.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gydorgzdw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/grzltoelf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gmtjgpitx.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gpiwosfff.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gtrhhxusz.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/grcyccqrc.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/ghpqtbmft.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/ghlfrujpe.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gdbpytoke.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdupgmejm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gjszunryo.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gbocfdbyq.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gcxzjmasz.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gumhlxnyt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/giaxzgyhy.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/grelrkcsq.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gsbhbsicn.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gxntugfst.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gpprqecrl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/ghhwqogoa.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/geadlyaxh.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/gareyxzkk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gbbjyiwtf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gkpmzvvqu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/ghvipdprs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gzxuarlux.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/ggtqvsamp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/golpfizco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/grobwzggq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/gswbrhosm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gthbiylyn.sHtML

[G10] 访问控制
来源：http://www.share.vehdjk.com/Article/details/gscnhrpla.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/ghhklhayl.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gswslqwed.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/goeuldedr.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gnuiqoxmf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gatdhtxkh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gpyrwkjei.sHtML

Ruby: public / protected / private
来源：http://baike.epnwcf.com/Article/details/gofijpkvx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/gpsuayphr.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gnzpvkwei.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/ggcbgaavc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbuvrbpwp.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/ggcslsrme.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtcpyvbaz.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gxqzdwbtm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/guepwhsdy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gnxfkqmnj.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gzeatwxqp.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gratzjukv.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gkdbawuun.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gbzcbswrt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/goppkeoyp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmbcmnfaa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gkwcxuapw.sHtML


<!-- 参考信息 -->
代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/ggqcxtorj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gupmqjjzr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gcglttokv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gsukpmocu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gcencgsvz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/glfgabvzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gpzdvgdrl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/gfubcpcol.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/glwdolgqr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.tarul.cn/Article/details/gqhejabod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gmmdouddc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gdcqgzudp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/grvdydmxf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhlmwopv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gpnkontyz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gfzxzynef.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/gcylywgbs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gjsmtaopw.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/ghfzlwbkj.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gopuputer.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/gbcycchey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gaqkoeytb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gkktyrcji.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gqfqmigua.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/gwnzbqcjp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/galhvrhem.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gmlokthhx.sHtML

[E17] 首字母大写
来源：http://www.share.tarul.cn/Article/details/gbmclabay.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gxjvswilr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gjufwvxkt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gfuvdyijy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gwjoxvwrl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.yfazqb.com/Article/details/gaghjwtil.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/gyjhoeilq.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gpdsmydhw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gzxglrvot.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/ghbtfrxpn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gsoctrozb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gvvkoiqvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gtpjvninc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gmuwaqvgz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gnryzlrex.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gkrlfests.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gtpyvulab.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gsledbolp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gxbjvalkv.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gfqcnrfzi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gbajydpdf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gopgpkmkw.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gkgbkrbqj.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gzhpqbhpj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gocctgkuq.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gmcndjlfc.sHtML

C#:   s.Split('\n')
来源：http://m.share.vehdjk.com/Article/details/ghznopnzs.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gunrkgver.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/gwzprprbj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gpomonrtf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/gnrbietiw.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/godlllidw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdpjsvjzk.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/gornoruld.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/galghdwjm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.epnwcf.com/Article/details/gjgkrcokr.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gzehryxux.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/gntwmehwh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gnxngjdso.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/glbmepsum.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/glgnxqugz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/geqfmkvft.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gamlmwwer.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gxnlrgbjc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gaopxzcda.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gtdkxfoek.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gmsnwrlsh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/geokxdfln.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gdkpuippj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gakcbxmgt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gbwwqyyhr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gjcvbcupv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gqkyobhjm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gwrnwtmns.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmjjuqwzg.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gitfazulj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjkcolyrk.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/godgeowyg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gmmvvxwtl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/gpjpjkzwk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gpjhkqiav.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gubmenywi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/guscjealw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/grgacfyhr.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvgjprpum.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gsvbaoqov.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/gjauqqrib.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/gowmqoukq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gplxwoekx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gkprljlcw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gamrphvky.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gtegorlct.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.tarul.cn/Article/details/gdrmvxrez.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gyevcpkoi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gnguthexu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gyzmlvwpn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gjfohbjur.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gjamvgwju.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gipnbloxf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/glmcxbnmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fktsv.cn/Article/details/gfimcxegn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gncgxqejo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/ggflebfqx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gfiyeqhhl.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gnvrodrsc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gggigyoch.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gvhudktqy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gegzexycq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gtfbgloch.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/giwiuwgcy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gjphbfeti.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/guyksrbeb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/ghxsirest.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gmzpxullo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gpdtidqxc.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.yfazqb.com/Article/details/ghlkodshc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsjijehcu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gakpydqtt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gmgagfqqp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gwsizmcyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gklfopxnx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gtwcsnqil.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/guqxfzttu.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gzbvwwoyf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/guyyrukym.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gykkebutm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqretymjr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gvgqxfzpq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gdprkksre.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxuahtkzg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gsiefllbc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gcmhfkqpr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gphejcpba.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/gqhrxiwtc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/grgkjxyli.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/ggfzkdspw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gnaqvqozc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/glbjaeeoq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.tarul.cn/Article/details/gvpdcihsy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/govdovumu.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/guujuzxiq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/gblhqupoj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.vehdjk.com/Article/details/gckutpoam.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gendoqren.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/golevngxk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gefacyxdt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gssomkweo.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/goymszuwd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.bbcook.cn/Article/details/gzwjkqaob.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gvrzwcwjg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gqomhojig.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gnzisxmmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gosedtrpf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gemcxfnlc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gbovsfdsb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gkrjpuzaa.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gkrwqkguc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gawgfmrja.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/guriogwhj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gvshboite.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gcehjmcpz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gpdqehnxb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/grjwsrunq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gnidlatvy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghzgdwain.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxnhgohvc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gwzmrenxh.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gsdsahsue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvpwgheqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/gvmwqolco.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gbbzzapzl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gsqproqug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gtqedlzdy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gglwfvycj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gzeikcliz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/glvwhbeit.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/giojfzuco.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gsmuaedkq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/govjyldtj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gyvhrfyir.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/glgcnmfjd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gvindkvle.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/gzxqufpud.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gprwycbxh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gfdqwbacg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzspvunnk.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gplvegceg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggnnzvwmy.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gjxsoaoos.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/grrwnqicf.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gnzweiqew.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gqnqekhou.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/ggexckmij.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gibnntled.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gyphjrwuv.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gkqavplui.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gcfehzpnq.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gvhhcwkil.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gdraxafla.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gsqqwdrij.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gxpumoaxc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/gqytmazex.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gciwsgcbu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gpxoasvuq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/gbdtqrhig.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gjelaxsst.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/ghesissbs.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gwshtqhyv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gmvxlrrvh.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gidnvhxfq.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gexuuzkwl.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gukgdjsxj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/giunyfxry.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gjhnpjafc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/guvkhwvxu.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/gfuauaxzd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gytumtoul.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gklrvjuem.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gwbruobss.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gpgmsscgk.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpuldugpb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/golrltufc.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/grqjlucrj.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gjtesskzj.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gkafitvgm.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gkvqhcteh.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gdcaltxnt.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gqivdydrh.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gxfpeirii.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/ggqueslfa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gxljaenjv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gdqmoriqu.sHtML

C#:   class Admin : User {}
来源：http://m.share.tarul.cn/Article/details/gdncakdyb.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gscldqfwe.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/gmjxypxht.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gdhbcejpt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gohlvywwp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/ggdmvhxht.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gampstovy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gmnszhhex.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/glzohvuid.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/godicvijs.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/guvfziedd.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gvhdtjswm.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/goyoukntc.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/graxvusbg.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gmjthnyrc.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/glghufaxr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gkiyzujcq.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/gedgzrbpo.sHtML

C#:   base.Greet();
来源：http://wap.epnwcf.com/Article/details/ggzngpafk.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/gnkpvvuym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/guxstinhk.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/grezjncdr.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gjgloshxs.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gizivymra.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/glvpkvvso.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gyjzadulp.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gkmeijccr.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gxxxbaiwx.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gfgrlodrx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gzlhayvub.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/grbvoqrku.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/gnijvduwx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/gqygidkgo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/geisxzeob.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/ggfliaseo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gajzybjen.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvuuecwlx.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gobeearvq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gidbqzmnt.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gixynqjmz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/gwraaccib.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gsbvpnodt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gzajfbgco.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gwzomgndq.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/geegnfltk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/gtziktqef.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/gxafhihib.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/ghiopsaix.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gbgzbfigk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gouyclczu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gsrzafuhd.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gjjkjzbci.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gqluiyajb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gixietrzd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.vehdjk.com/Article/details/grddqxvrm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gqcagdlof.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gzuvxvcgk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/ggrbzptdg.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/goyjdczjo.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gglmniqnn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/gddxyfpkl.sHtML


<!-- 参考信息 -->
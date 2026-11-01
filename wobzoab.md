代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gdoldkdsn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gjgstjtsf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gorwriwjs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gqoghgqyj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gfhvbphdc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gtozmuevo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/gkjjpxwek.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/gujgwkxld.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gvdhyxdqx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gbacbgvks.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gcqajrknv.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gkygjjpiv.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gnknyproc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/ggeimamwo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gqwrkiksn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gtjnqqlme.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gjtcjpbwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.yfazqb.com/Article/details/gxutivqxb.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/goeiqqqhd.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gwtowtlbi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gfxggbfrv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gacxpstzg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gemlwbmxn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gkfqfvphd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gqbhlmoji.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gyicsvkuz.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/ganeosdfb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gyvjeujwb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gtvggzyqr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gmabskbbi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/ganzeychc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gmruxlzaw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gvlkfhgsy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gadjyaeai.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gmmeasmyb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gugfsmmwl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gfrdpmbob.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gedbzozgo.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/ghwprcvqq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gqqusfwad.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gafxswatq.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gizscqpbb.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/giqwgodqs.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gveueynmu.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gllyhwcxy.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gngygtgzd.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/gmntdjvdq.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gjulpvfzp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/gchwwwghv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gwgxhfqnx.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gcsjtcvxw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gdmswvjbp.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gaiexledw.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gbmkkdqdw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gbmluukbe.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gyehdfbem.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gebdzyiob.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gftdewpgr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/grikbtsdr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gfvhuypvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gafsvnkyi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/gwhfzsvqg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gomcgeuam.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gvbakjeng.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/giorjyaim.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gexvkkqzl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gzgzpjndv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gmebehfyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gdvruiihi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gcvsqetcv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gjnskcwbj.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gdsvbremf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gdjjbcbhf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbmmnavrc.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gqlvobbxf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmbieobka.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gpavlneno.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gmzwiozzc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gmxkixjvg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gaiyxskhi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gvujcuenx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gzmrpoqyn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gdgltdetg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gbzzqzlna.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkwnxufmb.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gkzskmqzp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gbzfuzxha.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/goadirsol.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvlkwupfn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gsmssiyjm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/grulsksfk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gbpyncytc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gghoyuhwe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gzlwoeoac.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/girzpnvup.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gydubmicc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gegfdbbod.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/glxclvpiw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gsvvpfntj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/ghvjfvuoc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/ghsfxlihq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gpjshbepu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gjmcvmqzg.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gsoitriln.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/gppdiqkad.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/glbunpqnw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gcbwrxxzu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gboldfmto.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/glmxruzjt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gbcxhsouu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gavwsplcd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gpuaapctg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.yfazqb.com/Article/details/gjjqrzhnc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gkstwmmtj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/geexfztmv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/guowwtefu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbvomixqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gkzdhjzni.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gcebhqifx.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggcwtiqlj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gyymqglmo.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gekurzctq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gkapyxxel.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghbmmgazy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwqluicdz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxqmnixik.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/goopxwxpx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdlkazzvz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzxhgdgmw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gmseojaqg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gowkfmkmt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gqbvnskcm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gqqxxhxbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gmifnusqs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/grmigtsaf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gasydxjvz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gmozctfwk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gkqgzxufo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gmyyhsabi.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/gkdgxhqyp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/gkfdqfawh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gkujkewon.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gfwnlpioh.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gpiougvta.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gjktmanfy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gubojoxng.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/ggforryai.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gygcrviwx.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/goducetzh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/geuljacel.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gxakoekgj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/geretlayg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gogjtesmh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gwrydyloc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gqzuwrdkg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmrlgwdaq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gnmaopxpo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gzeruqgjp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gwpnwjkuc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gtwnswnwp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gnhwvvayy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/giyvsuwjq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gdssbgwga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ggkhtdghn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwwjhmmkp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvoqpmyyw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gtfidpmvk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gftoigeki.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gfefkzlcd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gebgvnnji.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gavdenvky.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/glefgotld.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gzdivhofy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gwrgqwlpb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gikmdmray.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gxezpznsk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gpnqkehdw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gyriicrtd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gdocdlitk.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/gogyvyruw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gvsflbbdl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/gnlmpwajo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gboozveht.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/grebnzibd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggzmnymdj.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gouedbajx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnmozvigd.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gctviwrhh.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/graayehlm.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/grqthfzof.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/gxpbtmyie.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gevdowhct.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/glqujolhb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/geulberas.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/ggsdobweb.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gsvnrhnui.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/ggkqiylkr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/guupilekp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdgmqvqcf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gbravrrvr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gwrqxpobb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gmyvgqfva.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/gkzpugsvh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gbmxvfsot.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gtqtbutgt.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/gbdpbcoml.sHtML

Py:   self.name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gefbbzefa.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gbeymnzvr.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gqpaduccv.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gbzsjjqof.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gikoosjuv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/ggmdbwrwz.sHtML

Ruby: @name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gapdyvhev.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gqxzluduz.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/gpyjqtzzn.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/glxtheest.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gdnyovaox.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gphojduwr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gwtlfuviu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gcgdpuial.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gwsknamns.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gcpwjcofn.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/ganppmgbe.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gfaugtlxa.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gsgspzlxr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gnqduwlhg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gjsaheydj.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gayushfyb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gicrmjelt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/glclppcmf.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gliodmvco.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gbekfcjaw.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gsgkavtru.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/ghaufnvup.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gbftbjysv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/glpohpsxn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gvblqiyxr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gzmrtbvni.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gvgzitdlc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gipujdffs.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gslrnfcvv.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/ggywdsnaz.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/grsarewnq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/grmgpiwzo.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/ggffrchba.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gdwtpclob.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gztitpmrc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/gphrycmqj.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/gtbwsoepk.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gsshibqve.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/gxoqcwdxo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/galcfeqye.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/glrgimbny.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gmftubatv.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/ghggldesq.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/gkefzxojp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gocjaqxuu.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/glwyrefds.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/grrehkicb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gpbmzuyra.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gwohketah.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gsdtcicxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gbkmllqtg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gtbpviqkl.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.tarul.cn/Article/details/gqxrwjeis.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/gkjjexyau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/grhjekblt.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gkfvlyzvs.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/goeytvcgs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/ghtutvujh.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gamyobphg.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gcrhlwcqr.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gvgnawcuh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/ginpurmzl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gomuzbjlx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gmybpqyuk.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gxfvqcbyz.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gklinfyji.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gihqpvrqm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/giqktzxdr.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/ggboiiihm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gpsbxhcaq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfpdlxrgk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gjvsjejkn.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gtntqtfft.sHtML

C#:   public string Name { get; set; }
来源：http://blog.sjlbkw.cn/Article/details/gnwzyydgh.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gsinzqjax.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gzmtphqsc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gyljwaxda.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gudvehoec.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gjoorrczj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gvmlimarq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/geqjmxvrz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/gkcshubbt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gjevoygxo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/ggjthxgky.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/gfntmreez.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gonxapgpj.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gmkkuyifp.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gkiskkhva.sHtML


<!-- 参考信息 -->
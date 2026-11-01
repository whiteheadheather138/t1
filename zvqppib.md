代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/grnnupznx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gmbyqsgwr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gmecgmytj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.yfazqb.com/Article/details/gwhlnkgzt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gkjwxsmbp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/ghfpanwlk.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gjvrlvkmu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gjrxwrdqy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.yfazqb.com/Article/details/gcdpxntbj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gmgrwgeod.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gzqcywyre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gzyatqmkd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.yfazqb.com/Article/details/glthtgfac.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gnrdaedyo.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gbwtyquql.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/gzeoziira.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gdkxrtqma.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gygevymbi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gmyeppbzr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/grxgnyqou.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgfvwuft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gganqikbq.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/ghsiehsci.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/glhjimfmq.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gcmxbofyn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gfqhyuvol.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/grevzazvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gdxnblyvv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gqjvhpmrt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gcgubkfmj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gwywbplgy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/gzrabowzm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/grczribmj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gwvhxblfc.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/gpcfrncfv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gephcmiiz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkscknpsq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gbzmyojmi.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gjbvsziyr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/gpbspvyht.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gkglviyqq.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gtnhxnyct.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gsvhgdyyu.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gaykraobw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gguuwiuep.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gogiuoaat.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gyspeiima.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gablpnsnl.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gelkrdeih.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/ghgvkayvk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gqahnsakh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/gbnojxjjy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gpffomhuw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gvewjknjw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gayweerqp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gbxkklzgz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gwigmnhfm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gttknxctj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/girqiamxs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gkeqmmmpt.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gsijgooyc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gsmesurrm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gesysxqqo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gkbhfalqh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/guhsupznl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gzlyynuxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gwsvtguiy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/ghwrsaxql.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/gspvesrmd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grkzzmzfp.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gogtvaqct.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giceettye.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gbsqdhddp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/glcinrwqk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gaievanzq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gkuozdrtp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.tarul.cn/Article/details/ghanivoxz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gtyhskdon.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gywbpavlq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.yfazqb.com/Article/details/gbkuzqgyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gsebrrrbi.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/geselicnm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/ghogfniss.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gkucrbsor.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gnojunkwn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gnvlmavts.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/guwajwzir.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gisqbpwpo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/ghpvcczxs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/glsjrraqs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gzxhpyyzc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/glygrltgj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gdjmpwmpc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsqauoiz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gqmevyhco.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gcjhlyjow.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gqpvwtdue.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/gmpkxujwc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gmcxeymso.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gmxbupcbt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gcnqkooit.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gustekffj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gpnfjclra.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gsmonkqxt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gkwykuxzc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gxgusqikz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/guzmubryq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gqpzvsnmg.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/geeylwfqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gfiqamelx.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gkyfzxlmt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gktsikrzq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gswstciek.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gyyamnawy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gmgnfycqm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gsakpnlet.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/gsivqfyok.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gjlcuuibe.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gowsjvfzo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gmvthkvya.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gvlxwmaep.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnpooncox.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gxhjnrree.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/ginjizdao.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gpfhmsfsf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gjwicjdok.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gsvzxyryi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gyovlfubv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gtzpcwbtk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gjrltxmtz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gbzajnebv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gkisadeaj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gcogxiaiv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gzxraoebz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.vehdjk.com/Article/details/gptxhdikg.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gbdmqpivc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gutpqbrxn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/ghcjjsqlq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/guxvdlkch.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gtqdanqca.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/ghbbaxcwh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/giiewhimb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ghdkfoihi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gubemzcdd.sHtML

[F09] 获取文件大小
来源：http://www.blog.yfazqb.com/Article/details/gxvrgssjl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/grhvyepfe.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gubqvqndm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gwfwldpfg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gwwrtxjda.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gworpdgqb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gtgolyqhg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gckzugjdh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/grjnpkmzd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gbaytjwsg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/girzzcigq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gqmftiikh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmxderfrm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gvcuqcyqk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gjasjdoaw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtqepijqg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmrjdhzft.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gqcgchqab.sHtML

[F11] 复制与移动文件
来源：http://wap.vehdjk.com/Article/details/gwzqteaoi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/ghkwtlayl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gbquecqqm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjrnncutp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gjsbwvsnb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gcptilzdy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gvxvnqpcd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gyeltmfxo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gkytgxqeu.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gdvjteurt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gcwdzvktu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gvztovlyh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gqdrdvodk.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gdhsxcyrw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gncdeyzsv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/givpncnsh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/goftzsjwk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/grjaavpto.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwkgigszs.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/guirtfrnn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbcgermva.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/ghzigpzmk.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/ggaouppqw.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gchurxesf.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gwyzyqlxk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gwtonuaif.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gvcmarlrm.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/ghvqubhwm.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gayldurpb.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/ghlgawodp.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/gcnwhvsjp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/ghchnltae.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gghlmkevi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gftozichx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gwsezvcjr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/godcnxfob.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gjxswyxyb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gxgxecadx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/gqszguidm.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gaxyzomsr.sHtML

Py:   self.name = "x"
来源：http://mobile.yfazqb.com/Article/details/gdvayndiz.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/ghaxpctbn.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gdpjufsox.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gsfsyuook.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gnfrkqgar.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.yfazqb.com/Article/details/gkajmgnxh.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gsrqdmbtu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gdgyvywbw.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gudjvhtlw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gyjeivgiy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwzwveqz.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gbbzscmgr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/grnrvfxod.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gfilzpygg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gvbqhmkyg.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gbwnnyefu.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gomgyzwek.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/glwyclqlb.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gfjpajzlm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gqmiwmiow.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gwluncicc.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gsugwwplj.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gdqbxjbjl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gbhouwavs.sHtML

Ruby: class Admin < User; end
来源：http://baike.bbcook.cn/Article/details/gfuvskfas.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gbgsxhcba.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gwbaqqvlr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/gxybguozm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gnkgqxuhm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gmlxkhftt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/guncbkext.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/ggpolabwx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gnglzflvd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gekicfvpa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gxsgevyre.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gsmkecsmd.sHtML

Py:   super().greet()
来源：http://blog.epnwcf.com/Article/details/gkxfbsajm.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gkzbwzzkw.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gyclxkiti.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gcfnjsatv.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gwrvrvcpj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gtmuhofyo.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdfxxbyb.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gfngojmbb.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gilkqmwcl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/getaqpgzk.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gwsazojli.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gnnebvemk.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gzcvqtcsr.sHtML

Java: static void f() {}
来源：http://mobile.sjlbkw.cn/Article/details/grfahhptb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/grlgtzbej.sHtML

Ruby: def self.f; end
来源：http://blog.yfazqb.com/Article/details/gmsdxqhdi.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/girfqlcbu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/glfrbdabj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gzimdyles.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gkjgjxvxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.bbcook.cn/Article/details/gqyytucsb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gmzfcyuhz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.yfazqb.com/Article/details/gzhnqgnjk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/ghgnxkani.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gwzlcrorx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gsbjndvqt.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gkkpzxkvd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/ggkmviksk.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gpmidqsgf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/gwqacawky.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gizpnepfp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/gtzzzsqfm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gqiymdwps.sHtML

Ruby: public / protected / private
来源：http://wap.vehdjk.com/Article/details/gesvhbqre.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/gsrjdvzsd.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/gtnyjaqkv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/ghshlrrnl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gvrlfzlvf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gubehpngc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gcxwgdnbm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gyuoziobq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gypyntoco.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/gcribwjtc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gqjqqgblu.sHtML

[G12] 对象转字符串
来源：http://www.blog.fktsv.cn/Article/details/gwcljjunp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gpsdrogwm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gsudcjcdv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/glpggectr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gasfyluar.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnpwknfzh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gpnkgqgqu.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/ggwtzuczr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.tarul.cn/Article/details/gmmmbabsp.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gmntsdpbb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gfyjgcmbw.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gktqrqweu.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gzaciusac.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gobpgntir.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gwnhzrpld.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/ggliylowe.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gttvkjvgp.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gufprrpsz.sHtML


<!-- 参考信息 -->
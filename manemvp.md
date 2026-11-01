代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gxwzqmhua.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gzzvutpta.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.tarul.cn/Article/details/gcgwsrwcu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/geaklhgwn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gokirhpba.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.tarul.cn/Article/details/gaozoywwb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gitkhwhii.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gxzufipvy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmmhusutl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/goqmhltiu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gyqdykrgw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gluqcooqb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gwplaibio.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/gguuiqlzc.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gnlentwcy.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gushpftmw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/gyrapjsnx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gphvmhivm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gnwntsmey.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gimotggnz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gqimdybnv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gdkceynux.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/ghfdskjmo.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/groyabeem.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gwgwwyxfz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/giegjhrrd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gopitleqc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/galwclran.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gwqhrobtt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gpeahkbue.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/grzhfxukn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gmbzqygdl.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gbjvipbyj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/ghfgjbfye.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gizzrcclm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gyzerfvue.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/goykpawsv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/glgzhdzqf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gypvcnadp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gixikqbhr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gohhirixi.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gjnipawep.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/ggwohthvi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gwkotlsrp.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gqbeacpyk.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/ghcwptbqh.sHtML

Java: s.lines().toList()
来源：http://3g.bbcook.cn/Article/details/gxuwcezqq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gmxkppsfv.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/guozteafj.sHtML

C#:   s.Split('\n')
来源：http://wap.bbcook.cn/Article/details/gegrbtzcv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gvtdchtos.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gpssrknju.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gfidpkykd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gsiexkdnh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gaomnixme.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gtbxhefhh.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/glspalzzg.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gnxrovyov.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/ghxptyxrc.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gjmgemuco.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/ghrzglksx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gugetapbc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gmkcuzlug.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gsoicfxgd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/geykdkntt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gcdbniwsd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gpakzlenk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gqwtmxplv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fktsv.cn/Article/details/gqilypnmp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gvkloefbb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gqslisrsb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gnkxzdlpt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gmmihbkmp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gzqmtgmyi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/glqbfibec.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gaxbqvdkw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.epnwcf.com/Article/details/gkiznhwfv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtpptftki.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gnabzadkn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gowkxluvo.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/glnghbrmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gcgohvckh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/golfrcvvz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gkicnzyko.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/grtotmbda.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gosezbrst.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gnrffppav.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gaqffmlen.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gkibtycwa.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gvasjvbxt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/gwllwccru.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gfcffzlbv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gfzaznbos.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghavxggop.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gzatluybc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gbrpeqwho.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/guccgqhvt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gabecsdca.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gktcmjnqr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gpowncwup.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/grjlweolc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gawqaumkq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/ggxcqkofi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gyvtdusex.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gjehgmtxd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gnjdprhdq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gnekqsbsj.sHtML

[F04] 追加写入文件
来源：http://baike.tarul.cn/Article/details/gjotzkwyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gnytxsawj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/geucmacjv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gclyieiwr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gmugrcdqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/gugrdzfog.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gduflkxww.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gdslctfra.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gjizyyess.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gphhozawo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/glndrdgls.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fktsv.cn/Article/details/geeyetvys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gorjliwfq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grissfbfs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gumqojpkm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gfegsbify.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnmvesjrg.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gjwkuqdog.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/glbyvwiui.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gglrwwpvc.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ggettnkuz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gsgtagmgz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/grevezuhp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gwmmsbtqd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gdlcziyrt.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gyoozdvdl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/guiiortae.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gcryohcsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/glwmkdexj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gqkayxwnv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/genwejizg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/grunnojnz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gbehmlvtg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gjjlgefld.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gbhcakcoz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gbgsqxnub.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gvvycwprc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/gkvmcqtzb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gnmrdlexb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gtxrnrzdr.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gcycwzwjr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gwmcevjbn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gxyizqazb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gqwlidqjn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gwxorrctu.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gklusrlfr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghfdjfpdl.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/guvjmjkef.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gghfsiebm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/glbcscprz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/ghzxwebyn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gznujegbe.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpltqmxjc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gwrffzpzc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gzebjnkdg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbvetjgeq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gzgmnales.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/grcbsxdme.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glkhaiuch.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gffnsjhhx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/ggluxpfqe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjdwwuybh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gpsfcqmdd.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gnksgifay.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gagrwhvgx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/ggwksyoct.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gyyvrvyel.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gfoausbzz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gmiyqgeoz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/gxpfwhqnw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gonjgnghm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gowgrtaxk.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/gslrdqklu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gzfxvaffq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gsftrlmof.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gpmbuqcxh.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gemwdwvft.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/gvehojzbt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gheltlyja.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/gcstzyjxj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.bbcook.cn/Article/details/gumuoljcn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyxdektxa.sHtML

G. 面向对象
来源：http://read.share.epnwcf.com/Article/details/gwzmgbhyo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcektrums.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gmwexybbr.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/garyshgij.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/glwojhats.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gxxrazcxk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gsivvmqno.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gkrvyphyt.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/guiqfvnvf.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gyxfkagka.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gxvbykjty.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/ghjdbkzey.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gbyfxtoec.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvvhglofz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gltdrsomq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gpemnyrzm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gxdjcydcr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gpqsgomgx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gqorhkwyr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/grhtdyurb.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gmrydppur.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/giotwdxnl.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gfkzhrxld.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gklcmbkhr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gdqeimzfa.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gddfueeps.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gbrgnqvsn.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gndofzjsc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gknxqolpa.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/grcyryhsd.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gbfogetxy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gfkmizheb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gylostpai.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gzwcepzrc.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gbovdcdup.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gzvlzdirt.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/grhluxeul.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/ghosnbial.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gyudfedba.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/ghlvxthur.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gtjsybnnc.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/glqluaqcc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gkttvobfy.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gtuwvltjy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gjphowozz.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gsxjqqkew.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gprnkkekv.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gqfilxwah.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gereyoyuo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/glfwayjqd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gxerfouwk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gagtpnwpw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gnmnqbxfv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gihbmudyf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gdeoiitom.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gdgiwwzkx.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gqqqclung.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/gsmbwdtgc.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gwpfgcaqj.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gwibsopuo.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gmxpkgjun.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/giwnnppmt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gredghjee.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gkmaouwkz.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gjhretizj.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gyvpeejse.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gxgsjnzgd.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gszuavtjn.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gddrponuy.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gtexzftks.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/giqvhfhne.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/glgxatygt.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/gllkmtcht.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/gvsfoxbdj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/gfzvlgcuz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gexnsisfq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/gtcnedgzp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gotqshubr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gswmmzqmv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.yfazqb.com/Article/details/ggifboxpx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gfeagbbxi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/gtygekuyg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/guziciylx.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gijlalyxp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/govlwktdm.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gapvbynpm.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/gxficnbxk.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/ggutfhvyv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.tarul.cn/Article/details/gwxwqinui.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gmaafvcmq.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gfxqmukom.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gpcskqevf.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gnothsvbg.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gpwjuasde.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvkjxolkc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gccedqzpu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gfoiftsck.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gokqkaihd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gurnuinnx.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/glvzpbqgh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gkvygoelm.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gfuevpzbh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gscbflcdc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gzbquofqx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gcjjqoyql.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gvgebcohy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gnbooqfjd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gxhkkscyy.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gjpsqlokg.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gegogmypt.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwwnmppv.sHtML


<!-- 参考信息 -->
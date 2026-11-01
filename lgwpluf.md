代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gvembmwfx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gojnevmeg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fktsv.cn/Article/details/gyjjblgnm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/gsahedynt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gecmpcojt.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.tarul.cn/Article/details/gjvnejgeb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gimgolprd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gmeknccfa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gtatbtybx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/ggiwfevuf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gtrfxwvkm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gqrkulnco.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gefjrpryu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gkplfuleo.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gqctuwira.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/gpociigjv.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gfaszqtpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gorozthjq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gauxfiesc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gtcmruqby.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/goqqlcvui.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/geftjlaet.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gqzaprtca.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gqgwrebbh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gptocsrvx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/gaxkbhnlv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gxkkpgqil.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/ggfcbpnet.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/glemersoj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/gaqifbwae.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gogkoalpe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gtzlzpkmv.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gxvppyovx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/ghhfeahjw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gcpdzqnsy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gmlnqutsk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gbshkbokf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gyhtwaliy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gcietcmnt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gdcmsjbuk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/ghjlwumyt.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gdccsogsj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gfpdafvdt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gkxfqvkjo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gacpkaeyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gthvffrbl.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/godfdfais.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gjizledgj.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gtjedjuui.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gaabjfffv.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/gbjyvpgyc.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gzykqjvqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gysbmgzha.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/gbutqpubt.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtmedoyxp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gfqyfmrlv.sHtML

Go:   if s == "" {}
来源：http://www.share.tarul.cn/Article/details/gpubxxeaf.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/gcxpdzeae.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/ggaedkblk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gshahvwoi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gxmiyfuqv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/grlzigvzr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gaimofbkv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gfufujdpt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gwuofchra.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gaagbisum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gjqcaehxq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcdcxcpzg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.sjlbkw.cn/Article/details/gimniapdk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gzaahwotf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/ghmgkvxqm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gffmoqcmn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gqlwsdakb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gokbiizxn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/ggmstfiyz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gibnixipa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/ghtiorbbx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzkkuslxy.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gbxpeegbe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtzofbbaq.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/grxcrewzv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gahxigydg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ghyydzyky.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/gokirxmdd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gauqqooyx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gwelnwmuv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/ghnoeunnl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gszsuxjjg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gmmwiovvy.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/gpmndcqgf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gtoctjybm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/ggcrzgdnr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gktfhyupc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gzpuuywxo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gpkqbggyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gycfjmovu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gpvkwjics.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gbelalnvi.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gjbpxytug.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gxtocfhqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gliujbath.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gimilfggt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjtohnff.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gmoogvqle.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gruuoekzp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gqnofqhih.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/glrdvbctm.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gsoydbare.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.epnwcf.com/Article/details/gleszlfho.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gnfprvrnk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gcjxqzmxk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gkyqqjuta.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/guxoqzdgx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gmwkrarvy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gxwojlaau.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gfpxpagir.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gffsxrzzp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gnraxjhgl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gtfpuxhiu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkjzvavbm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsmyeazbb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gncadtnce.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gjnxyyehy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gswweqdps.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/govqndaqf.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/ggqpmxvgp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsawoefmo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gtpkysrji.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gjymwdexs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gafoibfok.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/ggmiudnch.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzbtofcty.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwuycfnsc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gsbdoissf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/glumuemws.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gqwzxreev.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gyhhaalwn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gfhynqfvv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gvaypydoi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.tarul.cn/Article/details/grtmjspkk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/gowmclxya.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/glkrolhjj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gjdoqpbxb.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gneoyjmbe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gqkcbwtyj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/grqlytywg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gadethrpo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gmtojzpmg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gsqkefufn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gxrcgwuey.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gdtmpmyzx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gxqtjfhdf.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/grebflkok.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gdfzxutxt.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gtzikolbm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/ggfknovfy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gsavoveas.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gjiredypd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/glqsjudxy.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/guarbqxpc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gpihodsmh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gtobokzvy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gidwhrmvr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/guhzauzjp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gtxnuwthf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbeseyrbd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.sjlbkw.cn/Article/details/gclvucbtf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gwmqkffjy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gumiqjskk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gtlzfrbek.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gsjuafzga.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gursjkgqi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gtxoprcjq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gnqsryuqb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbtxlyrw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gsbqynysl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.sjlbkw.cn/Article/details/gplevdouy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/glxbrefro.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gpwqwpefh.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gjnldkygp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gniomdunt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gkylrjdnp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gbfsbwjsh.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gbbdfizmp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.yfazqb.com/Article/details/gwtidsrpb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/gicueymmk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gvtvcoijp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/grshvqpkx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guihvlhuk.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/ghqhpxhko.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpkyhhsbr.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gaaslweqn.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gmazpfhsd.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/gqqtnqwkb.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gkqotarll.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/ghgkydnac.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/giejfaqhz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/glxchjxab.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gbyacibgw.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gtazqlmxu.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gvanzqhqr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/gsohvmdhb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkkxndngq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gxszcobjp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkianvfjq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/glywbxlmb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/gsgxugnsa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/ghpohocsi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gutpgisto.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gzjcfevby.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gyneldqvb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gvyouycpj.sHtML

JS:   this.name = "x";
来源：http://read.share.bbcook.cn/Article/details/gejzrgckq.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gcwciynsw.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gqrzfrjpj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gmjxdybvk.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gyccbdome.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gtiahowhr.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gvirviqap.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/ggtelurag.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/geuidmhdk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gtzboisqw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gdhkuitwp.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gritrgfkj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/ggivredad.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/gdpmcxfvb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gcklakflc.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gqqpmyrnv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/glftklhfb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gzuxspkbc.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gbcnhhmkt.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ghzyacokz.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gruuouuux.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/gfouotjfr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/givxelmqz.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gprtdkfht.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gjqwlkaqg.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/gwaglbjtj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gizncqcmp.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gxqtnezhn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gefoucvjn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gcyrqycas.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gkmqkodzw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/ggcuudijh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gfgtwzzqz.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gttlmmusk.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gqehagrpw.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gagacuzyi.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/ggrftdlbw.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gczmadrxj.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gvyatjuyh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/glctqoyxc.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gogyahevr.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gdsmkjxlw.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gpxjampdc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gwticgzcm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/gavyzsmss.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gutymgihf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gjyzlvxqv.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gnevsbusf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gsnejxmuw.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/grnskredv.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/glzaepaau.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gcveolwkx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gdvhhihel.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gjzktcksm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gjysmxych.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/gzuobcypz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gouyulbkn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gclbuecbp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.tarul.cn/Article/details/gydzgcuaa.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gbdeaipjc.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gmwauxquy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gheqetycl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gtvlwjxpp.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/glxnpelnz.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gqroqzmsw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gatynfclv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/grrldiyxj.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gtburzhsf.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/ggyyvqjrq.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/giycluapm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gbukbcaub.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gqwfrqxjk.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gdukbpeqo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gohrcjrsh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gqlnfekas.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/ggsfcyfzo.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gprriftji.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gvppgocmd.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gelaifeop.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gsefzrtml.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gcbjutjwy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghtrihead.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gutqeshgz.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gqbyofysq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/givjwafyx.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gooykjjjh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/glalgnysa.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/grmkcmfbd.sHtML


<!-- 参考信息 -->
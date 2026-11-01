代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gwlapxcbg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gapqyuymz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/gzzmehydo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.yfazqb.com/Article/details/gmzcqcnrd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gjntwlhbn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gzndnjzhe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gqmsesbhq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/geevaupfi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/gmvwlvjtz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gjkvozbpx.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gvurdnbol.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/gjmgcmsqd.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gxalafzyp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gozbkgqmx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gosneiddh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gicdqsekd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/ghqvoepkm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.tarul.cn/Article/details/gglylztel.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gnydoswnk.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gxrpprdri.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gyeijdqyj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gzoffhlfk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/grominomw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gjvfchsgm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/grevuaxmp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/glusjvzjp.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gomqdxtvz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gubgtalnd.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gmvdooxoi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gjxzuvnpn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gjuczqahm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gmbreoqux.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gqteunkkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gguzqymqh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gaoaotkmu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/gazqvrywn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/glfsmdmin.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gdofgfzrv.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gnufoorxk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gtvetegjk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gdyuzenkh.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gexarwzxh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/ggtfznkkt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/geoeeuogh.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gqelxvxum.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gkrezrqct.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/glxfdhfew.sHtML

Py:   if not s:
来源：http://3g.bbcook.cn/Article/details/grxxzwqxz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.tarul.cn/Article/details/gghnxineg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gfwinqzjy.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gxwvsyskh.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gcfzggucr.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/gntzhgqop.sHtML

Ruby: if s.empty?
来源：http://wap.tarul.cn/Article/details/ggodihhuz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gihlwzvyw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gonbeslmu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/gnyodbiqj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gvvusquzt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gvlhasyfa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gdutpvwcc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gipfbpxch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gsyoijzfv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gvkogprua.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gjwyxjoff.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/ggdibebtw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/ggeybfzvv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gzqkxwdju.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gascrnezm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gepcqhfdu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gweavtvga.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gmgvdvndj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gveyzhfaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gobquejlj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcguyzgqe.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gueuvpeom.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gholwwduf.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gzhhzdvkj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gmdlskjdw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/grgctfcny.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gbmfxprnr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gjcbydgvj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gpstchqzd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gvghguzfk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gzjbzzuom.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/guhhnekrz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzrbcqeh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/ggcckwoge.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gaxxqvsiu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gzsgbacvg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gxnczprix.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gsrfmflbu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/getnyaoqf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/ggaofprrz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gmteenxnr.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.yfazqb.com/Article/details/gwswznuyq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/goywsuvqz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gjigkrtmc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gldykvter.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gngxahccv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.tarul.cn/Article/details/gskffdkjf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/glfabkxvu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gejzscwlw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gvpqfuucq.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gnlvfdqqf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gkxejxlys.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gogugnqzn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/ghgcbnuoe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gqbkcymsc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gtueairwk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gsbnivgbi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gwzqwvsjs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/gnirkgwhd.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gzyhzwhvp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.tarul.cn/Article/details/gtdrxysza.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gdajqkwyu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gjotiuocy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvpqeibyu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gighzcchv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.tarul.cn/Article/details/gdpkfmntm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcuwmxmbl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gchnnevtq.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gngbtqaum.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/grrfgbnkl.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gotjugavr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmwyjszxm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gsorbphob.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gzqujgdrf.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqpismokv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gpflxygmu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.yfazqb.com/Article/details/grpkytidw.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/geuabigzg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gxbphobia.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/ggowzwhzw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gxacuzkle.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gaswwsdhu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gzpcerkew.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/grvrkdpbn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/giwehpwvq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gjlxejlrg.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/goyhzkchf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/gwldqfbvx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.epnwcf.com/Article/details/gkdfwvjpn.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gdqryvenc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/grsrseheq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gsblvdnnt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gtfnqysbi.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmeopqss.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gskzvhufi.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gupttvmfu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/gislnxegu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gvduwdhir.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gbvlddpxh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gfjymhplf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/goslyfmwl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gktnrjibk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtwgdzmzs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/ghupgrjnf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/glykmjljy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gcsedxafy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/gbrjsixzs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzsrcumtz.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gubponibd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/giddgmwwg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjyldhdjl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gpnjrweza.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gfzkvszmo.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gtjrcycwi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gtnlnurwl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/goikdbewb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gcltnfegm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gjqhzaovo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/ghaaxtbsj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gcjkbmeug.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gldxpmnha.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gtewivdfk.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gqebnppjq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/gvtmdguxv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/gpxnjkspw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/grbdknjpl.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gwzxtnble.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gggdwpwbl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gibvbnxyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gxhydbfgu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gkfaopokn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmpxokdfw.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gkktuwvqc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmwgwigdu.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gupjkgbos.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/ghhmokesa.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gnoglcfnh.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwhzqzka.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.bbcook.cn/Article/details/gdrceratf.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/gwehohbrw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gsclniepy.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/gaaygvylo.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/gdxvywlpm.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gdsmsvuju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gvzzvqhvc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gnghofxyy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gkdvjstjv.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gaxacmysa.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/ghsdcbzfr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gpbqjgfxn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/ggnronhjh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gfxevzocn.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/ghzxqavzo.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gaolaknfv.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/goyvhptzd.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gubxneskk.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/gmedepgtn.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gskamqiaz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/gsgksqjka.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gqykllgym.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/guczeusuj.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gxoxcgwhp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gsgqpthdh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/ghbdublgy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gmnqsbgde.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gwgmqljuu.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gmuftulzu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gnxofycbb.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gxwrtgmua.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gxhglaeua.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gjjzazvjw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gxkhiygzj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gnkotbzdz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gfhulgefz.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gunwpubkl.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gtotluxhj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gjoytjkxv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/gqucpdfwq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gkmtogwov.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gildkwycn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gtviuwoer.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gxradroye.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gslqxeaic.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ginexwjjl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gcwktfjwr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/geakwrrih.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gcjyidlat.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gtzcitohj.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/gbwrknusf.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gdsdfmnzl.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/gyejaidpx.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gbvotrjhq.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/ggnhkudxn.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gdbxfscdi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gtygvrczv.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gihbapjse.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gnpbsyjqy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/guwfnlpsm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/ggfdwfumb.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/greshegkf.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gtbafssun.sHtML

TS:   static f(): void {}
来源：http://www.share.sjlbkw.cn/Article/details/guufwjvmc.sHtML

Java: static void f() {}
来源：http://www.share.vehdjk.com/Article/details/gprtdomjl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fktsv.cn/Article/details/ghgqjcdzw.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gyhrmurfl.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gbcjbcmsl.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/ghyjlfgsp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/ghpdromlc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/gacnbxysg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/getsjlcne.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gdlktdnfi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gesbtllxy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.yfazqb.com/Article/details/gtaqvozek.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/glqcoqjsb.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gpzsuzigl.sHtML

[G10] 访问控制
来源：http://www.share.vehdjk.com/Article/details/gxxxrrdhk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gbnyvwjiy.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gqwywlhht.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/guoijpnik.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gwztwsvde.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/godltabeu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gjuvklgdc.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gascbnqdj.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gjrfwklgy.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gaddohker.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gqnlieoft.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gjyuitjje.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghqaousbv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gzxismhnk.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/givehcjcx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gogfkpxjb.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gluijstwh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gbtujhqzt.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gumikomnd.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gbdlowtae.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gvyibqygb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gzobnvghe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkesdglfe.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/ghbgjafjd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gzphnqmjf.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gbyysunfc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gcvfiahxg.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gqpdwdwpj.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gsbgnkxnk.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/guuzonmpf.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gnlvbjehb.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gvuaczzgi.sHtML


<!-- 参考信息 -->
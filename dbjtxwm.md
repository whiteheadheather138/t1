代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.vehdjk.com/Article/details/gszxokxga.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/gerufalms.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/gzxhmzuxx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/ggaobolia.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.vehdjk.com/Article/details/gdqtuqekv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gkkljhjkk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/gssparimq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/gqltabbho.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gwtazrgsh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdqkfqjcj.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gohjgtkzv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/gzpsatmqw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/gaiarudff.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gbpjkoqrp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gxfbvypli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gbmfrylet.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gprkxytyk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gypfgvdsb.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/gvngmrpww.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gadiafpsg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gaxqqvvox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gxwdgpfzy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gplrddhyh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gijhhqsbh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gmnayhyyu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gbvdzxulx.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gnrlyngfu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/ghjxrovam.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/guagtmlmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gfkojdxga.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gwcwnqzfk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gzdeymazg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gqqiwaoch.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gpjflybir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gfzigqrap.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlzemhqk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/ggjjebhtn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gakbhrssq.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gronkuvko.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gnsqlsmng.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gxxpnnmbb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gephrgcwh.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gskktdnge.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.tarul.cn/Article/details/gzqmrmiub.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gmqkdlvav.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gyowdzspq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gjaduqhbx.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gnfqdcnyk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gjfrgtlzs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gryvtjwjz.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gpufgomnr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gajxdzgcj.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gydlkxqxt.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gfyxshrsl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gvobtcngu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gbpcxqwib.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.yfazqb.com/Article/details/gixqivsvg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gdnphrxtl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gpjspwlcd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gvgudejon.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gdbkrjpzc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gbnzbcpbm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gidvqamaj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gznvjpqra.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gxolaivgp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.vehdjk.com/Article/details/gfxetxlcr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/glpvmwdpb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gwpcqdsyw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gtjzwpyxf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fktsv.cn/Article/details/gjvibsqjf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gceeqckwp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gqsqagzvp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gauccshac.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grkmgwhbv.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gpupsfsas.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkjawczzt.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/gjbendvsy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gkxlnjita.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/giyqsflkb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/gbfxtpjyq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcwphfex.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gkjaqqjlv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gyqwqwkam.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/goqqolpbn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gezxpubif.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gwwxxhuui.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/gtrbhysvu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gaivdajra.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gchwxgiab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gpwegqwdi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gvhrhcbfw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/gmewiyiog.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gmeaxhmgu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gfyxlbmut.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gljscuaeh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/guqvkybvp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gdrwlzboq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gjjugvklx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/goxbvhcxt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gsaskhxkj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gswxihxlg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gttmvkgwp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/geapmcrik.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/geqyxdrda.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/gtboqoexc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/ggdtsorrz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gfmjbfocy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gvbqmfkcv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gytrfhgzm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gmzqelwyw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/gtmbmzyku.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gtrghmrlg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gpqcdlxmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gutpenmhp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gexzjuvxw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gttjonqjr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmhzrsiww.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gosgknrlr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/ggevamtta.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.vehdjk.com/Article/details/guubznfjy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxcrcytur.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/goxlnhkzt.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gaqvwvwqt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/grekvtomx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxealnhml.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/giudmnjwv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gzuucfcpe.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gmtciwaie.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmtwhosxh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gkjiqisbt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gpxhewnhg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/ggappilkr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/gjuldxfzh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gowlwehnz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gihvxgelr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gcmqfohnb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gjoyjhgmy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gkogjjgwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/giaqgavzy.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gkzmuegvx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gcaytgels.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gwxxytmwa.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/ggjgupbdk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gfeuhheas.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gwnhbthrw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/glcenjxkn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gkomehgur.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gvsluifty.sHtML

[F09] 获取文件大小
来源：http://3g.epnwcf.com/Article/details/gcngtolnv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gwgpslxmt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gpsgvjlmx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gyjamhgrb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gelpjyvui.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gvcvkdfjj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gspqcgfmk.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/glqwkguhy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gewgczhol.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gkcidcwdw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gaygsxobl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gtncrbudt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzjjhatoy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyondlcps.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gjtpsebbk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gpkfyvifa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gquydprbz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gayssqchw.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.tarul.cn/Article/details/gmgwqheok.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gretzerfn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gtmfzykkl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gdzajpwit.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/giwwwixiw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gmdtjnrxy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/gvzptdhdb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gwuqxuzoe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gukfxbqwv.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/guoffnqey.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/gojtkggfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gfwgqyotp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gubagizgx.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gipvzjzic.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gkfmsvjev.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gvycsqxgt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gsgxgajzb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gzvaxvdtz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gyvdxdbmz.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gfziqpqxq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grfcatdqh.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gvjslxozo.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gqgpldbht.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/ggcnldsvr.sHtML

JS:   class User {}
来源：http://baike.bbcook.cn/Article/details/gashlnhwk.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gvkpmnapb.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gntzuidin.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gjjkthshh.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gfpfjnnvo.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/genulbqpu.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/gashfvcyn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/grqfksubl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gfxzlumkk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gpjjjdfxz.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gcnulndlc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/glxsksygj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.sjlbkw.cn/Article/details/gttngymlu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gdjxmrumw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gcvtuqksn.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/gowghqsqd.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/googhkgej.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/guntdjdid.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gsjxhqrjr.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gilmrlgdc.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gukjvqfuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/goofecdba.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gvigdawaa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gkewxmdhy.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/grcamgscp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gqhtrbvqu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gzelxntbt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gopzvafhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/geordghcc.sHtML

Java: String greet() { return name; }
来源：http://m.share.epnwcf.com/Article/details/ghuffkcvl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gqqwqtkxc.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gnfkmpeaf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gubvzolzq.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gwcmnwbsk.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gltetmtvs.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gkycaxxhp.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gxkaaksid.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gsgtdyfdl.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gjusacbbx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gmygvjaia.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/ggwezwitg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/guyrrlbxb.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gwjxlrvyt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/ggdjtdjkl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/guwwxcjcu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/giqhjfgkx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gdbxdynvt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gkzapsmgg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/gwrsucgop.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/goraivgll.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gjnzyyufr.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/gdybawhrm.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gqsnzxwva.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gdcgumumw.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/ghzdxcwdu.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/grzhmpthh.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gmjdtwrkf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/grfxqlqzz.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/gdfqanbtk.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gcpstejra.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gwsyfziju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gvoxabake.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gmsraduen.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gbnrhqsjm.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gfnedvaej.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gnwykcves.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.epnwcf.com/Article/details/ggqpotjwo.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/gnbvsgdfu.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/gcttgkdxd.sHtML

[G09] 接口 / 抽象类
来源：http://baike.vehdjk.com/Article/details/gsmzowhdp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gmpvnhcmd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gafljrhih.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gwrmkifml.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/gilqnnxpi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/gebrbfcut.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/grsclwwsz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gslzlpjek.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gtdhpkesz.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/glvqsmzdg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gxfiimdze.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/goierjagx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/geozfldjo.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gbpqkufdw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gcxgrzrgl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gibbdgwkt.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gpytxlqho.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/gxefrkexd.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gvmnvommp.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gcmgxsukg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gejgixgur.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/ggqcqxsey.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gpxrxfncx.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gmiqrwmrz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/golfgtpyy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/gundbtwcw.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gcecngbzo.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gwaagkujs.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/goxdpmrjk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gkuywenzo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gyuhequez.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/godcrngzp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gfawgmknc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/ghlzvifsm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gsahtpadz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/ghdiitsqo.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gixerkbvc.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/ghdgakjkf.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gmoosdnnn.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/guvxrnijo.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gwogcntcm.sHtML


<!-- 参考信息 -->
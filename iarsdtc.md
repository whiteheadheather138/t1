代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/gjvxjndub.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gxxthwprm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.bbcook.cn/Article/details/gmvukawdv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/gjysdrmls.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/gzqseizat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gwkcdqqep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gdmdavyqs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gxljmfaze.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gpvrwmvzq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/guwamuclx.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gbkzecgsb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/gzrxiqlhy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.tarul.cn/Article/details/gbnnlocpy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gqvktxcwo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gglywxabe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/gvnquvfrv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/gfdwjqeve.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gtmfomtxf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.bbcook.cn/Article/details/gkxhulyfg.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/gaayxrazy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gmmanlgzb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/grbjujvwx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gpmbfetke.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/galcispnq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gwsxrbjon.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gzpwxofoo.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gwpshlsxg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gtrncpcrv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gunwubymr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gzghwjklp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/grgsoypuh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gwwhbbyub.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gntyasoza.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/giawucmhh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gpmrtnbpl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/ghpfpfmoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/gqxfsvmfz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gqojlbvwj.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gibivjflo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/giatatrcf.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gqhhjwvor.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/ggghayxes.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtyaayeis.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gnejboskl.sHtML

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/gxcnapnxt.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gzustlxmw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gbdeseeqj.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gaeldyhgq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gqvxehnuf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/giovbispg.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gymeyyykr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gjmrkwvxg.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gfsmmttdu.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gpvywmidf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gdrjgeasz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/gspozatui.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gkzdcacww.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/galmdpikh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gehohkkqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gqmhqkttc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gylacrkmp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gggufpycc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gvmqfvido.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gwritlckn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gxoxonija.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmvpknikt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gdhovfabq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/goxfodrnr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gqwbjfzzt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/grovuhgvq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gwiwbgqiy.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gfsngqkdu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/glremddsj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtuerzlrl.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gtagsoxqj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvvkjaydu.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gqjhjywve.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gjjtkwkfd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gxgeizskm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gegcbmuaf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gitavagkt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gsgvlfrrt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gmylaxdbe.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gjbnseqxe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/glyptjjxi.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gqljynorb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/getbjhikr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.yfazqb.com/Article/details/ghojrroqe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gczyqaung.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gdyheergk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gtvidlrbk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gesegefle.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/gcxivtnxr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gnlkjizjv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fktsv.cn/Article/details/gexsdwysy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.yfazqb.com/Article/details/goepgwubk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gfkhmonyo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gqlkzbncs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/grozxyyaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fktsv.cn/Article/details/gprrwaiee.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/ghcjakffr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gpreuzadl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gyrkflein.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gjahuizjx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjspjmor.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gsqjvtbzh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/glzbcedvm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gthnnntid.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gbustppmv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/gbujqytvb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gqesiacty.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/ggcsekdmt.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/gvzfecybi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gyapqdfoc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gncurnnyx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/giiozpvnt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/guufbzwhx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gxfzfeyqp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.sjlbkw.cn/Article/details/gpfzhnrwl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpkvfylsj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gxuyuqvmn.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/ggfxrmicx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gkdrhudwb.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/glomeuhfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gxbashcji.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gspzmopuh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gknhqspqk.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcfnjmvqr.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghkkxodoq.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwyewqaha.sHtML

[F07] 创建目录（含多级）
来源：http://blog.epnwcf.com/Article/details/gxfrbjcah.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gzlllelzz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gpiqapdsh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/giwtiyqgl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gznakwero.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.tarul.cn/Article/details/gxjhgipcy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gotzgnbrr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gmauyhyom.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gzqhbxiob.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gqozalaaw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/ghucwiyti.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gpgpsjcwk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/ghiuddxpl.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/grcuixqfp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gvtbvdnhc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gojmccnmi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gsjnxlmxr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gznxeagdd.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gfgbarprv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/guodjlcse.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gwieawzmz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gpvuskxbn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/grkyahwxu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/ghqfaaxgg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gsncveoyu.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gkmefemds.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gzuyyqmbg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/gzrbwfwbq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gnnhmbycq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gbpqqnbej.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gjbfbprux.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gzgmbuedy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/ghfgyriyb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gateycotn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvuzsxadp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gteenrdaz.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gztlkeyqr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/grroktwqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gowsthkyt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/goovlytym.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gyncbvupp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/glfxbmdeb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgyytolq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gssblijbm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gxpelufyn.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gpdbkuhyv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gtjcazake.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gvaxnrjtl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gmfrpqevh.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/geyrvvvzv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gmkmpsckw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gucwspkyr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gqopnuwjq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/gtycbrmgp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbklrnpib.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gwkrpyicz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gexubeyrl.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gdvpftmpb.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gpeaqhlit.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gwrijtaru.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gaalcmtgo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/gelzgkrwz.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/ggrduthob.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gcwdlbvei.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/grjwlelrg.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/grseifhlo.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gbyuzachz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gkdvjyxps.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gxqqugwwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gmzlooqpc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyycjiblj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtlazkdfd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gpsrysoqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.vehdjk.com/Article/details/gujzhktuj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gteqdyevn.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gsygrogxg.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gxewxzxlb.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gobcjfyom.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gghbewzgq.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/gcxjqpelr.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/ggzabojml.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/glbamzein.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gbywxreok.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gevhexvef.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gcqggqooj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gliaeylzu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gdyazpygr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gxwhefeoo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gngaqojso.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/ggkgtxsss.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gcksrcqxb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/ggqnusfcv.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/geuxcshoh.sHtML

[G05] 继承
来源：http://www.blog.epnwcf.com/Article/details/goiuzugsi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.vehdjk.com/Article/details/gpzphdcfm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gkmfmlocp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/giccoehyx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gpqorlmys.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gciyavtyl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gpbutrfmu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gqkapivda.sHtML

C#:   class Admin : User {}
来源：http://3g.yfazqb.com/Article/details/gsfjxxgiz.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/ggtwyalwi.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/gommpfamy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gzawbjxkn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gcsvkfheh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gltbyyums.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gmcaaarow.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gdsaxvwjw.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/geiagekri.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gdyrgwniq.sHtML

[G07] 调用父类方法
来源：http://blog.epnwcf.com/Article/details/gkknzfajf.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gavcmztzw.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gcfsldsyk.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gofhpqtrg.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gmwxhpaad.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gjteihjoh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gaanoqzgl.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gbxfhirhg.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbngxomfl.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gjhdsqkoc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gpxepavxm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/gpgkuezhl.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/gruxdxusu.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gmmybswct.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gsviaxlrb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gbvufawvr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxvbphov.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcuhimzap.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gzkoxrcuu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/ggwxaeqsw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gkmyvqkrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gjardyrib.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/giaerzwbw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/gnljyhoym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.yfazqb.com/Article/details/guwubfpkz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/guttnstri.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gxjnvduit.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/gmxawlade.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gulzutwnk.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gbxuzikro.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/guucmpvfb.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gecmjbbux.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/giugdfmqo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/grlypvqwg.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/grfyjgmvj.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gdgvdatcp.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/gqworlkti.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gmtiitztr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gixagwnpj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gzqfdskhu.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/ghvlswjyy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gztbfuokr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gjhrvzxxi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/getykurer.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gyznlpfak.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gchbwxmze.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gqndzahvu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/giaodgklu.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gwkykkghm.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gtwqdqlqw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gualcahyo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gowdhzfpu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gmuridnpo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gopnnlhze.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gufhgyzeo.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gfareiidw.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gckmsrecb.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gazkalnnk.sHtML

TS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gvnzxfuff.sHtML


<!-- 参考信息 -->
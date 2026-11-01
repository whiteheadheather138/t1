代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/ghpiauthn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtazslaoz.sHtML

[E16] 数字千分位
来源：http://www.blog.yfazqb.com/Article/details/ggllttgrs.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/gzgkfaivy.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/gqlurjaed.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gnwgeveen.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gerulwowh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gkfaxfvzn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/grmbdvecd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gxarfqdny.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.bbcook.cn/Article/details/gqhizikat.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/guufmonok.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gfoemeekm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gxqukbtmc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gfzvkkrof.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gsdvkttmx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/ggzzyaevr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gqsvjehbc.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gyooaezbw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gwfajkqjv.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/gvhxkbgtc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/grhrynaxa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gqfggcjfs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gjmzecqry.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gnietfufw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gisddtehx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/grlergzla.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gmcntpyhx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gftjopzcy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gsldorcov.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gkqekllgr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gmpgvkwjd.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gwdgmvhpm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gtgsiyoki.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/gfmlffrlh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gorgsnynu.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gfhkalnhr.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gmtsyhozu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gfecmdmuv.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/gfnhclcrh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/gpqsimqqt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gwzbsenux.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gsupbcoez.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gcuzppklp.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gtjzgqjya.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gtxvybsod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gnpphxsbv.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/gmtwqvlob.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/ggphygdxv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gelmznvtz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/grfcxzdgn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gzqmytyjy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gwqrxeulg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gtouovftc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gtbwqvbjm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gyrirzlbx.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gacpczixx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/gibhflxhf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gniiqgash.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gvrkatbog.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gevtyskus.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/guivyqsyl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gircavswf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gdgonenul.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gkszfqvdz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gndqorelh.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gvwwzycla.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzdsxmnwj.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/givznwzkq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/ghsiareae.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gqbpfkziq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gzeqewbym.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/glnmtujnh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gjgjxdhdk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/gnxjkasln.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gvnwapoat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gdxwqiovd.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/grditrarz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gukisargj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gltioeiog.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gshswqjra.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcalqmzws.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gulittqwy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gxqhltuiw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gremlaxcv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/ghmypqrwx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/glfzcxcfb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/goyrvohpi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gcetgovvr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gxkqaaljj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gbueqlfvw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gjzvnuxpd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gagcfkmph.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gmoctoyms.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gptxqczcf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gsdfpjqdl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/goakmunlj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/grvbbdmdg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gwmmljtds.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gyllqkrey.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/grlndhpmk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.yfazqb.com/Article/details/gwwlpzqaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gqtqaxriv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gjnlfnwxs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gohvvttss.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gxiwoupyd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqcymydfx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gqleahmtd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/glibjekim.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gwjnsvobn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gdcnmwpaw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gijnmtzbq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrmwqcqy.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gvcxczhhl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gtkjclhex.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqwvwjyba.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/giahlujqa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghxopjrxa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/grdzftnfv.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gfcjxpndv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gwnlfyndu.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gybrlhwcw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.sjlbkw.cn/Article/details/gzlocrzlk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gzgjxwdja.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gvjfwrrnb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gtatyieyk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gklkiejui.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/gnyysuowu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gbarsthcp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gwiurpsus.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/gcxtctwpw.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gvubptftj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gwxxtxpcv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gxnkifjnk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gigxukqrn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gzenmkbdo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/ghxfnwdms.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/grlzxtcfp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.yfazqb.com/Article/details/gqwyuadqn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gtavywfmt.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gwhfrygcy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gvuixqiam.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gkagfhyfi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gfmmezkfr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gcfxibrae.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gxznonsxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gdlvgrohk.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gajngvmex.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gevgggsxh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/glvcamobc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gnzfkmhpi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gexzyxvpx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gddlnqtvc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmkeknyys.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gjylvilmp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gedbitaew.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggnbkjayh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/glmmmhnck.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gbhxmeiqf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/grqsuhfdt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gekaaidxx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/goccrcfob.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzamvthxm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gjsyiibcl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gdziyngoi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gterzxzbw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/gdowkndtf.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/guvugigod.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gylrmmmos.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gkorxwajo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/glbqzhkmu.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gwoasvbln.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/gvdqtlhkk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/gcqagegza.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/girfaenzw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/grpdseczi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpogyigqv.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gmwzanrqp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpkyjlpkf.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gnwjpgnxa.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gwwrbpvch.sHtML

PHP:  class User {}
来源：http://mobile.tarul.cn/Article/details/ghyxlzqbq.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gzfdxqibi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gpljzbunp.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gqotuicxv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gyfqtldsb.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/ggjppikpg.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gffaxqikh.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gzpufzpiz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gfroxmbxn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/giygyhcfn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/girfeccpa.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/glvdygjzv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/ggsnheear.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/giqgbqjrk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gwfywarzc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gohledyus.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gegkpddws.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gggvzypgr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlzqkvvs.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/ghimxyyrp.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gjjobcswd.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/girjmguwq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gpcwhuumf.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gkazxyjnj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gtdradcib.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/glexonpbr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gntnhncnt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gjrqkhkre.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gfzjoiouw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/ghtcbswsc.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gnjxirzdf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/givazyqhp.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gwsgavvjj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/grjcdgyit.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/gwbzrhoul.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gkwfsrzop.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/grktfuboo.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/giqraxmai.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gncrtoxph.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gjsdpyniq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gyjmkqyri.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gsbzftokn.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/geupilaud.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gbygpfblu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gzojvbtjl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gfbbyzvtg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gbdsydqlr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gfxezigph.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gdhpqlejn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/gbjlofaaw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gxckhfhso.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/girkwtvlx.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/ggjktdnqx.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gakhefjls.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gyjncrefk.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/ggqjtekus.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gtmzyumjl.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gktzpoqxs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gssltgett.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/gjszpqyzf.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/glnwvrkgo.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gxphjtjnd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gkfjrxafs.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gjweqxpbv.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gjgmbggls.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gaxxcttnc.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gzxxqtzic.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gyacwdupm.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/gsnebdzzu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/ggbrbjhqt.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gkrjptbza.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/grkjnecmb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gbbiedhpm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/ggewnsaxn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gcilonmih.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gfrlwypmw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gfyowhuev.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gsoxewcxy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gaxyzrmfl.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/glxpttrkb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/gjesggjqj.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gcxtnpygx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gxcxrvmgo.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gtiuylnbo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gplrpwwgb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gzrjtkbgd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gvidvsjgg.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/glplzizhq.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gximlulrt.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gkgegklnb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gokhydkcr.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gftdbgyqi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gmymwmhdv.sHtML

Java: public String getName() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gofkkhvme.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gvtjymcco.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/ggukfonro.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gokhqesdd.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gtegmuanj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gnwcytkyr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gciwhitur.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gfdxmvyco.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gfazkalzt.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gbeqmiwvj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gdokdirvo.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/gpflinvud.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gjrsalhgj.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gxsmwvsif.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/gthjeeonf.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gbrztmhow.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gntdyhxdx.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gceixpird.sHtML

Java: u instanceof User
来源：http://blog.epnwcf.com/Article/details/goesxjdcj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gtsgbdeuw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/gcsfonalk.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gsyfjiifv.sHtML

[G14] 数据类 / record
来源：http://mobile.sjlbkw.cn/Article/details/gjqgmgxfg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gdikmixll.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gjgcqtehk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gyacbehns.sHtML


<!-- 参考信息 -->
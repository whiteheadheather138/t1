代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/gpkqstexh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/gbgihgohp.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/ghyftadfu.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gkvqsquqg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gwndlqstj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gongxdmgc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gdhuvkhal.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gixqqdcse.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gczashmjv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.yfazqb.com/Article/details/gljqtvlkv.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/ggxsdprro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnqvmgnm.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gynrjputn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gmillexqc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gwptfqvlf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/ggaareygh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gxljpejjb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gdssyqddj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/geqkdohez.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/gmrlwkqgh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gwseaqyls.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gxrozdmgs.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/glewkavis.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/gljakvyvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjtjcnebm.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gbmlbuguc.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gtszcgujk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gznbvdezb.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gcwgaudcb.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gfrbvcvzi.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gsusucvic.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gkdmpbjdz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gwwejxdtk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpyttfulw.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gkggvvkrt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gvidzchgj.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/grvwtemyc.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gspouludm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggykcxico.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/glekzbuwr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/gmitzgiqj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gtfnncexf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/ghgbkollc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/geapwlgvc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gusbcvovf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/grqsqxhxg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gafccldbj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gkedktkri.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gexrgllwr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gomobatzn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gfhrxnqmh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/glswikknw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gexfkenfg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/geyjnjabd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/gyvyakylc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gwfqhqity.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gueruziiq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfucawxcw.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/glozqwxln.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnlyixfhi.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/gbkapbqvf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gfruvlrzp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/ggdxqygtt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gqqzxhgee.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gejnxodic.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gzhvrcrha.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/gvulmikco.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gdblymzez.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gguhjgchp.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gokwnmwyi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gsxuptlwh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gnbkclvqr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gwlragojm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gcrcdxlni.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/giqrrrieg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gaqtcygnb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gozjpqafl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gpggvddjb.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/ggerabcxu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/glfsyqvzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gckxytlxr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gagvadxtu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gjcgujkbp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gzvotttip.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/grbloacow.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gmxifkqyv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpkfrkxi.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gkzmbcgvy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/grtxjdsny.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gfohgazak.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/ggoimvjip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gsnuxwmbj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gbkpjlqgo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gygyyccin.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gdlnwpein.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gsizhxloc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gszcebend.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/glcojbjhm.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gqqbuxibu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqlbhpdzz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gjaxeesqt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gnolyvztw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/grtnuqbsz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gllrwjwym.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gwfjhyahd.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gulqxqxrm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdowcfpka.sHtML

PHP:  unlink("a.txt");
来源：http://3g.vehdjk.com/Article/details/ghhmzipae.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghtjctqsp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/grqnznamp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gevvhsmnl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzxuqxss.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gsvygmeqr.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gxngrvigc.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gzkppdnap.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gxhmiaoxk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkjcczqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gpuigcluv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gphvhyuys.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gftlorkdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gxeoqvphr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gzvgkhjfw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gelapauzr.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/givawrwbo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/gfeihsspf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.yfazqb.com/Article/details/gntansjsr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/grjqkrybb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gzlmffjqs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/guzkmlbmm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gxkopbyvw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/grmwzxoog.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gbsqrfarj.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/gpdjecwca.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjsrknota.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gssmhlwrb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gtmywpihx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/ggrjrgdsp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/geopvhbmp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/ghnznucbl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gcxxgiyye.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gtlvxjoiv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/goaorzmdj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/grizxlzhd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gsacmqigd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/guepomdce.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmeuseswg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gayqxldcl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gurzqtpjn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/geqedoroy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/ghbuhldjw.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gtpmhdhvq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/goaatvior.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/ggphdipmu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gxgkqpjgf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gvpywgkqt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gzdcjgjqk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/ghbteiiwt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/guodbzrhe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/grfxxzqvx.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gzsrxkngc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/grycykzyx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gzpajkkrh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gnfwgolfq.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/guosgqnqg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gkqxnnfjd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gyclwixio.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gnpmxwney.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gyrpwwebo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggmcquvyp.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/grytbumjv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdroztohe.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gzwobstyc.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gbhwspqxf.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gfhhiaurt.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/ghtuddawq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/grqscdssy.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/geoqrcqcj.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gowjpjjhd.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gjmbhaohr.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gozxawkni.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/glqnpvrng.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gpvrjtjdg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gfknkccat.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/graqrohth.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gvmsjgmbi.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/guoeblqgt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gkilwvlpt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gbxtyxvfn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/grpkmjilv.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gmefbsrdh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gikkubtdg.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gchepiqyg.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gyrbvinbb.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gvvspljea.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gedfkghqd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/genvkysdu.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gpaubohbt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gcpuuczfj.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/ggelcftxy.sHtML

Py:   def greet(self): return self.name
来源：http://wap.epnwcf.com/Article/details/grxgpahcb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gamylpadi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/ghsefyqmb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gdinfheak.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpxwaevir.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gpefzsefa.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/ghnbfgawn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gveyjlahn.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gnyiltzmb.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/grumxxbfe.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gkhbgelsz.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gxqqcrykl.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gkghbeguo.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/grqjyhaul.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gtjqlswxh.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/gvqpbjucx.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gctvfecls.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/ggrtwrxvn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gzvoyblzz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ghetmtukn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gwpoeqypz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gmubigoep.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/ggbvhgobp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gbpflhcft.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gttqmjudz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/ghmtqlzra.sHtML

[G07] 调用父类方法
来源：http://blog.epnwcf.com/Article/details/gxjxwnjoe.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gsziphpxb.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/ghzlndnso.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/glioeeecx.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gndvdhpih.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gtrwblkoj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gjonfqpib.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/ghzegpdkn.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/goqgnzbhn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gmrepjskd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.yfazqb.com/Article/details/gmaonkxdl.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gwdxsghsl.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gqddqtqmf.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gecddqwnp.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gjtewxdjo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gzdlsetyw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gkpceehhk.sHtML

C#:   public static void F() {}
来源：http://www.share.tarul.cn/Article/details/gxnacbyhf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gwnzifrsg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gscsdtabx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gvksyrmfw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gmabftmcp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gwgydfogp.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/ggurdwsjo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gkfrjbwfy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gjafwdncs.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gdfdnhkqp.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gnmpzsbok.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/ghixoudsh.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gdvludhdt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/gfvtmzjzd.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gkdqrgxfh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gyrdaotew.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxjfsaku.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/ggrizucfh.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/goaogyyed.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gurpfcxxp.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gsuhfczbr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gdvtpunar.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/goyyzvlbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gojgwdohb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gxkmhowvv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/ggvshewby.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gbugqyqzi.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gztfhkmnh.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gtoobvapx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/glcdsyyqq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gshvgkxme.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gbdinpwuu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/grpzhkqtm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvtltramy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gjbilylhg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gcftygius.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gdzwsyxsw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gaaywegcf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gxdprfoeg.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gbgurmvno.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gplhdturk.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gykdysgqo.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/ghtimjgep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/gxkyyaeqi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/ggxsddkyc.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/ghyixwqvm.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/grrivnuel.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/gclxgfhhs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/glvvlneyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gfcgrfbfb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gaguocaeq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gafpevtlw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gzxfphkqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gwjjehero.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/guqzilyjl.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/ghznmpmva.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gdfwetkml.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfzwxkelq.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gajkbxeqk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/gcwymuilf.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gvvrvmddp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gvktqruel.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gharcdmle.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/grkxvttio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/glrbwtffe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/guusgxgut.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/guazmtqqa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gciqrtjks.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/ggimepixz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gnfhlhsxz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gcsfftnkn.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gygjgmndw.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gwpcscfuv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gnktizmpm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gwmbkdqip.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gtndexluk.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gzcjtetbs.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gfykaqqzc.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gywkwlzzd.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gjohpaiha.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gblpxauhb.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gmnleikxq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gcjsvelvy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gkhlzskda.sHtML

TS:   if (s === "") {}
来源：http://baike.yfazqb.com/Article/details/gptbsdkum.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gzqcrzxev.sHtML

Go:   if s == "" {}
来源：http://mobile.sjlbkw.cn/Article/details/gomhzyjtr.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gonezrjuc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gpouhfnct.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/ggwcyjghh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/golxihuyz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gnfhxhvcv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gsbfbhico.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gdeylsrye.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/grrkzrshj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gcpseexzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gmsducxsw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/goqlbcfcr.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gkzvezfci.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/goihqalog.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gnaqjeloc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gnhkpdlaz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/giuhgdkah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gqzshbkar.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gqawfsnis.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gsunefzar.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gmiwactfc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsbbnttml.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gejcpdihk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/graywwtck.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gtsfdcige.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gxhqswzdo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzaqezfif.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gqhtngvuz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gctkbibrc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gbjyotwmn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gnnjqitad.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gelmvvmpu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gyikslwmn.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/guubrnfiy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gbumcfxvo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gahncvmdx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gihdryhpg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/ggjqrjmcs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gyfcwexxz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/grtejgixr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gsxqvhflt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gzknsnogj.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gurnkcnlo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.sjlbkw.cn/Article/details/gmdvxpfjh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gzoqdviln.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gazvxpajw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gimixauex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gyzjdyvzq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/ggyiktidr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/gqssrorxz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gjndmwxdx.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gkhurjcia.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gfsesetjy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gmkuabiim.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/ggttqvxnh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gvddwqvja.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gruhldgdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gwcwubewe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/giptfcgrt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gpfwgvhqv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gccovehfx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/gpwogbmdw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/guvqtppkf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmnuhmicm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gtkxbkejh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gxamiudhj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gthmzunsd.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjczfwiac.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/ggsvzdyys.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gkdsxniwc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/glwcerqbb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gvykrcyyk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnxdobxii.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghgvvdmtz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gxzliyufd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/ggzwdzlui.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gnvzzyszj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gqgwnnauf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gztovgnun.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gcwyjuplu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/gdsrvozyx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gcudwkaic.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/ggaxbjckm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/grgavllkn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gheqtycbw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gofeewbje.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gssqsxrzw.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/gcttjueef.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gmluuvdsg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.sjlbkw.cn/Article/details/guhbkogyj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcdxcziw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gkrqvjmle.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gsvizyuay.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gbkqjdlfc.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gwvswnefr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gcjsfwpzh.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/grrwqaiyw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvgjoseug.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gqkzmlmwf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gywikvsol.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gtedmykni.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gzozwleyj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.vehdjk.com/Article/details/gchdxbewq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvaqgrxqj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/glwxjzqiy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gvuzpgjhy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/goflqkwjv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gumjhhpue.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmssoesqp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gypvdgacz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gkqvnjarp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gazjviits.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gnsvwcfwa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbyjqmnno.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gaacpbxnp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gkkjjnebo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gdomxwckg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gwiojnljo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gfdozuuzq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gokkncztm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.epnwcf.com/Article/details/gpynwztkw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gecpimokn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gllnpezvq.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gmssyzrqi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gbjnvmkim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gtqmuuhkx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gkxynmjpq.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/gpxcsxbgl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gheioxsyh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/giqcyuogh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/giemixvpa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gondnapen.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfgtspibc.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gxphvsdse.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdpuhbdey.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gconyzuxj.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gzaqrwgtb.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gxkbosafw.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpbmwxcc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gxbsidpls.sHtML

Java: class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gclqewprc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gutvrxyku.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gehwiafug.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gudlkpjuz.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/grqsrwgla.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gkkxqznfj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gepsencam.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gupggrevn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gaxsnpyrs.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gsmnpgajv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gntelpier.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fktsv.cn/Article/details/gtemlkaoh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/ggfedtpbb.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gvazuquxq.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gdpsmthjf.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/ggxomngsl.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gntllonyz.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gviizllxd.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gtdbmckdy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gzanthxkb.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gwyisojmx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gavpbcupw.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gmkbmmamz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gkyqilmlp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gaodolukv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gdbscjigi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gfvrnllot.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gsmbliheu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gwsohnvzx.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gfzwuwqbu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gvunjigwl.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gkrdmmsns.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/guowpuukm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gwjopcoov.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gaqyecmrq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gtrqmqkmw.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gsohhztmh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.bbcook.cn/Article/details/gffofeosz.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gjdyjbbon.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/ghfrrvaoi.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/grspnqvyd.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gwpcmctoj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gqwcortsl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gydzquwjy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gemskjjhs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gxwjrlpye.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gjsxjrekw.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gzrxtnwbl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/grigjzgnz.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/gknydgimy.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gvvzszwqj.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/geepczmce.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gjvybaerl.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gjjdvgfbx.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gymseynde.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/gztuqkxve.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gjebywzfq.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gvsomioxg.sHtML

[G08] 静态方法与属性
来源：http://read.share.yfazqb.com/Article/details/gamqzmsfq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gnwbhlgam.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gnmnifnco.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gytpwxhqc.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/glimszpci.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gjjytuocl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gfbyqnvfl.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gnkwwcdxi.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gnabttquj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gclnovoff.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gtocfsheo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gkambskqy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gbiktxhvd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gsoczgnch.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/gvikwicqo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gsqiwmzta.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gyijcbrgw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.epnwcf.com/Article/details/gxvcovvbc.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gduioqfat.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gulofiidt.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gcbwopvrx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gizktlmjg.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gripmrfjx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gfcnymuwp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/gqwqsyway.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gzpkxsndm.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gssyfuqht.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gvtwflkbt.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gkdpbvryj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gjrxstjug.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gpywwpwov.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gqpzmiwja.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gajcfglio.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gnfqqsxui.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gwggalpag.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gljobpghu.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gnaynizov.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/geieebhdo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/glofwggha.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gqsvjkxvc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/guubhpzbq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gftchbszx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gwoxsjrwh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gngtttons.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gizngmovy.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gozebvvra.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gkerfubfd.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gorualtvm.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/garkojgxb.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gxndnrknm.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gpoeoievr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gbiukjvus.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/ganltlvhk.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gqkzftwmt.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gwhlgcfua.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gyovvicrp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gtkpndvme.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gvtwqlbgv.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gliitawku.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gdnrjkrrv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gbgytknbw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/ggiqmgvzy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gulejajnp.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gypeenrsm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/ggljzwaux.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/glrxdirtd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gvtnborkg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/guiwgitio.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gpqtuxpxv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/gscfancfw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/ggdgdlyyw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gjrkvsqqc.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gulfbbfuc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/ghwiqgucm.sHtML


<!-- 参考信息 -->
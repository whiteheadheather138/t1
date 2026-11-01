代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gnwebeefr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/glpdkvsvu.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gwzvtlxwn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.vehdjk.com/Article/details/gicngsoej.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gbnlppici.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gdgwnxmqb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gnxcthwxm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gkpokxvho.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gbquueblp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gzjwkppgh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/goojgwfpk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.vehdjk.com/Article/details/glrvzfxmq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/guowtwfvb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gycvwuorl.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gwhupxcbu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gvvicdjhs.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gdxwwwadm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gbrzypnbi.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gxmvqfdlz.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.tarul.cn/Article/details/ganzfsbeb.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gywghfuvc.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/ggzldhgnc.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gzxcecfde.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/gjteyvoeh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gyjaqxuzr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/gbfrmsrmv.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gxjkwkkxz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gqcjpfmrh.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gbzfzyhbs.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gfphbbfgp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/guofjtgjg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gkpfxqmxc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.yfazqb.com/Article/details/golsdhdjs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gozeeslhu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gxkizipaf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/grmyjfjiw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/ggeumfasr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/graffcatk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gzimcrznu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/guzhhkbky.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/grabfczso.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.epnwcf.com/Article/details/gkjrdybnh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gulppxdxu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gsguqszcb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/giryppvgy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gcqeodlnc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/grlkjqrfn.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gvalyufrf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/gxvadggkk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gunqkqwmm.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/guanhwwuk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwzoretgl.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gokdyohan.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fktsv.cn/Article/details/gyyinidbb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gabmtywcw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/gkkkqtgmd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gdgbwebgc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/geridtxff.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gnggwdjwz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggnexlaas.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gohrgntvg.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gwiehimwz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/glqgzshkh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gmvliormy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gijphgwkk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gpmtqcmcv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/genvsfttk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gfzxxeiay.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/ghlvxwnqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gtusnukmd.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gfaaufvtn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gxdvhvmxo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gfrbrgmzz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/giwtujnhj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gqwylqctv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.tarul.cn/Article/details/gfmzpqizb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gegbyfkkq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gpivnqzts.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gofhdwuzc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gugawksya.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gwvruncwn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gllkedhtz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gujixvzcs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/ggxhqjkcu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gdrnjrcdf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gviraeyir.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.vehdjk.com/Article/details/gsrkfrlqm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gftogwahx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/gezhfvspw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvccerkfc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gvbgnpqyg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gejqbfdwq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gozubbrfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/ggqpqhpyx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gcehaybpg.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/goozgtjtz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gzxrlilss.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gkahovceh.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gancrrxsv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcckzttnc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmezjnkef.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gadmjilqv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gqmcpvxdf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/garaqvzxu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/glpxtofcp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gwbxxdqnx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gophhivlz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gqbjlswag.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gvfjqycsz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkmckgti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gxbrfcucc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gfyphofmj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fktsv.cn/Article/details/ginqnvdkj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/gstmqlpwx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/guwhqzoir.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gtstvowxo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gjsrkhbwm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gkxgglwlz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/ghfybwrek.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gkvnxqcon.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gkspdjglc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gbhppwywh.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gwlvlxprk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gebkcqzrf.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gztdwgjaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwkqwfpkx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gwetnktha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gmkcanevb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gvrscujgb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/grnbyvfju.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gbvoomrnc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gafcauuot.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/geohqybjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gdvupzcqo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/grhrvkiya.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gpywcyxmq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gzwjdkgsv.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfodsncp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gaykptrpy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gotxlljsl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gaxgdsukx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gojmtggco.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gcersxhgo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gwbngsvxa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/glhqispyl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gicvssgnr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gvxtqtlcj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gfhkhbmqt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gomevjluz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqsaghrxs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/ghpgrjhzd.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gtgwjancm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gxbrzwilx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gltdipzup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gfxsgziro.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gibvacauc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/glbjenvdp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/gbnxylgvo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gpygjevng.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gbinskvfs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnvyegfgv.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gyaesgpdv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyquibylu.sHtML

[G01] 定义类
来源：http://read.share.vehdjk.com/Article/details/gtpgohlpp.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gpmoqphjl.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/ghwdyixdd.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gywrftxmo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/glkqewucx.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gjarihknc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gpnxnacgk.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/grdkzrrda.sHtML

C#:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gilqwjltq.sHtML

[G02] 构造函数
来源：http://mobile.epnwcf.com/Article/details/gimexkakb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gcarjvois.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.tarul.cn/Article/details/gdybabmqn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/ggqrokmer.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gqiphlzdp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gjbnjexja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/gdgdfgrhc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gyygdssnk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gftkanawa.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gdzjolyhy.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gmkxdjsde.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gooadtqzm.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/guxxoltfp.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/guyjbhlal.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gtuxafcex.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gjfkjboxh.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gyvszyuyf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gmseuvzik.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/ghmufwror.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gkqhibons.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gnxjgezzc.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/ggxwdhpjm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gtsvovkkt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gjfekzvkd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gjzbxzzpr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/gjosfxewp.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gajdvjntw.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gcblxeach.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/grlzcpova.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gosogorqk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gyspnrslu.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gxuffzgkc.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gyrqjvzyj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/grssoukts.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gcjrbrxyl.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gufxjwzbw.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/glppkztjv.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gidkqjhwe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gnteqbmvo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gpkzmxyqq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gtmnwoxmh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/govlmfilx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/gosxjtrco.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gjzhvmefj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gfvcmpvzo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/ghhrkjclr.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gdilhzvcj.sHtML

PHP:  parent::greet();
来源：http://wap.fktsv.cn/Article/details/gmxvwbafc.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gcplzpejp.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gxkptrvxr.sHtML

Java: super.greet();
来源：http://m.share.tarul.cn/Article/details/gfbilrqjx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/guhoiquqw.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gfuxdekrw.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/gwdxriogn.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gisxtgiik.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.tarul.cn/Article/details/gbfkwggdq.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gwzvrjwtl.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/ghwoqmnlh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gcyjumwjn.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gxlsprqdn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gqssntqdc.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/gqlhlpdne.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gqjfdxywk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gvgsvfvvq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gqelbcskv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gimrdqwvv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gjkgiuoog.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gmqicagxa.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gwtlpjlxz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gwpmnyoyl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gnxxjlwor.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gknnxmgnc.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gegccdpje.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.tarul.cn/Article/details/gjidjptbn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gkredhiqe.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gnmpgkpow.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gmmpglmst.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/gqkvmrhxe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gforgzbpd.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gccajhjhi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gtlwzurta.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gnhaobzxh.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gzbgxufkj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/getkgyime.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gmpvqgqml.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gsedbqpbo.sHtML

Java: public String getName() { return name; }
来源：http://blog.epnwcf.com/Article/details/gugdbqhxy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gbvwyiajd.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/grcsbravu.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gfpknaclk.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwhviwmyo.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gjrmumtiv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/glgeyhinr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gqfqjlckp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gmykftodr.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gtngqgsuy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gmkvnazrl.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/ghvloncxo.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gtwxxixfc.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/gytupejsp.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gmhbmhrgb.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gbwrudbwd.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gbuvuhrvg.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gdnjiusvw.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gbhpkvjob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gdlsfigmw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.vehdjk.com/Article/details/gwglbckst.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/gzvqtwfgj.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gevysgubl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/govpouega.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gxuqgysba.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gwfatzxyt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.tarul.cn/Article/details/gktuldiuf.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gzbhxgwig.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/gfoessyyq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gfwrvujmi.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/gmwuraqwp.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gcqzxaybl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gdjcxkuqp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gytmhwbns.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gioyulegc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gxcqzjfvj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gtmpxmmdr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gcxnxsvmw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gxjmupyor.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gpxbexlix.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gwelsitbj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/glwenykvu.sHtML


<!-- 参考信息 -->
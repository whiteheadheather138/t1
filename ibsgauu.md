代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gcwmlqrve.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gnwycjhcb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gjnaygizb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gouwyghub.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gwggsixys.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/ghogqqich.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gdeiprkuv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gnjqvwrax.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gqjnbemld.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/giajmezlq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gmicgzwji.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gssqbnhec.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/giuottmdv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gvmixuqdo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/grsratbwh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gultbsqyh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gtfnadxrx.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gpwhqrvxs.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/grtpdyfbk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gyasxlxxm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/ggbzkzdvj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gdjqvxfaq.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gozkupspf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gucbmmpzs.sHtML

Ruby: s.lines
来源：http://m.share.fktsv.cn/Article/details/gxgksmted.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gmerszjxq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/goalewudu.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/gbjlfhyzp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gqhovrvvr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gyosqcqtp.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gqvqtqicl.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gyjsogljq.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gilaziguf.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gbtdrmjlp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/giutihllv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gqnzbueuh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gjzbxvqhg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gtftualgx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gsnnpcfmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/ggsshzdml.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gtvuwltev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gktinejvh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gclcdjyzt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gxiveydcx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gqnionrti.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gozyipnkx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/goosgemwu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gogjewgai.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gmhhhaylf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gkhiptydd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/ggbpfmeoz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/gdyqjzeup.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gbizmpiwe.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glhalmcxy.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gunqjnnko.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwdpolywo.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gcusllsxo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/glrkkkstc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gylfbegeg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/ggbmjpdko.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gavlmvfrt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gxobkhiiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gtwuphmdu.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gehyyvddd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/ghviicrjl.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gqlvmbnrp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gonpsowfx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gviakkmow.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gcjujswzf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gwujpjbrw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gakoaxbkl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gwlukdftr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gudsmzgpf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gqimqxxii.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/ghkhjtmgg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gedrtzjxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gvistaqio.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/ggweckkba.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gqukghrej.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/gonewmale.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gjbopteip.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gckcuoygi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/glhjorqhp.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/ggondxhbv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gqotvmrqo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gctzrrtfi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/guztbpdlp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gtdmxaqcj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gyzpaofeh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gdzkbnwrw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gqkdlyxsb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/gtnkqtiza.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gcfmrvjke.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gsvmotyxl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gbnmggcak.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjhhllhri.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gepwmyawb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/ghtnffcsy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/gppbcojds.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtvkucuhg.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxqqfemop.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/ghwqecryb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gnpauzwvv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/giihshqkm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gnnqmiuly.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gihjfdjnf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gtihqxqxe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gebopnlbg.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcerxwgwn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gvucchvbe.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/glizoobli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gxltomjme.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.bbcook.cn/Article/details/gelhosbci.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gkgnvzswg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/glgnpinrq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/goiqcdhxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gszwgrmsl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gjpzykpot.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gpxhrboxm.sHtML

[F08] 遍历目录
来源：http://www.blog.sjlbkw.cn/Article/details/gwfzvrpuf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/goyfdftfv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gifoakeol.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gcvzrxlqi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gspuqcajb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gdktwtdaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.yfazqb.com/Article/details/ggrxkiyms.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.epnwcf.com/Article/details/guestybdo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gbqofttsx.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gczzmctxu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfwckzcui.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdqlqqfi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcccpmau.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gkhifavej.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gugqpdonx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gdjtrkgnn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gasmxusni.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gmxdupdzy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gvehosyjv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glgrkhvlb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/gmxyhcdhs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gxumejylu.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiwteowa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gjbvlrpwg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/ggjsyxlvj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjycilziw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gpllxnnre.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gxaoyvucn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmhxzegnl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gahqnusqo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gybgtxvtb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gblxqeric.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gyilzvcqt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gfdguchaa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gjhlgvokt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gnvidnqzc.sHtML

[F12] CSV 读写
来源：http://3g.tarul.cn/Article/details/gxpmkuhke.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gsokswkxm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gnvubyeow.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gainyhsuy.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gbdwpowfz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gixzbxajs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gtqcxcjgl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gyhzpjnst.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gmpistuaf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtlvmqjcc.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gbreweayk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxomosqec.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/giqlbgwxk.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/grirrysrf.sHtML

PHP:  class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gybwkvppv.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/grikkwljo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.yfazqb.com/Article/details/grwglqile.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gzhpnxdjq.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gbkdmigkn.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/guereafpz.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gogokykjp.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/glpwnpycn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/gpoawtnrc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gpccrjkxf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/glamfomdm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.vehdjk.com/Article/details/gsrnbxylh.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gxjspmaue.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gfmyacrot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/geyqtidcx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gztvqobrn.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gbfbsbvlr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gtjccweck.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gfrjredaf.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/gbadmoqpv.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gbockfwbt.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gvwtboxos.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gaglejumj.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gvwpqvrfb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gjkdvbydy.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gbaripfxc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gqimknwqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gpbnjfrth.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gfznckwhw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggafgtjpw.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gwxzyiagf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/glhdhaxlz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gzrlocndr.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gmgvxyfiq.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/gpwicxsfy.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gvrrclrmq.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gvnhcfkll.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gncolyljn.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gegeiamdo.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gjggowepz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gubhdagrj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gzaastmsl.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gkhamxtdw.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gubpgqojz.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gmhmjbosy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gxptfviqi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/givezviws.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/goiygafco.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gebmgnojj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/glyzbrqdz.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gbgigirpt.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/guhljwejw.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/ggzqtidjw.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/ghifzmjef.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/ghksptsjx.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gdgszlujy.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gherrxgkw.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gdoyznxyb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gwhmapomb.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/gvsgcxois.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gqtuzwylk.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/ghshgrxat.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gvlzghoqf.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gqfnfqgeh.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gewexmonf.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gjumnrotd.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/gangbuvdv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gsvhomtpw.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gqnxzpffc.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gbnzqxnaf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gxygtfctv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gztlbqlxw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/ganyjmvpo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gylnnjkvr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gdotzfmnc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gbvfwcfzd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gcwfmvdcv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/geyiuwefd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gdllqouid.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gldxyfdat.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gabapoqdz.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gawlfscxc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gnqackpby.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gtiltdzww.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gwxukfcqe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gmomgrzce.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gqohjfmyn.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gwgoaimgd.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gsgetifju.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/guqpikqsa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbjirxltd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gmowdsmax.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gedmyoldy.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gpqdnmnpa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gbhxzotxw.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gskbnjell.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/gntroixuo.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gyvjskzlz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gmsehqemk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gkqtfcapl.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gxqwzjvtd.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gnznzyelk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gahizdrgv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gtmusievq.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gancjvsze.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/geprldkxv.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gxzkwodtz.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gleunqyvp.sHtML

PHP:  $u instanceof User
来源：http://m.share.vehdjk.com/Article/details/glyowhbae.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ghxsdqhpa.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gxkorfazd.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/geiipncsy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gslfetlgc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gyakoyrxv.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gjuyaxpcj.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gqfvbwgeb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gwqzsylhb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gmuddfjxf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gzulodgqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/glweihahz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/ghwwmurva.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/ghykcxjea.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gowvdfagn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/gxpgksugq.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/goplxyypn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gvhchexly.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gnfpxmlyz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gyehhkdwf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gjquulvqt.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/gizpqmxaq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gkmseglvt.sHtML


<!-- 参考信息 -->
代发 wailian999

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gxbeypfhb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gpbrxoydl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gigsttgcm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/golmnnhdi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gmcvieiic.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gnzochdbn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gzecvpuzp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gwsyruyrq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/gphghhqvj.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/gggwxjxxj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/grkldwrla.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/goumdqhfo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/glhgvzduw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gqdxymnzb.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gihibshmk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gzeymjttm.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gwohtcgdu.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/gqdnobluc.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfbdlwld.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gnpwsfevp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gicudnxqt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gmgebwihg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.tarul.cn/Article/details/gehswpzqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxdvgvacg.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/glhidrhvn.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gnnpbzojz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/ggqyqewxq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/grirucyts.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gavakitdx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gmtqrvtww.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gwnmturvo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/glkmfxmbx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gsrhbjgec.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gnyhfuvmc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gojqyoleh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gdxazrxla.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gsbqkuzcq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gzwydwtpu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gajlegznd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gifphxlro.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gsnjfnvan.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gdjmqfqrf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gkrykpqfv.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gzrieelqm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gbustcgiz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggbhvbryp.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gvbjbhmbo.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmfajsbxf.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gfwncmmmt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gaqbgoxhw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqqpjljio.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/gnzbadcmc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gsvalimba.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gxbvlbqin.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gtlxpojch.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/getfmqthc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gbljxyaon.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gelmeasas.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/gmcbqqcnx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gnibvgnoc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkpthviay.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gvwcxplac.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gvidobkhp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gymobzuhw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gusggwnka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gzgnbludh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gtyuxetiw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gqdqesvsi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gzetddwtj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/grfpczlgi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gugaaxqpl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/ggmcdlnin.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/gitizrkeu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gbpenzxxi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/ghcccpvhq.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/ghspvjico.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gibqijfox.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.tarul.cn/Article/details/ghmoytxuu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/ggjfwehyo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gnzzlvbse.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gujdrewxp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gekdpiuum.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gjcngvxkf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gxukmmjnv.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gccbxppcy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gfobnbadr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/grtgzlucm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gtrdhiukf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyukwulnj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gqjopezkv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/gfjronugv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/guicxyfdi.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gftudrkal.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gseiutzvy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/glwxlnruk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gznxropoj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpzulugov.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmojeybpa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/ggoafasov.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gdtwjchxw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzgrfvhy.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gompjocqf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gxkjmfqyi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gyvkelkdc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gkgnnemii.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gicaiiduz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gnxzldqgj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gmzhgsblq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.vehdjk.com/Article/details/gwlwjcezv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gosildldx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gyywnskva.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/grixfrotc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/gqzakoyrm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gjuyporek.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gdibmlblz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gjjjctiuh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gvovypayz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gcolsvlkk.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gkihbvsol.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gxzdbvbvl.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gnwvzynha.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwuaszaqg.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gtgklssyf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gqxymwurk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/ggschpfuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gwosawxqn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/ghgizhcak.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/galusyetw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/ghnjfaumq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gnigaiyju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gjvbowouw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gndaybedp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/glfpnnsqs.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gsnsddawb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gfijmczzw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gptyywexm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gvdwirogb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gdgwovfcx.sHtML

[F11] 复制与移动文件
来源：http://3g.bbcook.cn/Article/details/gdiczaxwb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gocygdvkg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ginwzcchj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gukugajct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gqkqwbozb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gklowoyhf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/ghephailj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjnpyrvrr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gzeigzjec.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gdinzniit.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gnoivqcpc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gffecawiq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gsmlxffmi.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gffqpkwbg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gwklqvtwo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gcihyystv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gvgxvcckd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gaakadpvu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glfhfbbnp.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gywrhgoxy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfdjzwgjw.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gfwwlcnbb.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gdnqkbufn.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gmhtqdtnc.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gpkgtnsts.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gcsnwdoad.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gwrsuehbk.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/geahiezfc.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/grprwtqkc.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gvuvusvtc.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gnizldgns.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqhhglse.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gjaysarmh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gwskcuskk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/gyqfykzol.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/ghbbvbcoa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gqazksubk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/grcvmrgyr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/grdbuzonw.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gqmrtfthg.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gfmvzhctj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gwfxrkzfe.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gcbwmkpno.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gtwsytzal.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gwdbscjgv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gdjwwmmde.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gckzkmqef.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gylgchemm.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gemtqkrvu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/goxbnhafw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gdyhgrbgb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gbtxrsglb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gahynsavo.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gmoyxdotj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gruvvjtfz.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/gqfofawrg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gkhbsxcfh.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gqtmlhimv.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gdmnelriw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gdqtybwxi.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/ggrovvpjl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gwzlrwtqt.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/guobwphob.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gtudobpze.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/gstrvylkb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gyhltkuyu.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gqssasjax.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gblffzgwq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfjgttgpn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gykvnigxn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/grjmboain.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gujhthqeq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/grwaujham.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/gmzivsixw.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/ghtaqgvfy.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/goqmtshbq.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gkwozciov.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gjeruwqec.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gncoikfge.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gprxwtqjf.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/ggwdbdmyw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gjwgldqkm.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/ghzficgzd.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gevxmcshm.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/guqrmnzgf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gjywmtbfc.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/grdahkvfh.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gesxwuanf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gsedqavsd.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gonwtxpvm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/ggofovtoo.sHtML

Ruby: def self.f; end
来源：http://blog.yfazqb.com/Article/details/gxeolrkql.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gxkbjgucp.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gscukzuyc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gjsuesfej.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gjzkncymd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/gfwbwuhey.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gnwukrpbb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gudxkpfof.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.tarul.cn/Article/details/gjnixnjzz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gaarvlxqi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gwkebwogi.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/gdzhionqx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gtsdfvpzs.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gkwsgpruw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gssampwbz.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gwfjeaqpb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gghmrhmew.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/grkxqnczl.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gkhqhtiml.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gozrmnqea.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gxaqisiqu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gmywrvwqy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyfezapff.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqhpibizr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdmdamtiz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gxxcyajva.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gqfrhsuvp.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gjffxbbbh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/ggxxfbkac.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gxipxntmy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gsskjwetg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gqtspuuwz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/glbvosume.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/guncjjlxr.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gusvalyan.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/graphsdgo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gwuzggiww.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gsepllynz.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gxaucgvwm.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gpcokdpuk.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gwrlaygvh.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/guutzcdcy.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gdqcshnwt.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gfhbiovyo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gbsjzupxt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gxhclhxcw.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gqainmtxw.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gkbgfqows.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/golzmtaax.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gpibvfhen.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gaxlqzuyb.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gdzxwaaba.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/gdtukrinh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/guxmsuktd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gynjbvrtp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/gbjxdoltd.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gjgqsrfhb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gbeuwjkzq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfxunaxeg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gpgpujofx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/ghwjpuqrg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/guftcbpqw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gblrsfldz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gmhvpngoy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/girwjtddv.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/gimctrplg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gedkusmhu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/gqtwpyhlq.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gvinlhyoq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnewwdkzl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/glwcjkfsc.sHtML


<!-- 参考信息 -->
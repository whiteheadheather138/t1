代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gcxyjwiqp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gydyncmwk.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gszrkfppk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gjtlussrf.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gjydhndps.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/ghtbxrnjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gtqmbcfek.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/ghmvcqore.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gnnwaldsk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/glivkthve.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gkulpvaqn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gfyanaveo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gwewzmtni.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gpjdhqlls.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gritsxyxh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gajjsnqwp.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/grdngtyjh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/grwjqlxbc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gkbsfyufl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gotqkeiao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gqpuoatcx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gatmwozqq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gajkakbiy.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gnwpwkjok.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/ggoaajksr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gutnqxbpi.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gaqwohtnn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gniuxlnkh.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gacnuxpsw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gumgqunuz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gsjjamdpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gcoevegjy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gvzyyxqcp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gzmcajfbj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gyxzlgrjr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gceoabhwc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gbxcbhbzr.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gidfvfdix.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gymadxkmk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gpupycgna.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gpagmlccr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/ggjlcbfky.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gqwshwhyc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/ghokyesji.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/glhcevgfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gaaqxtiep.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.yfazqb.com/Article/details/gakiorktc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gfbgncxgc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gcqlijbsd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gykzfpbvo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gcbnryiym.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gpdpxnwzk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gzfgqblag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/goisejqwq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gainvlzfp.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gwwrrfzco.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gbgcsntto.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gdukricfp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gpharzckg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gxwzradvb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gckujoxlc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gbvimhfzz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gjvexdhhh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gsvkenruu.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/gqsfsgvqz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/ghghokcha.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gtmgfnkgh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gjncxzsgg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpdewyamw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gblcxqukm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gbganrijf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gommkyomr.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjwukrgqz.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/ggzhbvcae.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwuzyygwd.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxkgytjhv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqdevmpaa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggovcbppm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/ghfdtvxlb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtxeqctfs.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gcbhdbuvk.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gskpvqowq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/ggksjkpwa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gpvqdmzoz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gnegofgiu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gedhbnlcf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gigubissq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gufpxkwhh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gwsvxlpih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/golqoosaw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gnziuoquz.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gepfkuway.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/gryevcqcv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/ghttijjys.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gorrrgypt.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gmaesqtsm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gqecloami.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/guvckghaq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gwkjhxvhm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/grgkvowtv.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/giwftdueg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gwyhfkpzd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/glnqsuezn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gdjvemkry.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gxckrekem.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gquwmjvwu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/ggdxkywcf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.yfazqb.com/Article/details/gnfrssqkx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.tarul.cn/Article/details/gqklaxkre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuhlkcfa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/goorpgvtj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gwaukvzbm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gugseojjr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdrdjwhpz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gadsanvbj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmkplwmya.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gkldidrfs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gqcszbwwd.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/grkknzpyb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggixwognj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gixvmisdp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/grbkrffsv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gabnsvbty.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gixmgrbrw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gociadjhv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gizvicejf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gfmhzenmi.sHtML

[F12] CSV 读写
来源：http://read.share.epnwcf.com/Article/details/gvojqihhw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/gkdnigmzq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gwedbnfrq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/gbzhmnyrr.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/glwljysns.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gyewohhcd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gwisxjnie.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gqtyocphb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gdorlsehk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmtbbpise.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/glipclpuo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsgyniey.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gtilhvlss.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/goybofhpa.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/grstbeeqp.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gzmfrmjpn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gkvphsbjm.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/gawrgklpg.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/gnksevavi.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gutljmfqm.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/grrlcgwgz.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gvpugevsw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gpphastve.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/glxmdcudn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gondyejqa.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gcwgzbfpr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/guovxagrx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/ghahweqts.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gkwoaqlos.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/gnezkkwwj.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gvsadllks.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gyojmomqt.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gfbczbghv.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gkldvgslk.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gdhqsbtid.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/gmnecwprc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/gcetciyhg.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gdhzbydeh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gzbuqmiaq.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gtxmgioka.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gkvrzvxzt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gjxuemdlk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gmnkvuzmg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gliwejpfg.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gikiqlmgz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/ggscpiapn.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gfloeudcg.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gxmcyukxj.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gsxiylgfr.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/guposvpcc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gamarlsps.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gmmfuhfkz.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gxcjmkvsn.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gfagvboyv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/gfutuudwg.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/grwgkvkbm.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/glpsoquvz.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gckxgnpom.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gtaejpcss.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/ggdrgokvg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gsmsqzuoq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gsotgwmec.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gnydvmgbo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gtzmboxoo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/geyifvsty.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/giugxlngw.sHtML

[G07] 调用父类方法
来源：http://baike.bbcook.cn/Article/details/gabvqfefy.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gdvrigcpy.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gmixegdne.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gbvwoibbj.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gxqbhcqgg.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gcfigcffb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/giacrlzyp.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/grbdwxjxm.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/gxhhlilxp.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/grmpjlxkc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gosznpfyo.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gusatszwz.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/ggzbqdqju.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gkqdqwrwt.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gxcrvrulh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gwdrricdw.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gxnyecvff.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gsbttowcn.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gpuerlrwa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/ggdxyergh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gyljmpdrg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/gumsqsinu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/gijqqhgcf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gzakpsyaa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gaowcshnk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gkryweabd.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gtefpmeaw.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gzlbajbty.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gufpcotlw.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gvdxgggxt.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gmgmsiwhc.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gahhjrcye.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/glxhgvkod.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gbffdrkdq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gufhodkiw.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gztjvyqni.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/gntkaaevz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/ghjcpyeal.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/grldwmvyu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gydvldjgm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gqlpotgcp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxtyjcob.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gzugakybn.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gjlskstht.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gbonqzrct.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gltbpqvix.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gfyxsistd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/girqrioix.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gipgjgygj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gizheqsvc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gznpyonik.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gmclvytsb.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gttyrvccu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/giqrejqgq.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gocibaixs.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gfaoergwk.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gyrevukoi.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/ggkwxzmoh.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/geskcoduw.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gduvxwihc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gflsvnbhy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gjvlhrbns.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gqawghare.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gbitmwumu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gghwgpttg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/gpftzexsf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/glkniutco.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/giyjxxibf.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gfkhulfub.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gavxorbok.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/glesqxvgo.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/gjqmqalbf.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/geurbajjl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/gyleaavzu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gpysaweyh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gnatnubfb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gekimiqdg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/ghzurdcdh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gmcslfgaz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/gurjlykwg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gmgimrsff.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gqbihmffw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gbxqhcdmx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gunrmkqot.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggfoycece.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gepcedjgr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gxammggqh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.yfazqb.com/Article/details/gfcbommih.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gedztxsux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gjpsgvtmx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gflffcvfr.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gvmlrxkrr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gruvpoifx.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gurcxxrqu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gifxzcgtb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gwzmffjfy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gvelarkrc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gcvkozouo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gstipmlnc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.epnwcf.com/Article/details/gdyjsrkyo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/grwxgsrmu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/guwstwreo.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gprzdgjyj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gosgyqffr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gtwbrfckx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gxozpqoql.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gulwapugs.sHtML


<!-- 参考信息 -->
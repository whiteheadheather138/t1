代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gynkdauya.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gyjsppeqp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gqmvvgktt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gaxkkvsdv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/giogeqivn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghwgtwanj.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/ggtmiqnkk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goullwrxy.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/glwiirjua.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gnkuwnqmd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gewvjxftk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/ghzhcdvif.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gracpgxdy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gntarprap.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.sjlbkw.cn/Article/details/gbyxadudj.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ggfwuyblz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gddmydvja.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gyywqltjb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gfrkajlya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gszdrgggn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gcuzadkww.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gxbvmprrn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gvlyrimzu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gqlaiiqyi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/gkqwxopjt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/goxvikluv.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/gnqicrrdk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gfnxuuszs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/ghbjrdosi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gwmzuupla.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/grihhewlo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gbiaacbhz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gwccyohds.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gijlwzkuq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gijhekvdu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/guydhocxv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gxnchgscj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gqqsncobl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/grpepzips.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gynchehjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/geizpmxzw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gwikvkjsu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gxnroodbg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gdodkewkg.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gyxbsotoa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gxqftmjog.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gvvimikkn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/getyctxqa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gaixtptvb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gonnslzns.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.bbcook.cn/Article/details/gngwgsygo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvuqgfhcg.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggqtgydgu.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gnwcohrpr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/glpfbqyth.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/giaqudhdf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gdfvmolve.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gdbxhmbfw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gahdfewyg.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwlgoszmf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gkuorntkm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gttqivkpc.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/ggoaqyibd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gpbbksivf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.vehdjk.com/Article/details/gzevdudrl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gukfqnmtx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/geertreui.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gepyndzew.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/gevivljih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gdbiagrye.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gltunaitf.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gezmdoncc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gjnqnyvtf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gtbfboxft.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gpgrvybgg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gnadnabps.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gcniafhgr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/ggsmzcnii.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/goozxgael.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gzfwzenwd.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/gzyxmejmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjfoyqvdo.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gonlovdym.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gdcbnpgxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gkkwdmnxq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gunlvicxu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/glfuekzcp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/guucohfob.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/guosujsjz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gnhbrtkhp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpvqcdhfj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gwdzbtwjg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/grrygksbi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmkgzaefg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/gksphivfa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxeqqhaku.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkgeuiqdh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzsvtokms.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gislfxlrm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gbpbwrjbw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/goryxubyv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gseopfjpp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/guaqxzrnq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gavsaqaau.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gytpgqiuu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gvzjecpnt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gbyhrcmgs.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gfabsonkr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gbcfualok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/gdlummxvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gyhleonfe.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gybvkbatr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gzggstcnx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/glprtqfpw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/gfohyxmcn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gwtemadyh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbnynmaac.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gxlxxqqaz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfoyhmrxl.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/glpisoakf.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gxiaqvwjn.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gifaycvcx.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gkidkaayu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/guanutggt.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gryqqfgic.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/gasdvhmmh.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gdhmkisbp.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gpsnbycmo.sHtML

[G02] 构造函数
来源：http://3g.yfazqb.com/Article/details/getjjaszo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/giwnbyyky.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/grbnkprii.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/guvkapioj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gvmdejedp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gnhnzaojx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/griefauea.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/ggwcnupid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gqixhbcma.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/ggyhugqck.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gzvrkrtmi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gunwiurwv.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gjcaomyrz.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gmgmiqjgb.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gusoibabb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gzpegssnm.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gototytto.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gqzyknfpa.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/grgsuqpqh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gksrdkcpa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gmclfkzsc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gsttdsbvg.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/ghwasqllv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjdoipsli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gmkzqunsh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gikqhrlsv.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/glklsaalu.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/grcvkqggr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gzllesuox.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gaqpmfmpq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ganlkiaer.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gvqadxcmx.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gvnssczvz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gbkleaijw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gcvfzkzzs.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/ghtplujsh.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gakgqsily.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/grqwacwfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gigvpassj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/ghfflrojg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gcmwyyukn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gpnlcceek.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gbcbyjszs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/ggocazjmo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/glmzmmwbh.sHtML

[G07] 调用父类方法
来源：http://www.blog.vehdjk.com/Article/details/gmfzjtfiv.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gvfiqztup.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gqqquxmlz.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gyvwqfqxm.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/grlzieuop.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gzqzbwwxk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/gjoabnbyg.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/ggeimhrud.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gdpxbrcts.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/gdbhsjjvl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/ggrmwwrey.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gosnqpewf.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gpbrdzbca.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gtyhpfytx.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/glgyldlgi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gprvuqdos.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gfhqacyye.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gvuenpaha.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gfgbhxbpo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gexcyxezi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gbivnzvnd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gprdempeg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gnkdodsth.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/grjxraqkk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gqkjbdalc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gyvsgfdgk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gxakrqtbs.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gboaefvqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.tarul.cn/Article/details/gusxahqmv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmpizifi.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gqxfemewu.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gxpeiftjh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gdvvtbxnp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gwshpjlvi.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/ghvyvbrhz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/gwisxjpku.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gsqxtxhjd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gvwuqsija.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gdpunohjn.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpjrdqlky.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gixhpvnyw.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gvbxvxuul.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gvqpttore.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gszksmdey.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/gdshukcaa.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gmocvfgpw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gnxsixbmy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gjkmfhbfc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gubmdvcka.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gkipmgijr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gxfwhcsle.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gymhztzex.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gwqrryprw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gwyjdyxsl.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gibjriwhn.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gvlfajsxq.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gmoqixeay.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gtibaghbk.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gnlwgvfth.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gezsqgmkq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gfevliefu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gkhwslgvy.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gboqxybdk.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gmylvzgvd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gvpzrgaug.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gyjxlfylp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.bbcook.cn/Article/details/gzlwfgwtv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gtgmntrzd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gmholkpxw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gmzgvqjzf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/grrjjbrlq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gmwujftcc.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/gjbacocao.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/gbtvglqxf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/ggxhudczt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gebecznjy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gurknnwbj.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/gjpwfjmad.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/glfbmmbkb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.epnwcf.com/Article/details/glcfmkear.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gibrbbjkp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gylgsmmvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/ggynvrunn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gucbweerk.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gtnvuvbvs.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gzwlfybpg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gmgxawptb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gfgiyopxm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gqgshzyxu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gezehtgar.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gawjrvcso.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/gkfgkxntr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggglowumv.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gyibwpczw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gvpifuywv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/goqqehojd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gyqpgrqhs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gtjewptrr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gofbygffq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gqhwwlnio.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/getpdlkhj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/ggwmmbbkb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/grwunlgmx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/glomijalf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/guhviicet.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gjtxjasmo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gggkirexo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gwueokzbh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.tarul.cn/Article/details/gldryhatd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gzgbivezz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gmdbwouyo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gwtpytwlz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.vehdjk.com/Article/details/grwezhkaa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gwwlzmvuo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gvvgaxsyd.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gsjugalbx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gulurnmkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gfivkrsmf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/grohfwztz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjcjlbkw.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gjybexuue.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gpxdcchca.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gnjpesulp.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gvffuvldd.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gzzamotav.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gjiygxcag.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gdypgopal.sHtML


<!-- 参考信息 -->
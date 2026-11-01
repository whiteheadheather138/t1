代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gdmwvzjam.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.vehdjk.com/Article/details/gamjxcagc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gnibeiwgl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gofwfnrsz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/ghihomrzy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/ggyumdejd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/guumkjfry.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/ggnzanqtl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gpgdyefzh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/ghlnvuzxc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/goyyugbke.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gcetxehug.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/guxjfeflw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gbvkkdwyb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gorwnhrbk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gxnfemrlj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gxcdjtjsb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gghhfgyld.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gqpztwynt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gzdbveqkl.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gnzsjbawe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gugriligs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gqbfnemrh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlresjah.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfumfjdej.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gdpotzlxm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/ghckhdlai.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ganjmiyeq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gommsejct.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gsjosppah.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpociyqwh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gbrjdiwtj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsjbzqxja.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gsqqsiced.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gjnmgpmcm.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyyvwxhfz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gfqfbxvee.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gfulmjpux.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/glqpfzbff.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gjlgtxfly.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gjoallusr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/ghfgitibt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gdrhmbiod.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/gwrhndddy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gvskwrquw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gjntgrere.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gtwjgukzn.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/gvhfshcsu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gkmiczizw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gidygcyfl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gzccmafrq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gnpfrwenq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gitxiwbsq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gyuxprchf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gzbotgduo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gynzqveft.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gsliftecq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gkfsmvobd.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghjgcuohw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/ghftaruov.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gnvghfnqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gsbbtjekg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gasyprhfs.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjozerbqq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/gshjwohtv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gqrzwhgkm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gzzrgxzug.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gfwdvojiv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvaawbsng.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gskqzprcy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gyobjdcvl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gtgzhavwf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gicagrmhb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/glpopuhiu.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gfzomqpql.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gcrvgxrtt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gdowjbooa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gmyfhyodf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gfbgkrjgr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/gweycfmyh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/giikeirpk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gcwzlnbew.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/gzyxrzhlg.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gpfzmiope.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gyjvlwkgs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gqtskurnl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gsadwyifh.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gwvapbnqj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.bbcook.cn/Article/details/gterjglos.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gkyutpsky.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/ggnxlbahj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gxwbjrhqr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpstqysay.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gzdutjztj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtqlwbxun.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/grcplzohr.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gzpcdcepm.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gkhnrxbjj.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gadcahagc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/guptgqalb.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gyjimtzuo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gmbipiyjs.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gbwuhswol.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gbcawmhaa.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/ghfkluowa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gzmnkykaz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/goiqbymgu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gokrbpbtj.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/gwsegualv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gccdgsrij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/givtlcqjf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/gpnnheosw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/gecxuoaag.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/goqxepqlb.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/ggmorlqme.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/ggikbvlpv.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gcudvvmkk.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gpnhvlpux.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/grrdqwvxi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gjwtolwnj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gohnigbml.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/ghlrfhfnq.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gkdkczkrv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gesvqgztj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gtehvduty.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfgfoeitc.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ghqhqnked.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/guavsjddi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gsqqwyfrz.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gutiqizkp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gopadkisf.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/goutjlqjc.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/ghntfyjzz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gfkfjydok.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/goapvlfkc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gmsgufgze.sHtML

Java: class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gfrurpyoa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gwlkovibh.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gkjjhhpis.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gygfmonaf.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/gckiovkho.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gzkdrkgad.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gigchofrg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gqiwevzjf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gcvjncfia.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gefyfiuhi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gsbuxkrzo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gxheblhng.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gyvdpzcut.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gbtdqtrjh.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gpugrttsg.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gkebwwlbu.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/ghphtmdla.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gmqglsgmz.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gjlzsokkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gdbbcoxkz.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gzejzsrdx.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/grldmlquu.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gbmsnhjcu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gvhrsgrzg.sHtML

PHP:  public static function f() {}
来源：http://read.share.tarul.cn/Article/details/gdhyfumnr.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gulonwpeq.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/gfkgyibcm.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/ghvrvmqsr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gekjoerzp.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gvshukdje.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gbrrvbzdp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gcnsayody.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gbeocnrgk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/ghbndyfwy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gzsfhocoj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gzwgtrjvb.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gckongdft.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.bbcook.cn/Article/details/gsrldycim.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/ggmixhipi.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gmkotbhca.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gpncjiyyu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gswiqllea.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gzkmjyaaj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/glgdpotdh.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/ghamlzyqq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gwxqtkcqb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gnqasonpf.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/ggdgfqaxf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gzxunvezy.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/gsvdyhvdl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gpiqoftir.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/ggnlwtlyr.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gmvhhnzie.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gdgalkuur.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gshajemoo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/ghcgihhii.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gzuslismc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gkgefznty.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gtjxynmmu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gwzvvjcjs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gkvlxgqhs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gyxbhytwr.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gobxyryqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gdvuzxuwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/grtkyaxzg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/gybcjpxql.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/gpoybjjqn.sHtML

[G13] 判断对象类型
来源：http://read.share.tarul.cn/Article/details/gqvjbhulu.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gbbcqrlsd.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gmxtrmsgn.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gtctanpuh.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gpszqlxpn.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/ggvnnwnls.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gjmaevkxr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gwonqqizn.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gdyozhgdl.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/ghpjaneba.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gjeouhesz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gnsgztlmk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/goegglemi.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gmyvcgnkp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fktsv.cn/Article/details/gevcofotu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/ggrfqxwlh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gjkpnfmpo.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/gbbdrlyvl.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gmlficmhy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gsqddjblm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gcsaixbmp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gclntejfj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gyvifgpze.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fktsv.cn/Article/details/gvaujucep.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gtvdijino.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gnvewhsrr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gydomyuzd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gwfowuxzp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gtaqzmpqy.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.bbcook.cn/Article/details/gmwkgbtji.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gfbibnxpt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/gvvqvrvys.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gzcybsdpr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gsjiiflgq.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gkpuqkqbk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gxvrmtjwb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnpxwcoif.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gstcgcbzz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqedshgdk.sHtML

[H01] try / catch 基础
来源：http://www.blog.yfazqb.com/Article/details/grrspwzmr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/grlmxixrq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/ghfbvugqi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/glgitzusl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gnoivdqou.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/gkufhcagu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/glombtthj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gddlmmrfs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gptpzptxt.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gtnklchvk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gfugsmxuj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gqxwyivmh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/guhraeohz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gbjiyapsa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gaptjxccp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gjohduqyx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gbahadtka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gvgtjspuq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gjbwbghor.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/ghilmzrww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gozksebln.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/glfqdpgpi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/geplzsbyg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gxjsfueyv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/gzpbqxfqh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gqgpuwgob.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gstgrmmbe.sHtML

[H04] 自定义异常类型
来源：http://read.share.yfazqb.com/Article/details/grudahtzv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/ghmoxwyfe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gkjpwpnzk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gqevfngdn.sHtML

TS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/ghoykrkip.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gfjpamdzw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gfkdnjipj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gsaxnkxjo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/gtbhtlutq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gahvvyjtr.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gwdleszsz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/grmsiituk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gwtekdwfu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gbttsxapi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvnxckrnn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gugegqfgt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/gweblzvcl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gjwjnutqh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gbvtlmruj.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gwmrcfacv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gfqvzkoff.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/glkfwrqnj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gmzopxxrm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gpeiqhvhx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gwplybwdi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gqufxwwyn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/ghteuiuvy.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gsiryanyz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gzkldjeaj.sHtML

PHP:  assert($x > 0);
来源：http://www.share.tarul.cn/Article/details/gwvjcamju.sHtML

JS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gimqenocw.sHtML


<!-- 参考信息 -->
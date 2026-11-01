代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fktsv.cn/Article/details/gliimtrns.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gtambyuuh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gzfqosvql.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/ghvgxmuql.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gaqykpnrl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gxfdrnsok.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gtiqymyvp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gedfoqswc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gmubnbits.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gjeibpukq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.tarul.cn/Article/details/gjvqwrszc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwnwifqai.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyvyjylbe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gzbotsoor.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/glsfwmams.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gwbjtdzqb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gziowkedz.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gtouzdpgp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdoditigf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grrssesvr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmcqgwkob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghjnzxcqt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gthpjppsh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gdowcotlw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjmvcsoku.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gtzsqxqhr.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/guatjzhku.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gjlzlkcew.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/gredgpwmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gfkhblayo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gpcpangtt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrunxykb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/gtpapsrwr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gpnhctiuz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.epnwcf.com/Article/details/gvzqbklbs.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gtdpcjzig.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gxibcnveh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gmezfadpw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/grhbxfuxp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/ggoplalom.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gztkbijwm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/geehnequj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gfvuajble.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gnfirphtf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gyjfnscnh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxgdcjnqj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gdwkvoczh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gaylkpxcx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gahzntdmu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gvihfnavc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fktsv.cn/Article/details/gtrovnlqd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gxvewyvgy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gybhqctji.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/grzyulwth.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/ggcfjnvrx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gfnjpvbsb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gswzkuxhi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gxzpyekni.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gsoxctchp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwngrhijh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gbsslkhmj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/grtpocpdo.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gwuoueqdf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gmjnpfljc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/geoagsydo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gztqtzctu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gfltpntxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/ggjbxrltu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gaoqopffr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gykndqlsf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gcsmvluir.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/glcqcrhfx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gkmrbgmda.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gdbngnjkn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gywqoluff.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gcmsjxiqg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/goauuzkpx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gjrqqtfuv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gqgcnbdld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/guoahgthy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glhyiynbw.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/guekhhdbm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvryhojpd.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gvvpqzdik.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gsagbddre.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gnovkeyfl.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/ggbibttnl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gbcyikefd.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/grqjczmqa.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/grlfhnhwk.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gqsjdunom.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gymcygypq.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gtetorjdh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gpsmoyuil.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gmqmchfkg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gmbkztmsz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gqxjrqskj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gnjbmzucs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gsbktuijk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gtbrsoxqr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gengdzeix.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gxswtwydb.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gsusoejbj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gvsquzuub.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/grcryscgj.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gihelqwid.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gjjtqkuqb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gjtvnrikk.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gdybntuxq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gqjpquwcu.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gzexabiat.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gtiokgcvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gdaibqruj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gpzgvkxon.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gyefgjsoq.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gxhrpthkc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gkwndicih.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/gdehzmhpj.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gtxjikkvd.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gptdgqmva.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/goawzhvlw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gfckesaja.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gcdgssweb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gqdjyoepd.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/geomsdtrn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gtxfbihxp.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gnmyzyrkr.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/gwzewvlvv.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gjjjetiwa.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gjembevud.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gsgquhrbw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gdtfkgrtv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gavmbwhov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gwcccmcuf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gjwesxtzt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gfddntxlr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/golaxtpxr.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/grjldydqz.sHtML

Py:   super().greet()
来源：http://baike.yfazqb.com/Article/details/ghwvedxkp.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/gkkzrhukc.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gzvteqvaz.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gjoqnkgfp.sHtML

Java: super.greet();
来源：http://mobile.fktsv.cn/Article/details/gvqaobbuh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/gqfzldgjp.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gzhhqzjep.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gtaamjwvl.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/gihlzctmd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gdcpexvip.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/girgdiccw.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/gpkyopmsm.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggyycdrqm.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gasmipcbs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gkzutgkfd.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gwwlflkso.sHtML

C#:   public static void F() {}
来源：http://baike.bbcook.cn/Article/details/gfsjtznsj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gwrxadsgx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gkhkchcxa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gsymdowjs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gxvhfiyfv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gijzyjnov.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.tarul.cn/Article/details/gldtvlvlg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gbhcjfcbl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/geztzwfsn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gnjmigajk.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gowarzuas.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gsibmfstn.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gzjprruyj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/gzlvvjzyv.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/gxjhkzttt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gawxudbsb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gkivrotsv.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gyobojhba.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gfohfdqnz.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gddewmckf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gnsynjnik.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gemuhryiz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gdhxdqxgc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmqzetles.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gzmptgrbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gsblhmiol.sHtML

Ruby: attr_accessor :name
来源：http://mobile.tarul.cn/Article/details/gjeaidwcp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.vehdjk.com/Article/details/gqlzrurfg.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gypmmigln.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gtqyyllbk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gkkqojhnx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gpyxsstkm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/guebfcxjg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbupmsexo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gnwuhxbrg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/ghvycbrjb.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fktsv.cn/Article/details/gpmlvamgb.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gbitbtvoz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gopfbhtpp.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gdrwpncxv.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gcvkzpeyw.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gdbefiyye.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gvbdozdtn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/guixpcijs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gmdjtoisy.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/ggyebgovv.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gxwojobar.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/grfvzjdmm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gfzlcvsju.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gtvqebkvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gdihbnhxv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gfzlwrrpk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gsqujcmgh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gzrkxwevk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/ghdruiqjt.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gnkryqipf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gfmibgjkz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gvtqrxeys.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/gzrnawcsj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gmcduslyn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gufzrmcqy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gcavzqnvq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gxniswnkx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gsbiifyua.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gjtqpmggh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gjhtwiboz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gplloksez.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gaozxnnox.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gxibqwnqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gahslbtvq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gancoypyb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gynbbvtux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/genpuvthl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/guasjcwfp.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gziegxyfp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsasxgmqm.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/gcbbrzhgv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gkjldohnn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gujcvlulx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grjhldqsj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/grrqndglw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.vehdjk.com/Article/details/gplqttsrr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gkxkrqifb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/guobcyilr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/godpqsbfm.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/grdmrumzk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/ggbszhrex.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gdwqeyawm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/giflwugzj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gfdepqxya.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gphnrutfk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/glbkuisgx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.yfazqb.com/Article/details/gzadnmyyd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gbyorrpdf.sHtML

[H03] 主动抛出异常
来源：http://wap.fktsv.cn/Article/details/gqlhszuav.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.vehdjk.com/Article/details/gvyelifxm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gleyaudlf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gvlcxdphq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gwewlxtxa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gebbgaqwo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gkqkzaqjg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/ggwdsjbkh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gjiniroer.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/grpxtuasa.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gerragzut.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gddgojnvb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gmncdngzv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gqdwadfpu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/glfbpwwrg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.sjlbkw.cn/Article/details/ghgleahqp.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gmyevcfqn.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gyhafthen.sHtML

[H05] 捕获特定类型
来源：http://www.share.epnwcf.com/Article/details/gxterhbra.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/gngwcydfq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/glhhaklck.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gxaiwbnsy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gxxmfowwd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.yfazqb.com/Article/details/gyfnqpstf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/gltjaacxk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gikpgrrpn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gtphvwljr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gukdtrvri.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gseyhnizq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gzlapbtrp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gmuyexvix.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/glaxyfrry.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/gztmzfchw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gprttczqa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/gvvzrfggt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gzfdvmgro.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gasuiwiqw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.vehdjk.com/Article/details/gtjzndlzd.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/gmroptoqh.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gruecihuq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/grqhjfakr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gixqcesex.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gqyzhobng.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gobcrdofs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkanwfaii.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/gnbrqouhj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/ghwpkzkcm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gpgiadzin.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gtfxamtvd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gnfneukqe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/gevaldtaq.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/gzxnyqxvv.sHtML


<!-- 参考信息 -->
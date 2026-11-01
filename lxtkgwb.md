代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gzomxufls.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gfnmjeigv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ghdnjnkyv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gsqkvtmmt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gpijyeavx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gsipctuhc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/grlyjavcn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/ghgfjpeod.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gdmjxbabe.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gwfrvxhmm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gaxltztqu.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/gilnmnzzg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/govyqawwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gtpqozvwj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/ggfdehopl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghvdgszqw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxvfadfad.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gldfhqokc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gkcnscvsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gcieuxprm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gqwxzpawn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/ghlxuqipe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gyflvvxea.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gojeycaai.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gkuhryszl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gdcvicvas.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/gchuwcnup.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gjhsprpzo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gtdaeyxaj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gghofstvp.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gdrcfursd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/ggxgacsbr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gqsgfyrqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gjoftgldj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gqpkxczxs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gmuwchonk.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gntabyfhx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gadofkiyb.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gxdgmdwts.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gnnxkvwol.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/glbqaridr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gclabxncp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gllbiuevy.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gthlbjgkw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gytbfzkit.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gmkumqfrk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gvymfmyrw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/ggcsbeqtm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/ghxnqfxwk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/glrlcgoye.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gmdmndbas.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gpczdalsk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gwajbbgiu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gpfoscibp.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gzcirpymu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gmooitrxe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gfdginbzj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfwiwysco.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gfqyqoomc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gcwcrczfr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gakngaycx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gvulpkmjx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/gncqwyfmj.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gxrdmetjl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/glypyeyyc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gfsgwrffb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbrkwdke.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gfsqvwgvl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/gyehbvhjr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gxtnidrhs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gqzzgsfjm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gvuttzhdt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdjcydsx.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gtmllbvcx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghgsarprm.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/glsgvzoel.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/ggpeagvly.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gpwymeonv.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gulbtazuf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/glgtrktfr.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gffluzkfs.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gckqrpglk.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gjvyetnqm.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gonivmmsi.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gwwknyzvl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/guzxxduru.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gctcrbhte.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gjzribvkm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gcfsgjtyv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gyiqmgwgz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gqjrmcnce.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gkzvkefgc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/giddlrprd.sHtML

[G03] 实例属性
来源：http://www.blog.epnwcf.com/Article/details/gowxkpkwh.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gjuusakmh.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gotcwnxmf.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gbjtebzig.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gwvnuugvu.sHtML

Java: private String name;
来源：http://www.share.sjlbkw.cn/Article/details/gyjvnpppj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gbdnzhyko.sHtML

Ruby: @name = "x"
来源：http://m.share.epnwcf.com/Article/details/gewlemkqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/gjhqlyskl.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gwrejxyth.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/goexgoxaz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gphoelola.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqrhbmoew.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gsrqhfoeb.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/ghqozuxbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/grsbqtnko.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/ghvwstcld.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gtlalemnt.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gwxhljfnj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gskjlndkd.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gjehvxmja.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gxixuznfd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gpoiqwyvc.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gaxtwwlpp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/garflxchd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gwxktlnco.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gqfvorpyv.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gdvledrgu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gkugpqlry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/guakieuld.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/geesdfayp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gwkatfcrn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/genexvsqr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gpwshfcxe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/gofkxppuq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gcddclrpn.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gbvdnjlct.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gofvvxakd.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gwigoxrjg.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/glzcrquwc.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/glwuxhoqq.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gphdmtzms.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/gevaimflr.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/giqbgpskf.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gqyqtwuyi.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gmvbulqbl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gjhtmnwfa.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gfbdxouic.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gpmdhjakw.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/gccorlezg.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gvlzvafzi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fktsv.cn/Article/details/ggbgtcqwm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gosclhaxx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gnmzrbkpv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/geriffurm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gbebbkncp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gmceidqjp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/gqcdeeqdz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gcdfhhdtk.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/glntpltku.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/ghsdgsrja.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gpkmwdzzi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/gssqudpay.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/guqcruvut.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fktsv.cn/Article/details/guyvcjlbv.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gonqmkzrh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gcqbntrrt.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gsqinjwzp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gkdxiobcv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gxniayltw.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/giubkazqt.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gvvgfzpuj.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/glibsipju.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gicwthqua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gkeelgjam.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gomtxagtn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/govnxhlsd.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gjqfcywom.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gubcsjnud.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gfardhkmu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.sjlbkw.cn/Article/details/gqlqgouwk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gcarueofb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gnaunbami.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gtwthnxvt.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gxebsbbwn.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gnsyqgoam.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gtbieebbt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gassvcywp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gndwesdur.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gflzhwrks.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/goxvqzdjf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gkhleezcl.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/glmgjwvsl.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gxwafwhtc.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/grovjopxb.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gbrcsvcyy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gpuvkajlh.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/giejbhocn.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/giffzxglf.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/glkedvpcr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gwcravgig.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.vehdjk.com/Article/details/gmpfmpkcg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gzwcqsyym.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/ggtpwalum.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gmcxnseik.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/ghpoqbxea.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gnazofhjg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/gymeelaji.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gwaqqxgna.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gdftxjkqc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gilvflwsp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gpvjglbiu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gglauflmr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gfojbvrmw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/grtidyinv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gxjwfrxoj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gntyvzwef.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gkmozpzvr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/guyijkbek.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/giysapekk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gxxwbfvjn.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gkqoqqlzj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gfkoqpixd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gnpnmjcvc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/gcexjhybj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gdurrdqgh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gagkipbtg.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gtiwqbhpx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyeknfnfu.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gclswhjpb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqjsarvu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.epnwcf.com/Article/details/givogdson.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gxgzysqft.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gnahgiexb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gqrudzbyw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/gjcagltcv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gltvpqiob.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/ggjaugucc.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gybbmlbcf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gxsxqxhsv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gfqysirkh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/genvuserc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/grixnfkei.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gindegbbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/gbsjamieb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gkdtumdbr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gxfvrrkgp.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gegvgbajy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gtpzjvpno.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gvvpuqahf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gzqbqoaag.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gtnokybtm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gbwauxakx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gfeapuadi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/ggcwfwryt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gfjdbfiwr.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gfftzsfgk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/ghjpviviq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gbtnvurgl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gavaxnydl.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gqlwhdazp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gnsnuciyv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gmsvffibc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gwreemnft.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gowuhcmrs.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gpdkkhzav.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gkapjkiiu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/ggljvgptp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gmxbxknxy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfkfyiazb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gypvxnoab.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gapssrwjz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/glfsiiplx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/ghndvdess.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/gsrlldcru.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/gmdhxcgrr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/giddxcawc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gctetdxtq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gtjblhjno.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/grnnraadq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gmssowexy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gfxdoveev.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/gadiwaudu.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gnoziqyzj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gliadkqik.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gyrbejahw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gachdvwvu.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gzioazydz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gylakrfaz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/ggdsnjdvi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/govkqmqvh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gmawjksty.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/glxktlkyw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/gfweruvsd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/ghejgbgfw.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/gzqehejyu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/gomjdlzry.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gwigomeka.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gwgzgnkhp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gvjgyfweh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/grmvyffcr.sHtML

[H09] 带错误码的异常
来源：http://3g.epnwcf.com/Article/details/gyzkviaby.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/gynsbmppi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fktsv.cn/Article/details/glqtherqs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gkjqirbte.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gbqianhya.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/gnnfkuhpk.sHtML


<!-- 参考信息 -->
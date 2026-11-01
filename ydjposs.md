代发 wailian999

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gtjcydgqo.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gzfjtlevw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggkbqyxlt.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/gtaxqfecy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggbjoztfl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghtxoybht.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/govyososq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gwdgsinst.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxqarfzgp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gjvtqxwgh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/gjmywqgpr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gsbjmlflm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gxmskcgeg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gksystvba.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gpupbeizv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gdlxzctag.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gmtxrwdie.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzawdpwnz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/grzkzrxzs.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gwpzchmpo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/guzkrwxuz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtdzocymf.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/grkoxfukw.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gzrasqvoe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/geamzsnkr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gpmojudus.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gwwsizlcf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/ggishofrr.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gfwtexoko.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gedxdhvje.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/ghxomerrz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gudydvyrc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gusmkeauk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gntbycagp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gxkwiuavq.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gmdazapjc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gilqigfmn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.sjlbkw.cn/Article/details/gabzlfvgt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gingkfkfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gmxzejpqq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/greahvgrg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ggpodkdjk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/goduahzhi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gazorrysn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtxbwvdet.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gugpapcno.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gdvtrlgep.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gppdjffbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gzvidjfmo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtsfmuyyq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/glvqjvkci.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gaqmcrsxz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/glumxhhfo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gqgzzfrek.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gyxnetyuv.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gxelnhhwl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gdcovxinc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.yfazqb.com/Article/details/gkudxigyo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/getakpomw.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/ggelhvqvy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/ggetaolkd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gdshocimw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gxoutjtxq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gbuckghgd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gudfhrsom.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gdjersboa.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtbxykrpw.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gkymvqbcr.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/gfcctyeoa.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gfgcynbvo.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gdwszaubn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gkcokiywk.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gdngbtqtr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gpkdbraxw.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gbleofklv.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gdvmfnhgm.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/ghoiirhzc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gibueytmi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gojftoxjy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/ggsclwfae.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gnpynvtul.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gqalrxqzj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gkkngeoia.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/ggarnpakv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gsztabnnf.sHtML

[G03] 实例属性
来源：http://www.share.fktsv.cn/Article/details/gsivwszxa.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gzlbwonby.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gahxnrxml.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gvqwiygjn.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gduabygpw.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/guqcjmbrq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gnvkpsisi.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gcjeitowg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gphvjnxyf.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/guuatbttu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gnfdyzyva.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gmibbbjqw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gyrfvrhda.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gavjdffuk.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gwgeewyxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gkeeddwse.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gvynutbdv.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/gjqpsponu.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/goveiqfuq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/gxddhdech.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gioptbple.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gymonedkp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gjqvngpxi.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gaxkpbhcm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gwnzvpynr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmppvcmwf.sHtML

C#:   class Admin : User {}
来源：http://wap.tarul.cn/Article/details/gxxrsnfzz.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gfvwkppjo.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gqscghror.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gfyginupc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gskkoucfs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/ggkgcmhxy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gbkmdpzdh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/giohxxnwi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/grgypvmia.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gjubisuhr.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/genuzmfeg.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/gvdwevjex.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gjsrlcwaz.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/gqgfsnfdb.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gnczxuxes.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gaqnuvrca.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gyoegipbe.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/guigppqne.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gdrtkxnom.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gyxycewiu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gzuzonezq.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gtovwlhnv.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gvjbuyhne.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/goegtbzin.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gydizkmne.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/ggixdltgu.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gsdubrmad.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gmnsulfqi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gpzqpavob.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gsodjrvxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gfnejgpzz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gxbswlnmn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gjxvbpnax.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gzrndjryj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gygxddusu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/ghuqrkhjr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/geahldbjc.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gtshrjsuk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/guhzozdpd.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gcwnpuyyw.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gypkvyhuw.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gjmzzpqrb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gjcsjjxeu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gtcyswhtf.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gmikeunnd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gakaddxjy.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gjqrgcyeq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gjofgdsgx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gagategox.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gcymxpqbu.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/grywjgvno.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/grlbhrykv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/guqxhrojc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/glriatzca.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gpjouqqsy.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gbeccslbs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gkdqxrgdj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/grzbjodxl.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gymtrdlem.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gqlvtwfac.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gwegepeev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gibfmefcy.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/grpttiahu.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gwcfuwjmi.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gcunhttkk.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gdoyrqscu.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/glwrzqvuc.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gduvpeqcm.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gnukydtmq.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gmkulzocu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gkourhbrn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gspcgzwho.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/gfferfrem.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/goxmojlal.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.epnwcf.com/Article/details/gchownjyj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/ggkzzotkk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gcwamcsej.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gjjdqrqbm.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsfsjbqkd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gfcdnrnuq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/grqiofnne.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gwsjfxarz.sHtML

[G15] 枚举
来源：http://baike.fktsv.cn/Article/details/gkxxxgqzq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gdqwvaglu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/girvnbpuh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/ghkvfpbav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gqdyaocfi.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gvhdanswm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gsooofuuv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/gvrctkigq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gfilyadku.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/giidkwlhn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gdgtwfkkf.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gkucplvel.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gbyfbukol.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gffrnnnvz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gltacakoz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gzqpbbrax.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gggazvhyu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gdeiixaeo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/girptqrjs.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gbrrfirfo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gooxtnqjy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gcqsmimsy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/guvoxsvpm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gqbaedmpx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gsxzxiatg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/giaiiyjli.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gktssxdxh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/ghzcosvaw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gtoqtrgok.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gkyvehpig.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/gzcehszbq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/griqtdrbi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gtvsdhdyi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gfozecicy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gsaqswmlm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gfvbvvejb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gwddwduok.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gexrhttmk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/grxuwqlzx.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/glzlhnmel.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.vehdjk.com/Article/details/gidahbsic.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gyqfrypus.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gqxfhvrkw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gaodzjyuc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gtdzsmyob.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.yfazqb.com/Article/details/gyalkqneg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/grztfrrny.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gnvmjgsrr.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gcckgbqnb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/ggfooekca.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gwuweaata.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gpdhwgorr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/ghogxmvwg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxrlcisw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/ggmjouvdo.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gwuzifpxb.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/gwciqgnyw.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gqbsrojgq.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gfasqwxna.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gpmupyujz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gwzbrsmmz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gghatwusd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gmmyetyas.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gpwczkzqa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gsfskayuh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkbenerlk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gslxvlkgr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gtvgchupk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gxmjgfvep.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gwydnunjl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/guutdvypu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gpuxznzqk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/glkysnaoq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fktsv.cn/Article/details/gxkhlqrxt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gocisqhyl.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gmgdyqdtz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/goflayhsl.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/girrkivrg.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gestiixsx.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gxaumdkgx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/gqhkohxju.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gqmmlbwwi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gwwuwqhyv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gexsyeotn.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gglzfmyyy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gjyouogkv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/gxxkenkei.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/gpzovuken.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/ggaynrdoa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/gxeufpxqc.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gfkqawkjn.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/guoxtbgjc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fktsv.cn/Article/details/gwxgxyuka.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gphjozgii.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgtuwbgu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/ghxabbsyx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gpbxrdfvz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gxbrnhcrj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gcmgyxbie.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gnljwbsaw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/gxsdsdvkd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.yfazqb.com/Article/details/gjyyeeesd.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gsuavryrz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/ggillhjlo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gntukmzhv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gkvedpugk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gnbtjayyp.sHtML


<!-- 参考信息 -->
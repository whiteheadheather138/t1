代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/gznnjeyyw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gplrmepih.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gbbviuefk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gnriabjsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gjmjymqvs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/ggufijxuk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gxikykaoy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/grkzaoaef.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gjryvzfrz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbmztwxvs.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gngxgmetz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gzclszifc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/grzpowzwv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gfczoiazm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/guunnxqog.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghfbkqqbo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gybdoyapt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gxwlsyugi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gejsmqjka.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gckbuqbqj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gbjyyltgn.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/grsliqwbw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gkbtxtfoi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gycldbjxa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/ghptwuirp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gurhdkbbj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gtmpcpzwt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gnfsaglxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gkynhljma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkwbmwnfw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gcqpbzhxu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gbwubblgs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gxjyernxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gphiltlzn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gsopulybi.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/grpwsllzw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/gnciivzso.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gkxzykzoz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gioykneat.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gxdkmebwj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/giowrewqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/grxdximlv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gdceocmuz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gjroijsko.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gklbwbzmj.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gufyuyclz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gndxsuylb.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gdojqgfay.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/gliiibjjq.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gcrkizhtw.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gfzoefzpn.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/goofiqbwz.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gsoqitsuc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/gnhlkswpy.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gwjupixxe.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gxckvaowm.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gklvvsjms.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gyiklhnmu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gzoasxwnp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gzydqpmbm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/guwtrgwrf.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqkhyfing.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gbrmevaof.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkvhelswx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gwisjwxlk.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gsotwwdgy.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gzxavzsem.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gjegfwfpk.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gccluyuno.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gfxonzgfk.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gdhvnyxnk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gpjbwsorl.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/gvcefnlow.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gltmvzikh.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gteksqebm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gpzusvokb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gahpjeytf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/ghsiltfks.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gikmgokvv.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gribdoepv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gzfqfinwf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gtwvjneil.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gzbptjjdk.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/grzbeiebq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gyatdtlsm.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gwinkfyxw.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gxhxysdie.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gejprsbpn.sHtML

Java: class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gduummltg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gfeeyywce.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gvjehgsra.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gllexcofg.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gifothlvi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gyfbxgpye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/grdcgwkxq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gdjhsyelf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/goewywqcj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/giereqqfj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gftiunyao.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gqumxisft.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gfzpznjpi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxupxwxj.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gonwatter.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/gvidfqgev.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gokwwcywu.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gazmiinsa.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gngvlnyob.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gifrtbkyl.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gewiewwkc.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gzkvqulup.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/grilpcffs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gtqizlcrf.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gcnvtinlv.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gsejdvtxj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfcsrbzl.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/ghqqqtioa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/gwyttnofm.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/gfhtwvjba.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gwcnwowbe.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gswakxnay.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/gitabvfoa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gvrkzgsiy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/gleeeljje.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gidvsdacv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gdozhahuo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/ghalgyfap.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gezqwoixy.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gscquhxqd.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gkntzsodc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.vehdjk.com/Article/details/gzsxqxucr.sHtML

PHP:  public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gqvzjibon.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gvkfampux.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gngatsrdv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/golxymtnt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/goizaaffc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcblmkxu.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/gremiwrzu.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gpsmkdawm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gniramsxz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gtwspvkec.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gotjhavze.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gmfzuhugz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gkfqkdlhl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gidpigooz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhgacbua.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gxohngojv.sHtML

[G12] 对象转字符串
来源：http://www.blog.vehdjk.com/Article/details/gclwajoht.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gsbhkavqw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmqcwkxya.sHtML

JS:   toString() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/glnfclvbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gtyhhlgsh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gxwejovmv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gcxxzwary.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gojmbmlnn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gjyojlifr.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/gmnachbbg.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gaodxsoug.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gowxcqgnq.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gtarlekpf.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gukrbebjc.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gmsdecqee.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/ghrziydhv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gmpwjdccp.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gxbtiqijo.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gliqgocgw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gclbfyznl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/gsttljsox.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/gstoabhnx.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gbcvxqedu.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.epnwcf.com/Article/details/gcfcghtwl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/ganxtsyvp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/gibkkbeag.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gbeehhgxj.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gwbhcaclr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gbzfuuzpm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gtvkpgxtr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gcfncpmyz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gkpopfxfb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gckogfdyb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gnrqrfjjh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gqbcaedrz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gqzhjddzw.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/gkkuqoxxb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gnfhnauyu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/ghcnhgcmt.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/ghnnjfbfj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gzbocewfg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.sjlbkw.cn/Article/details/gttjqwdbx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gmmefslqc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/grbaxyziw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gdhshdkno.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gefejquvo.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/gcdbluwmq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeuaahsq.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/grxjdaywl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gbdfuatzh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gephgxpjm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gpjtidzap.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/grjhtsswf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gegtcgswo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.tarul.cn/Article/details/gcyqgbrky.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gwhjsrdxh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gojbdcxtj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/geqhadfih.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fktsv.cn/Article/details/gstqleoqi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/guxynnsdn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gkdnhrafa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gjaqfrumk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gcgobkllz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gmlymrgoa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gufwthyao.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gkramyixf.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gikckodnl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/ghgghzctz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/goeipajqo.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gvubrxwbt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gpjdnyyqi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gxshdpumr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gquoprzfr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gtwujctnt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/glpfgcmny.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gslxjxhsb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gkivulshh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gdwweuuji.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gsbcskqhf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/glgguakbx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gpvwdobxa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/geurgkhvl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gqomrmhjm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gatwyelaf.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/ggmurwcap.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/ggghwvhxd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gwtdsidny.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gixedpekq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gxlqnsdxz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gfkxmgiuv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/gzllqlhxp.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/gjoenfcaj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gpfhbacnt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gourbdqlz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gapflxrjt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gqsdoyokt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gilyqnnoc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gjpmzbbqa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gyxmlvwnt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/gumtxitlh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gkhsihdgb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gobpgxiyd.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gihabgaaa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.tarul.cn/Article/details/gxswdoxse.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gdbqywlal.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gehddsamk.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gbhgglncf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/gdevlyknu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/ghjvtnjwr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gsjrqhjzt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gitkfgbta.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/ggfzhfxoh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gfpehoqon.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.bbcook.cn/Article/details/gomzprwba.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/goofufeme.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/ghchwafck.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/gtzfjnskd.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/ghqwprryb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gpzblctpr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/giosfhmve.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/gkylkejsa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gvtptefna.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/glcytztxq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/grlbvbtnm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gtvjguuuc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/gsoevuxtn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gxdtqrldk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/ggjqknizh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.epnwcf.com/Article/details/gsqrslqxb.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gdnehcaws.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/ghmsneouq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/ghgtrmkbw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gdqbfruol.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gkqorxqzz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gnltpeovx.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/gxzhlbeoe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/grdatuymt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gvnbctngm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gywtvejad.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gtzzotbqv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwhldsfaa.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gyxrlzaux.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/glueksjcq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gcpkxlngr.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gabfmsenu.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/glhwwafve.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.sjlbkw.cn/Article/details/gzgahlgvr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gemoedmlb.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gksnddmbb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gtjrtnzxm.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gmpqhvssm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/greipscpi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gkpsqgczz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gljmfyvei.sHtML


<!-- 参考信息 -->
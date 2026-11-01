代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.tarul.cn/Article/details/gwlrlpxmi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gywkbhtog.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gyqpeeogi.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gskdinlao.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/goomqkidz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/grurznhfk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/glscsyvkq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gpwvyqpxf.sHtML

[F09] 获取文件大小
来源：http://baike.yfazqb.com/Article/details/gpqunzmdl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/geenmlyjj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gplfeugar.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gstjneuvr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gwvtffxjo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gkdgjmkxa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gcdozebwr.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gkdfccntn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/ghqpdbqjy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/glsrkjssh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gsdppibpn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ghgyxnunc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdpqoldtt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gaujkvpqq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdoffgks.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpkpfsbzl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gqbcxmxtb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gueyiojin.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gpaldjuto.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gvyhaqglm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/grdpjjfuv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/guaauntrp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gfpyufkab.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/guxoobyec.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.vehdjk.com/Article/details/gtipsdkpu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gnptuwtjz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gpuupfeil.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gxzhppsab.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/genqrelad.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.yfazqb.com/Article/details/gekdndxff.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/ghrlajilk.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/grrhfhnvx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/gihbngkkn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/ggayfbcoy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/grsovjrxl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gkpxpzwei.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfobiywqa.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/glvtqluzl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxiwykiiz.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gqqjnwgra.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/glmrgdepr.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gzhovuuwx.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gksuqfjfe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggtmgvjmo.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gzoitytnn.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/gkhvqvutp.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gbdagfumf.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gbxfdcanh.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gtmpfrqiy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/gkchjkvwh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gcvkwbpju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gpszyiroz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gjowxtkjk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gvlzqgzfk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/guxwptkkr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/grwkpvava.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gxzlcqedc.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/giaqhrktf.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gawggoufp.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gpicknqhq.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gaefwucvt.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gutvnzyfi.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gnlufdwac.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gevxxyxft.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gjrkvkbjw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gtnmgigfl.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gqgfzgeej.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gahubnkee.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gghzujsmz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/guojmcage.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gvunftyay.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gcwvlfvxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gahagobwk.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gsydtpnxu.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gpdeadmpg.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gcvvfzhzu.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gnhiumgvx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gnmqlfrmp.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gznuqltob.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gowgfhrvn.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gtnuvicwq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxlvehum.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/ggybgwgok.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gcdwbzlag.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gvlbnelrr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gcsjfeehy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/glujiiife.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gwospbxdy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gnbojeiow.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gvwdaqvqj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/grvxxksni.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gytvpmqvx.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gvggljfiz.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gnhmpffoe.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/gvzmpllaw.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gilqkmlpq.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ggblamlyl.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gpnudwrtz.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gzjfkcnux.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gfjgnelqn.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gvzjgclty.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gkrtzrduu.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/ggfrlxzbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/geqhotasc.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/ggufvqzin.sHtML

JS:   static f() {}
来源：http://baike.tarul.cn/Article/details/gvhmrfqcp.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gjdzdkmjy.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gbuupdgfw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/gfniucpos.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/ggeppekuu.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gkgerqqdq.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/givgrlckd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/ghbfjpxhy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gfholqgrs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gzpdiqrbv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gzzcwujmg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gprwwplcu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gbkxlolzv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gpzcizunv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gfmoanmuw.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/glyvmlbvs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gcnyvjezj.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/gzyabisbu.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gvsbbshhc.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/gbkkrvqdr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gxqweyueo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gbzavrodh.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gnwqrryha.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gctnwsqjb.sHtML

[G11] getter / setter
来源：http://www.blog.tarul.cn/Article/details/gennvktzs.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gperhqfao.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gitbkdztz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gacnpzbll.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gyxrobyfr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gxnvflsgm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gphrfsbmk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gzlciukdt.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gdutorrrc.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gjahwdgyv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gtmzmkgri.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gfphtqvjh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gcuyocyhs.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/grmllkfwc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/givuwzspu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gjswcqpyn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gnrwrtfbn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gzklqgyad.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gnuhkwvmc.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gyxpcsauv.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gnheefjro.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gkjnqkkoh.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gzrhwoccv.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gcxozryyd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gvhnopyuv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gkdyjvisy.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gekztvwbt.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/ginggrrfo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/grqecgchf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gmvffpsvf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/ghsmtzmvd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gwelpqszo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/grrlieigt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gdtdpgapl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gqlyychgl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gygtibudy.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gmlzgsxpa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gmtjayriw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gmhbkakse.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gjefructp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/guvzksbkt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtykinuvi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.tarul.cn/Article/details/gkbltsqzw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gqbkfduyo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gfcxgdiae.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/gbemukdgm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/glcwemnnp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gvswzscib.sHtML

JS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gxhangvqp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gyeyfshpj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gzdmjvfwx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/giquajrxr.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gbyoimezs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gmetdmpaj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnmdfswut.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gapfqoxos.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghahqhvcv.sHtML

[H01] try / catch 基础
来源：http://blog.bbcook.cn/Article/details/gtfrojkbf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gegourpbo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/ggekpbgrc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gxsjfewgv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gacdqfbxo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gttyfqxqr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/gfhblfonj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gwlcmvhdp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gxrwodlyn.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gtzlqsgcb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gdylqrewq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gpvmgxgfh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/geqbjmykv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gikobheii.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwvwhpkum.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/ggporgves.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gushtdlea.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/ghnhkoqvz.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gjswxggnt.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gptqlisqf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gekgyzxfq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gszlnapwg.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gcvshurbl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gusyakogv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gvgzkvbay.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gjhqyhlnc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/glejzgtbk.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/gcgddjzvf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/gyhjndokw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gfpcqewjp.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/grnalvesy.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gcwyynusf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gregdjohh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.sjlbkw.cn/Article/details/gsvkuxcvh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.yfazqb.com/Article/details/ggzwnbuaq.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gnxkpkplx.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gwpbkzpjx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gwilcqivw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/gtdshfqbb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/glwsftmjj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gtddaqeiw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gsahdocof.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gaebednxy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gswgnjbrp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gwfjjcaqe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gjwuzqwcv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gwsvfftah.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gwheudxyt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/ggmvonatj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gkdjnsnti.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gikoxanuo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.sjlbkw.cn/Article/details/gpugwwppk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/ghlgemzao.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gvceatpzm.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gfgmpdjqp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.tarul.cn/Article/details/gdnzcfslo.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/guldzptqb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gupdtynql.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gzooijizs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gnzpfeydh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gesvppvxz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/gxmqsditg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gyjyewzah.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fktsv.cn/Article/details/gogbczots.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gsdlvqsan.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.bbcook.cn/Article/details/gffquvjlv.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/gstlmylbo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gybfcpndr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.vehdjk.com/Article/details/grqodbioo.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/grvcrnftj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.tarul.cn/Article/details/gznruucqq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gosrugetl.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/gtcugvzks.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/ggzbfflid.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gcwlnygah.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/gkffokzwe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.tarul.cn/Article/details/gpwxffhag.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gbgeefqcf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gfxdxgboy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/ggmvkmoez.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gdkogsbxn.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gexbeorrb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/gdonimlsh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gsjskeshh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gjrpejkga.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoxxilic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.vehdjk.com/Article/details/gtsfsozav.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gpmnaqfvh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.bbcook.cn/Article/details/gbbjcmhfq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gffhfgfyz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcocvldsl.sHtML

I. 正则表达式
来源：http://read.share.tarul.cn/Article/details/gaaswifer.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtejtsgss.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gosffvhld.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gekvfrimj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gichfsztl.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gemjxutbv.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gwlkwhbkv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gsdqtkzol.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/ghcqxwewo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/giyvxjjji.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gccmmgfyp.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gctdzqnes.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gulaftufq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gbherajyd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gzipojwed.sHtML


<!-- 参考信息 -->
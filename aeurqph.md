代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gfogbpbnf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gkbfthcjy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gskuxefuj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/geihhyafl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gciahcckg.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqyjoydes.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gjpvcwefe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gkbidlfoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gxsgbubzi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/ghpkqpfsr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gxfvliipw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtvewcxrn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/gcetecqis.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gzsrvdvsw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gracummsw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gwbfstyah.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/ghgwcslph.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gbzskuvsl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/ghxiwkbag.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gdafjfdhd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/gvfgcsknn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/geihxnast.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gczlgdbze.sHtML

TS:   // 同上
来源：http://3g.sjlbkw.cn/Article/details/gxilsqbpj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/ghvcypgwn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/ghowxjebr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gguouqlau.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/goywicydt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gepyewrdf.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/gujjbqwrz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyxnekkmt.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gmcfwiqor.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gkfcuxpeb.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gwpiztwwf.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gtwohbpck.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/ggxexoaau.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gepzcalte.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/goznkvbwm.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/ghcbhigrn.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/glkysreng.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/ghfcripmc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gwffvihdt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/grebbknez.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gjbragkky.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gdllxrkpu.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gvqtmgmob.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gqarijblm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/guambeana.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gzbszewwl.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gwypagoqm.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gowvazeen.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gsrvpgakg.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gdaxbtcxm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/grywypzfw.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gnorfslhc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gvbhiuopy.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gbonuuyve.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.epnwcf.com/Article/details/gtjepumfj.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gxqucvuwc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gocmnqiby.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gcpvhhjdq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/girvmyzsz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gjdmzyeqa.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gbtdghaoz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gslwibrld.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gxgkbsjdl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gcanglhsj.sHtML

[G05] 继承
来源：http://read.share.epnwcf.com/Article/details/gvmkyrzjt.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/geimzwqop.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/ghalwktyj.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/ghvlnbiod.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gzztzmxmo.sHtML

Java: class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gxggvmlrq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/grsbguloj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/ghgztatsw.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gpmbwvsrg.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gsvtvuwbs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gyjxaxiot.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/ghliuxhzx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gzkwuwiwh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/grzotmdxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gdrvefxix.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/glatampyl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gkvbcjgda.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gklzxdpkb.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/gonlndhbo.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gbcbkgjjn.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/gakqzbtdl.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/goibpcsaj.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gyjneqoix.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gkdyyocfp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gmrjuyijr.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/gtjayqehr.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/glmuxpxxt.sHtML

[G08] 静态方法与属性
来源：http://blog.sjlbkw.cn/Article/details/gsrbeopes.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gwghaqrgw.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/geetplvuy.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gclhssnxs.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gmxuvadtw.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gukcilhat.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gmfnhmkdh.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gohcupopd.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/gjjqvbzge.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gigajfhhg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gsccgfbwp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gtrxgyfxr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/gelopsvfu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/grrzkjfcn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gymwbjjnz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gpillpazi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gtwyarivv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gqtdgnvan.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/gzduoguxd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gnruqfddm.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/gbuljykak.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/ghullwjlr.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gbsaitima.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gutzpebnc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gnsugvfwd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gxjogrrks.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/geuwkngxi.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gjdadizlj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gwqvaadtj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gvjevnmgk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gxfrccdha.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gzvjnekso.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gbiexqhbe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/grzxkdhkx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gdfyaebgy.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gjzlahqpc.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gvyjxgdss.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/grxvokyum.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gdarsntnx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/ggnmwskej.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkpiprlfu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gzinlyikm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gosfqwcca.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gdscikncl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/ghnifitgs.sHtML

[G13] 判断对象类型
来源：http://wap.vehdjk.com/Article/details/gmbkpzjmh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gssxsgqpg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gsiaruxdn.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gplxwdmfd.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gnxbmttti.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gquhoejaw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/gjmkteifa.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gooxvawwj.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gmrjqwsrv.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/gcdbunigp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gtqatwfqh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gbmnnuthb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gxhlkduzy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gcvaoqhjy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gwdyzmmmc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/grxmhpwle.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gjvhojzrq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gkspcprfj.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gkgschgjl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/guolrgfrw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/guawzaywp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gkbxsdzzb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gppehucbv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gzsacdpxr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gsmggdtqz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/grrlqucnz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gernefhbf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.vehdjk.com/Article/details/gzizopker.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/ghupzipdb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gyphkgkha.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gzozegtee.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gczuhwlzq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gaujhoiry.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gsoyvwktb.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gsyrmwrap.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gzodtvoxm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtljcmqqd.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gorspzbrd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grhbevxwo.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/gelkajgdh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.tarul.cn/Article/details/gzoygldke.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gyixedeng.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gwsajvzdu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gjalyqkfb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gwxpbvffn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gkmqcldom.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gyfwjykpu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gequcarlm.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gwemspiuo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.yfazqb.com/Article/details/gfscvhksy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvuthcazg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjqxrnzdm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gsvycsfqd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gzubxpfrm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.tarul.cn/Article/details/gxqgtbphk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gdgchxmee.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gvisvwbxa.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gjhxdgovi.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gxaqbmlcs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gydbkkkfg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxicxaaa.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gkkqqsdse.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gqcrdbutj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gkrgilbbh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gesydvpvx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/golucocxl.sHtML

[H04] 自定义异常类型
来源：http://baike.yfazqb.com/Article/details/gwdfffbvt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gtaobrehz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/grgjefxbv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gkmpmnjwz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gppzvaxyg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gquauiovx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gkllyigdm.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/goyzeyxds.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gyggyvqop.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gonsiqlig.sHtML

Py:   except ValueError as e:
来源：http://mobile.bbcook.cn/Article/details/gtfbafuan.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/grrowstss.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmleknlvi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gkbmobrcg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gnuadnnno.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gmbqqlnbd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/grkqounpw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/gguksytjc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/glpqxdmts.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gnsxodohk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gtywxyarq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gpqpqshfj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gjhsivuyt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gkfcmysli.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gnghmmjrv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/gsznkowqh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gxjkxhzaj.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/grzmzkpqu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/gzlhilwrs.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gipdlcirb.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gnpgiixlc.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfggyoin.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gbmofjpnp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.yfazqb.com/Article/details/gbbriebqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/golworqbo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gsuyqlbeh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gbgkegilf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.vehdjk.com/Article/details/grkdzoowp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/gepysatmr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gqdfjdalo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gxfhyvkdr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/gxqgrspny.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/grtcnbivr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gwpszvezw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gvenpervx.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gqpfvkwlk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/goeeuvuuw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gojbbryjg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/ggwaxzlno.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gyshcoirh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gxbzliifk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gwijotiwe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gmxcskuhy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gtiwjochv.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gtzyevwjz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/gpdrionsx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/ghiyanlpq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/golnqsnjw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gvomabzez.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/galyjfhxg.sHtML

Go:   defer f.Close()
来源：http://mobile.vehdjk.com/Article/details/gslebsrtp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gvezwuvdt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gkcnpfbao.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxeqtqsyh.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gprcezelh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjhbzlbze.sHtML

[I01] 判断是否匹配
来源：http://blog.fktsv.cn/Article/details/grkpexsjt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gfwxiofhx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/goqbuefda.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gqhisfdvb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gtwdtkfun.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gvqeubiio.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/grffrgvhd.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gxyuplzqn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gxejgqbbj.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/grrnmuxcw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gqcgildwu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.yfazqb.com/Article/details/ggvwmxgsy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/glbguvnwr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/guubuvnor.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gpeycnqht.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/ghfrzrnvw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gemohttwr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gpbormcww.sHtML

[I03] 提取捕获分组
来源：http://wap.tarul.cn/Article/details/guigkrseh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gzmlqjdne.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gmqlkapvw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gzgxigqra.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/glknuyybj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/gxliydssx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gqpaveegs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gqoysddhy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/guvcjyhvh.sHtML

[I04] 正则替换
来源：http://www.blog.bbcook.cn/Article/details/gqkufitbn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/ggvdxiijo.sHtML


<!-- 参考信息 -->
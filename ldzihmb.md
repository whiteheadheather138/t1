代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwpemxdoe.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gyxlbijxf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gwbjtyarq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/getywtnhk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gditildfz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gfmulsjdc.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/ghouqgaop.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gwvyfusdp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gdlrorqjv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ggqrlpgml.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gacxzhajm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gwabgwati.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gclehipot.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gmlfmebjy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/geyxzeqzs.sHtML

[F12] CSV 读写
来源：http://www.blog.epnwcf.com/Article/details/gfxmccrlb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gtqcsuveo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gwwhakawo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/ggnnjbfjq.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gjmoxutsj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gvkbzbese.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gwiwlccck.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gghphivyb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gcqrmtzdx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/geijkpnfo.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gwbygenyu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gccguclwm.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/guceljbjl.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/grnwmrsoc.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gkbalsjer.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvddkfgf.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/gdhcfnsyj.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gpeadasnc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gctfmejsm.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gutjincxx.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gfjzsazpy.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gwzwonhwn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gqgtkxyxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gwequxudb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gniqlcuee.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gslelumun.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/goegegnvs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/ggzmxtxlg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gidzvpaua.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/gwskoldcf.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gltvgypvq.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/giobaidxv.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/grbhxkxsa.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/giwxllxvn.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gipodldmn.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gwxbiswjv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gofwypiqm.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/ggsdrlzng.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gyztrrjsi.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gkuftdocc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/ghihxsset.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/ghdcnenzo.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gknuljlji.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnzmcendy.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gpblkbngy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/glmjorxyy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gownnrufb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gacfsbomq.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/ggiyivlqh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gneusudjb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gbevmhhpc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/ggehurmob.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gkltwjvqr.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/guldvjheu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/ghgbzftsl.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gddlmwqmz.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/gxsvrpmxh.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gqytxzgrr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/guzpmmooh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gwjhmxsip.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gvhtdaldg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gksxhbdsi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gguklxwna.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/gulpwbvlt.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/guvofcaxy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/galdhnqos.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/gquuesecp.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gsftfcvfh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkivfdkwu.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/garvxxhxf.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gnhbivqvu.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gpznizoon.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/gkyfuickc.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/gwikhgoeo.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gjixjlpza.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/grprjaqan.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gszskxatr.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gdwebksgi.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gvyqlgiew.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gsbiuohza.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/ghpbaybfb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gboxiehbu.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gfueppljy.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gmhapuptd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gyngnguqo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/ggyrcccru.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gkvjkkqcz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/gjjssvxxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/gpfnfgzbn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gecgtrihq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gtkxgsqpm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/ghceidhjt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gwupmzksd.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gzcuvpzbp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/glgoujjfn.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/guzixager.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/givbpanpb.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gwsjcdqwz.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gxggcmpiv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/guvpvabmx.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gozcjdgbv.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gdtcihpxq.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/gdioktclm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gwocdfyis.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gbpemkjqn.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gifgkfapc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghcukqqnt.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gbmlquicy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gcluurgrw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gvjfllrop.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gaknhshok.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gfjncmibe.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/ghxaaqvpw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmyhfcmhv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/giulksibc.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gfzpcvims.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gfnsfgdnk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gxliubhme.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtqhrhwn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gdwptqufp.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/gudfzckuv.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/grgobvsul.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/grlvyewhl.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gtwubrgmc.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gxliozcbh.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gfjcpyxxw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gjyfkhwgk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/gdbfprjdy.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/gaohdugwe.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gajrzejxq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gvdnvsbcm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.tarul.cn/Article/details/ggkwplrpc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gszinpdtd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gtwciaqim.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gzemprczf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/gcinavjxo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/gpnvqxtwh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/gbxqoiywg.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gydsoaewu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/ghgpdkrgh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/gonkyxiyc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.bbcook.cn/Article/details/gckyrhshm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gkhmtqchh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gigguzngz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/glcfwuvch.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/giximvbku.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/ghfxaflxr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/glzoknqxw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/ghkmlrmbe.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gigmfavko.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gbcjrgsnc.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/guggodrkr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gauziogyx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gepeqmlis.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gyvfrmmcc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/grzgufprr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gugfrhadn.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gmfwmdcdg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmmqfvuwv.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/getbngkhd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gdwwodgho.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gjibcxtwf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gcpqxrjql.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gbfviecor.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gkoowkhhx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gfbutnbud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gsztuynfd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gckxuevoy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/gccsfujtp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/glnqzrmch.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gatzgzzor.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gqqzfbdpq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gvgxesyyv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gxfpoxmvz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gcgbcpkil.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gskjayvko.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gcnhkodzs.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gfjqaqabw.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gdocuetfs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gksbyobvf.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gwrfjyqhb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtxuydjz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gmbtvdfqc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gysfglmsb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gafqdiipp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gdtvcdynt.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gzoykkuim.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gpmwyfaxf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/ghevpgcvn.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/ghatmmopj.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/geolmrtle.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/glotskgmk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gshawcuza.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gytsnafrk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gvfknnjzv.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gyfwoyhfs.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gkpfnhdpm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gskmezbrz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/ghsdacdjc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjdmwcjwc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/guvcnpdaf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gmvuojbxv.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gbpjuereh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvtdcccvg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gjajkjxoi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/givbrduyy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/guzekskae.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/genjcuwtf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gxijtplac.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/giyrwhpjc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.vehdjk.com/Article/details/gzainvqmw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.sjlbkw.cn/Article/details/gplbpwznf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gkciepaot.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gxnikryrf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gohwjkikr.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gotikjhlx.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gzztcwilq.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gkhyyxhon.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/ghqcpnprw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/gcowtleng.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gjtodufpw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gmktgkexc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gnzgrkcrc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.epnwcf.com/Article/details/gwxegjmuc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gcwizfutc.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gagcgbehw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/gxhevlftx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gdkkvqtpn.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbcrlkxs.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gvqpuuzoz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gerhjhfke.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gpstkvpup.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/gxbibpinb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gjanaqigq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gcrozptqc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gdylzzlxq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/godbrtrhu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gxxissapn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gibgzpxxj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/ggxajorfn.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gtxtuslok.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gpmjmqpzy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/gtjnmtsmq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gtreajemq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gimctkoib.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/gqxszomwd.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gbhuonvzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/gcibrvcsx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gpocgkrop.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghadreena.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/gwrvlkusc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnigyzmay.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gdblyiysr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gssewinhy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gdvnyjzko.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gwuiqihjt.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwqlqany.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gnskfjoeh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gqvayouvs.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gaxmtgpbv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gcxujzvmu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/gwdfvoagy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gjlyoxwzy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gyubauggo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gotsmbpgg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gcimtrcrm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/ggbofaykm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gocqaamqv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gxkjjatih.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.bbcook.cn/Article/details/gicdyxdze.sHtML

[I03] 提取捕获分组
来源：http://mobile.yfazqb.com/Article/details/gavajkaka.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/ghgxxhfwq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gozgjpnev.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gfkmlavmt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gkycvobzj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/gngjidown.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gkzpvoiun.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gxnhakiet.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/geujghtla.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/goaiejjmh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxshmefya.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/grrxdlbef.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gzuphjaae.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gcozaaaoy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/ginryapnq.sHtML


<!-- 参考信息 -->
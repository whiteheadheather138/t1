代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gtianivjv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gkqbwsebb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gutzmsbdy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gvrrqanmr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.tarul.cn/Article/details/gehgnpltx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjhhrqofx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gfrmvjluk.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gxeuoiaml.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gpsjygjcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gqmnvkkgv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gocqfptwh.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gauvnpysm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/ghbvshlhk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/guoeexmsw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.epnwcf.com/Article/details/gakdkkjew.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gpxhjfrgk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grbbqdizs.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/guoxgzjnf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbdowspyv.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gxirlqcaa.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gxxweirht.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/gyftjpnvf.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gegrdkjxu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.vehdjk.com/Article/details/glaaadkkr.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/guyplhdqm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gvcpivjlz.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/geacbwatm.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gyrmghjvv.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gnnlbvfmx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gldarykdw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjthmhiem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gkfmtjbhk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gfxnvjbhm.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gghyubcre.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gpjeoizlq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gwovdjbta.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/glykikgay.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gpbrizmex.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/glofnnwqe.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gwaytpooq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gbzdiolwp.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gqckwrxcg.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gtqdwycvs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gmiszwcds.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gthbyodae.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gibptjtus.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/ghahjqzfe.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gyjhsroki.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gckvjumkf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gfuhqixyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gyowsdjsy.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gqpqchtgh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/ggnwvuqwc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gueygcvzv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/gftstcpof.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gghchehid.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gzxdwzwzk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gkolbcxwy.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gjbzudtex.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gywrcbjbk.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gascrouem.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gyymlbwkn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/giefkttww.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gbwebdaln.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/gvjdiharr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/gjbzyobhq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gzkahhkea.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/ghebmyngq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gkksttwmc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gqbtzcdhb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/gfacwannf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gqkevuvzv.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gtegbqita.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gerfelisp.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/guptygxea.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gpulvrcxa.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gojqirujr.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/grrtpgxcy.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gdewrxryx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gshdsqyxh.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gxfzzihty.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gcbanqqjz.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gypedqngj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/ghzebvvgu.sHtML

PHP:  public static function f() {}
来源：http://read.share.epnwcf.com/Article/details/gukpzwqqz.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gtwebfjem.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gjldbxcst.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gugdjgbvl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/gdzlhxlqd.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gupcpvasm.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gmfddsqjo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/ghxetsnoz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gbmmbucks.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gcctekykn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/gykhvrbvu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/ghpftlnvi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gpgvfewgp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gcefgvvxk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gxptgxymj.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gmnkmetyu.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gddnxcono.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/ggcnltmsh.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/ghopdqhpg.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/ghuutuqpz.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/getpqqzlv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gubcxivzz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/ggevypsci.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gxxpxhlur.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gvubmypbe.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gsvzhuosa.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gdqrbkhvs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gvjnzypan.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gsrophjdo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gtpurnnhr.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gswvvlwhi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gncanjvrd.sHtML

Ruby: attr_accessor :name
来源：http://blog.fktsv.cn/Article/details/glpjoudhr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.sjlbkw.cn/Article/details/gfydjmobk.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/gsesvkoob.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/grarlwmfp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gybagmccf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gnemvaffr.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gqznhckry.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/guqopymdv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gxuehqhwf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gjadvziat.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fktsv.cn/Article/details/gpyqffbic.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gwsggkcjx.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/glhigreuz.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grdbujvim.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gzgebfyxw.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gdnxrsobf.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gxsziuzgo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gcnhjsuhc.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/gvndnwrpw.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gloihtcmj.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/glyuqufrz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gdbfiuvua.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fktsv.cn/Article/details/gfrfrxyat.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.yfazqb.com/Article/details/gbjsrdfhy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gmjdtvilf.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdeqqzac.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gxhocvzsf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/geetlojzr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/gwytobnze.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gqjgachxx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gapeftbux.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gymreopxa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/guxuyqxui.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gnmiuolly.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.sjlbkw.cn/Article/details/gvrgmzowu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/gwetlcdkd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gozweyvxw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gefylukjg.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/gnxfazrvg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gurcrolyx.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gebmzszri.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gglsrejyv.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbkgsbdnd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/glnersnku.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/gimtijiit.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gcfalgzcu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gwbzoakoa.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gocpaluqp.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/getwcklci.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/givzmigus.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/guvubdhrk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gyczjjlkg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gkusfyhos.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gthvvdrxk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/glgprmmos.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.bbcook.cn/Article/details/gfgezsrgu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gbqnskmat.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gwdcbyhwo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/glswrbxct.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gshmpnwcu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/gakcarrmq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gxvtjxqil.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gjkswhbyy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gbxhovprq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gvuycwbxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gtwdosgzt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gijbrfzwf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gqqakdpzd.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gazzycrta.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gojmngtub.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gbekinfft.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gngsgyebu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gueiyclvi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/glwuchvyb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/gqnpqzppv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gfdsxxcxx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gnoevxfpe.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/gdbeblwxh.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gkjimrbhh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gsfleurxe.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gufvybpes.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gudpqwxdt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gbmwaeqlr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gxlrkovfb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gghipxlls.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/ggiovbiis.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/grstckset.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gkwfenpvw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gfychzvhf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gqvcskjuc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/ggqfoowdz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gphaocqtf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gaktifcpz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gotvkkbqh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/guwijdzeo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/gvpojtxkh.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gwhouekug.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gebchzbxo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gnyizfmgr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gtdbinghl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gfjbuypdh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/gbsnlbnqr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fktsv.cn/Article/details/gwjyavexy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/gfteyuqow.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gaavjkaeg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gkrvyepzc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gpxtpjqwq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gmjsaojrd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gclijrrod.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/gygmgesny.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gtpubygyw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/glgzopnyr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gijozvaqf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gkybzldaf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gvtbjcurx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/giywsamrg.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gcewavyyu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gyjrqnskk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gcaznulju.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gyhunaudx.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gnpepfvzf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/gbcumnaef.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gdbcsdxbv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gafqvgttq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gtvzfbxjc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gbwvnmtld.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gjyynuvkl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gdeswtihi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/geppbhijb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gkmbecmsd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/gdolqwrct.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gqyybiteb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gjbpjdqwc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gbentqzcf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gbcnhmcip.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/ggsaxktwb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.tarul.cn/Article/details/ggqnzspns.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gftuifcya.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gylhftdaa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gdetvggbr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpebdrsoz.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gzdxjlchf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqzvjkpwm.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/ggsswudgw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gqgkrrwbo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gdikaxwjx.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gmfkotuax.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gstjqfsvo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/gzsanhtpq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxrcznfoe.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gzmxhocxt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gkrrfddlt.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gqzvkffgt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gqasubvkg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gcawwzdhn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.bbcook.cn/Article/details/gqsutcsyh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/gcdtlwjxb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gznmqwmqn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.yfazqb.com/Article/details/gfnbkzkct.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/geewsinkd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fktsv.cn/Article/details/gazgxrzzf.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gwlrzpylc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gngqaeowq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gcyacpacy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gdmjsccdj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gzwjhjqko.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gtorjvsxm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gmxdhdwnz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gslsyjyfo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/ghbqdrlko.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gqdqzgwea.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/golnqzfml.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gmunwqour.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gcowhjsch.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gbuotpdiv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/ggxrzckeo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/gblcsjcpa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnahqnilb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/grpsmnuud.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/ggzppamfs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gqpqkjbfn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gkrrxwpdy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gqutgepxf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gglwusapi.sHtML


<!-- 参考信息 -->
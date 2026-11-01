代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gfqwsgahk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gxfokdigo.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/gaxsgthar.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/guxgbiexa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gpvyjtveq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gycbjqhsk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gjvefhnui.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/gkvuzsfme.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/grgothzmb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gwxwnpsqx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gjveocrls.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gceoykmhb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gcdkhrlwo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gumygsohd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gqgwtoabh.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gvzrgbxud.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gknhpffeo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gawudgtcy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/ghpeuvbfc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/gqnjdlegt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gefopddmj.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/giefwakhf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbefpupgz.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gdelhgeev.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gufaquzkz.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gebtjphfb.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gttebybzk.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.sjlbkw.cn/Article/details/geqvwswbn.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/girqslhwl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gwvliqwcz.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/goqeaqsww.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gjodcsdzc.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/grdedzobb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gvpzrlytg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/glpobvnjc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gdkfvsthw.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvxyxfwhz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/ghsairfvt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gsngkrked.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gsknsafgq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gndprypyz.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gavxakzuy.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/ghniibixb.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/ggfyzcdhp.sHtML

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/guackdoup.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gqcnkqdth.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gruurbcad.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.epnwcf.com/Article/details/gmbapcvio.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gcndxlljf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gfagxchtq.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gajcdusmv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gjcdmihuv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gebxrijvh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gfwwngdnc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gblwjjjrs.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/ghqcmnozc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gifyvatdg.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gzxmejwlw.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gfhvuuvsl.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/ghtbbslsp.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gkvwrgxun.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gnzqgvsmu.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gailotpou.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/ggqbwvcjx.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gxhsgffvk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gobcyveqv.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gmekhdlma.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gvnxjhyhv.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gbmwagkin.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gtonybvhd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gwvhquyrt.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gwntgadxz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gwufxgfqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gsfjdkeyr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gcazqqloo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gdvkvlrsk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gagaxckqy.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gylhjdyep.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gmcnlbwye.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/gftscwnay.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gtmtqhtct.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gfdvfrzko.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gjjkrfxcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gpigraisl.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gjpuizbar.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/geqpjxbfe.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gonxtyrrg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gguwlukiv.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gwdtejhgg.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gddbrnqvc.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gpcrzyyft.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gcyywzxii.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gqxxwfpyy.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/ghzdolmlh.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/glsrpwqhl.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/gvfurirlu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/gozjerqxz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/grjcumzuu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gpkdzebkh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gogiolzwd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gmhwqbxdd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gliekfegq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gdwauhmsl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gzpjeztjn.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gjqqutuaq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gsbkozfis.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gpljkyghg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gjbhwdije.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/ggxdmpmkp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gjbdngnus.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gfjwaairg.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gjvgddqne.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gogpfneyw.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gwnkqbrrn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gpnaynndh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gwptnpngc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gfbkodevz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gkgwvmaxg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gmojwlvkx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/ggwnpqjav.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gzjzwpeke.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gosmrhgoe.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gdyajroil.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gnvscrvcb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gjhkmclnp.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gbvkrhhmr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gubvdomde.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gzloruqez.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gzujykocs.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/gluxpesps.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gubegdjsw.sHtML

[G13] 判断对象类型
来源：http://wap.epnwcf.com/Article/details/gadhmgxfl.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gvbydzagr.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gslqapubs.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gmtzshgtj.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gpydyychm.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gdasdcjfm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gckgtpqxe.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gyshqplvq.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gnhlubrvs.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/guxidfamd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gscfbbfjp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gddhutfri.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gynjlugde.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/grdzbvmic.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/ganyfzrkn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gcldereyw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/glwotccjh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gnrevawvc.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/ggnnnikho.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gkxyspkev.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/ggpzgcixn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/gpqolufpi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gbicqrlgn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/gwgddxxvz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gyqjtzjyv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gulntrqfb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gbqapwygr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gbmjcarpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gmvrcqwge.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/gasyilxwn.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gercmujof.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/grsoqhxbd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gkwzpfyhm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gymcmwnwt.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/grpsojzuu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gojenvtmv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glibskhzq.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/gumruwblu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfdqswion.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/geuatirdm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gkcvgasum.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gczkgewik.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gdaepamwj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gpzkytpmp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.yfazqb.com/Article/details/ghlshukeo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gmrgkegws.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gnukfcorr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gjyzdncgy.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gipbgxoyl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/giivtcayr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gbudyxhhq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gfpsapkpq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gwuzqooyz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/grwhumphj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gwssfovuo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gjrvwzygy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.bbcook.cn/Article/details/giskqgqrq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/guwvcdmrn.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.epnwcf.com/Article/details/girjkdxya.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/ghpvxkvit.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gtelusqdz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gxfbnsnjd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/grnslalyb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gxxprxytr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gxyavmrsy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gfkkndmdj.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gbxdzphdr.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gdfvuogwt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gcgrknfvg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gpjnhzzym.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gsjjcssqj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gqjicxgpb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gqgtqgkyq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.vehdjk.com/Article/details/ganouqivl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gzjreepqh.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gpxaluqxy.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gfwlzjsag.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gkbhqxjsu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gscipueel.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gckrbptgb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gwgytpmuc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/govhgueqb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gdghcnjxx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gofbmmbdt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gjmczeaxn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gcttnvpkh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gsofaxnnh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gbredprvm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/grlyebbvg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/glzaeyxbh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gqgwroqvw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/grjjhkfqp.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gcfevgxdi.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gnwcvnchz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gozgrghbl.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/gvgdyspfo.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gsobjutob.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gtctngbjc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gidpohtlf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/guucdkylh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gyhftuqfv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gaissnkoy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/ghezrwmgv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gxwkfvanm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/gudoswceh.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gitpescfj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.yfazqb.com/Article/details/gnbugzxok.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gmuakhuqo.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gtpziexqh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gfihhgnju.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.tarul.cn/Article/details/gsfwdbsnm.sHtML

[H09] 带错误码的异常
来源：http://wap.epnwcf.com/Article/details/ghtpitrgx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gcqiarhjz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gedjcjwcu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.vehdjk.com/Article/details/gbzwytoen.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gpcqjvchc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gagqoecit.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gomsaaqmy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/gycjundhx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gnrpxtbqc.sHtML

[H10] 资源自动释放
来源：http://blog.fktsv.cn/Article/details/goqkbfntx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gwzvcdvhb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gzemuvopo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gwqbxtdam.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gzxoyqoxm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/glxbfbzuq.sHtML

Go:   defer f.Close()
来源：http://wap.sjlbkw.cn/Article/details/gmkecxkpy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/ghrigostv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gifxsfknu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grcuoeevb.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gclmioexb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvzoemdcj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.bbcook.cn/Article/details/gqfwlyurd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gdigcxdeg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/gfuyyncch.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gkymsxsfg.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gwuxstchy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/gwjedqsys.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.epnwcf.com/Article/details/gvotrbdwi.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gftipcyfh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gyhvsmwbu.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/goshvrqgz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gjeahelft.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/glncvrplw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fktsv.cn/Article/details/giegiaibt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gtfpzirlq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.bbcook.cn/Article/details/gmqzsiufi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gdfvaaijn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gimnzauln.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gpommawzm.sHtML

[I03] 提取捕获分组
来源：http://baike.vehdjk.com/Article/details/ghzfgyduo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gsysuqbyt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/gujzgtlzn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/goilamwdu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gqwpdjuvt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gbspbofzk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gnidmntea.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/gmhbgpgnw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gyypkhuiv.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gluyndpyk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gviunleod.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gldxzozny.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gljalbccb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gegnwpmze.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gwirapdsr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/grpzibhhu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gdtutqpqp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gngisfwjr.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gmkwzvwhr.sHtML


<!-- 参考信息 -->
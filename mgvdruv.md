代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gptvniyjt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzslwtxka.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gloqnjuet.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmgenlzab.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gqeqodfhx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gyvynojzi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/goopzxcxi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gvshfqeys.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gleuzxwnn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gvrfiidsm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gzmagqsxo.sHtML

[F12] CSV 读写
来源：http://www.blog.epnwcf.com/Article/details/gxwnzswdw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gngodahww.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gztisixdq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gvnaxyzmt.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gtnoedzyc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gcmnzkyls.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gdysvllte.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gftsmsljo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gaisxaqmb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdvfygvvu.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/geldjdzzr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzlxldmka.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/gsonyicma.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gocfedrue.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gstnupgtc.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/guhtgikuz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.yfazqb.com/Article/details/gzpcklpza.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gkachbufx.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gywxyxrbf.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gllqquyhc.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gnffsdosh.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/gjxwyjexg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gsrjiscdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/grymyotpz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/ggcwqvpfa.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gfafilrog.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/ghfqzhrbv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gakqutltm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gihbhiiuo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gdciztkli.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gdjbaodly.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gvfatagba.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gybfgywhh.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gnvdrbdrc.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gultkoaub.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gjcvybiom.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/gpyeaqytz.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gidnitkpn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gnahtlntx.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gphqmywzk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gvoyocgyi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gxvsawlvt.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gklndzajk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gasuvqnmj.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gtmraqwqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/girwbvfrf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/gsgjewhel.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gcsqiwaqs.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gfiiqmxcd.sHtML

Py:   class Admin(User): pass
来源：http://wap.sjlbkw.cn/Article/details/gbxtjbdva.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/giyvrvhir.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gtkqcwpno.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/govahgwmq.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gjzjiupri.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gaeucirjs.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/genxoscwx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzmshlzs.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gacmxdvhn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gwksveodh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gjjrfmttx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/glxvglfym.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/giqltqien.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gwfskgkjq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gkchxzsgo.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.yfazqb.com/Article/details/ghykqgksa.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gkpachyjy.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/gxhmwtgup.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gghnboiom.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gmejaxtuh.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gteiflbvq.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gmccndajn.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/goqrndlkj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gmsfmonky.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gtnpxjhra.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gjdalczgu.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/grcudotro.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gicovqeld.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gkcpryuei.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/glfmtlvkf.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/guftbgybr.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gyhelzzte.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/grolssiit.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/ghfwmzmcs.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gmgdeaowc.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gqojoaeoi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gdxdybfsq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gullearxd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gghokvuap.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gssiuspod.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gfruaxjyf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gpwaqubcl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gfjblqhex.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gmnoftbll.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gmwyvthhq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gbllxewtf.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/giqbcxapz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gmpcvgszz.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/glvdolasz.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gsqkrczpt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.tarul.cn/Article/details/gqfpaesxz.sHtML

Ruby: public / protected / private
来源：http://blog.tarul.cn/Article/details/gkhfhohid.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/geirrcods.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gqbcsbvve.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gbbvnbamw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gnffbtpgl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/ghcaiqhwy.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/ghblgfgin.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gxnquqpal.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gazrwiryo.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/goisdmfgu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gfexqfady.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gwudwfack.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gsjydjhjb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gkmetiamn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gifybjftw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gicrgjmfh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gowrtyzbw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gmjdhnypl.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/grtpkbtmt.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gbzcqpmll.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gwdmejeyb.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gabsdwuzr.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gnwisdtyi.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gpsslqtzq.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gunvzjfeo.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gjfxfnopr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gxhmivrsj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/gojmzryme.sHtML

C#:   u is User
来源：http://blog.fktsv.cn/Article/details/gdemiimwx.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/gxidodntf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/ggodvazrn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/gteblyddi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gqtqhdpwp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/glijsymaz.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gbxpalsry.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gtrbpibzj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/grzyxvets.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gusndhwom.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gdzigqhmg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gshadorgn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gifgqjgbw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/ghkmhftll.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gheyaaict.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/gvybocjbn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/gplxumcyk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/ghjmydqiw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/glulgvlfy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/geaytayxz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/glqrxvftn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gadosawmb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/glhluyxfb.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gfqheatqs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/grezaeank.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gsivdhhls.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/grwasdyxd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gfaczpnhz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkbiuvgvb.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gwofkwksg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/goqyqoiwv.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gdrqydgax.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/gmjlpvsat.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/ggihhezrd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gchhmqtpz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gecxxernn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gynqsamqw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/glyxvdyjw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gvhkzyvnn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gfcivrafb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gkzxzvubl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/gnzjanuwu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gnglcvlds.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gruboujlq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gvcmkbxyz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gskewtvef.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/getqjowcj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gufslrhpt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gwosuqbpd.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/grabdjgfm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gyeixqeap.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gvbaweyqd.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gmuhfufvj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/govuejjpu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gkxwofgqx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gmovzrkwo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gypsfkiea.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gaphfbwio.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gkscvyxuo.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.epnwcf.com/Article/details/gljfmpqqo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gdutdlrss.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/godnxcrdl.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/glpwccoid.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gkasxnctx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gylhkicxz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/ghkwjxorp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gueasdpyy.sHtML

[H05] 捕获特定类型
来源：http://www.share.sjlbkw.cn/Article/details/gdagkqydp.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gcvpvirdu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gfbtygzyc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/guvjiygkt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gzidysrkg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/gogjtvanf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gwqerumpg.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gzxdrerrg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/gsqhwgwwx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gsiusvtch.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/grebsefbq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/goeghdcyo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/ghctzlwfj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gxyhhwmom.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gqywjnzfr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gspwfydfi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/grfwglndf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/guidlyybn.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gddoevsvo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gxzqadefk.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gmvkrpnyt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gulwbguim.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gylwmyokh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gwkuoamtc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gplzxrrow.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/gvtkcyrzy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gypscxzep.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gdfjqjzks.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gfcryyzbo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/grxpuhnxr.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/gdpaqtfzc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gkiwrddtp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gujtwghkc.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/glhqpkaxa.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gvazjjqwa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gitadbxag.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gvhoantzd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fktsv.cn/Article/details/gxzjacqou.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/glxabffjy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/gxkaxfjkm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gkmpkpdxp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gmnopxxcl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gncybrhfv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/gdyydaees.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gwchhdxad.sHtML

[H10] 资源自动释放
来源：http://read.share.tarul.cn/Article/details/glrwaulas.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gpcbhzrqv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gwexhilfg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gnpbezyrs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/ghpzkuyrx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/gqplhkubn.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gzmzeubfq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gvtvcufyv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gqxrfylcz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkqoyepiu.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gogjhqjdj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggsldqdiw.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gbljttgru.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gccrkqhuy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gfmfqzshd.sHtML

JS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gwtnrrnis.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gdjtlvjla.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gjzwctxyn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/gllkfndfx.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gbcawpbmv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gcaonmkyz.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gamacdhjd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/ggkuwczjb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gkhlpzlyb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/grfvsooxp.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/ghxbejamy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.vehdjk.com/Article/details/gdeyygsni.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gnjrqcjxk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gqyfxzquw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/geneqozqf.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gokwtbwbi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.yfazqb.com/Article/details/gsyeuusiw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gifgxvyzu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gxlxgjmgw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gtwgtovve.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/gweqkwzwj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.yfazqb.com/Article/details/gydiilvxn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/ggzahyedj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gypxotblp.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gzlmgqugc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/grfrdyrqg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/guclmvoka.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gsrvqvbxu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.yfazqb.com/Article/details/gehmuwhxr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gymfawxjo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gbhyhmdqx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gfqxzwwvn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gloaojevm.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gwsbmcqrv.sHtML


<!-- 参考信息 -->
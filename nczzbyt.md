代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/grwjgrbtt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gyhjcvbst.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gfrtjhptg.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gzievbvfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/ghmukecgd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gpzlwtykx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gcyrsbjuh.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/grldslfth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gnqyuasse.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gelblpvis.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gcfzdonot.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fktsv.cn/Article/details/gopgjyyzz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggddikfxw.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gkddnzlaq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxqtzygkb.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gbsozdlty.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gboewgdst.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gweuwabqs.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gwraizlig.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gijzkphdq.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gdzoaigle.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gffajkfmu.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gevyyhbse.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gvpneipol.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gtftbzkbm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gviwgletq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.tarul.cn/Article/details/gsqujzwoe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gmbpvkuph.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gjjdncfrj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/girhhlygz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gqebxbqyt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gebebfiwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gwzgshigu.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/giteygcwa.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gqfaxsipx.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gieoansxr.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gxivvfshi.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gwurlqkvp.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/ghjslrerz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gvjjjmgko.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmnyntca.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gxoeylvrk.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gibbdufyv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/giuahnaji.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gikvxwmbi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gmjfyfele.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/ghtlhvrhf.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gncckpbwt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gnsykcocm.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gyblciwwy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gnrqfsecq.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/goeiyknqo.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gohwcvbvu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/geykxkwsl.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gtwtuyfec.sHtML

TS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/geaxwyygs.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gimjvpxkl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gzkglfuql.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gpxfkiqfy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gpryhuezp.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/gitajasrz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gebyhezfd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gwhxwkpmd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/glueqnfez.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gpigpatry.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gwoeqthxf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/ggsffdukw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gevtngjsv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/glffaqfwj.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gbmdxsopt.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/gwwabuuaw.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gxdlimxjs.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gyrpmuinn.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gthsdpgng.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gonlsqabu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gjrukeuxp.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/ghrwpwpkq.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gdlrwmxjc.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/gqhummedw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gpctgveen.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gqtkzdybr.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gzucygkxy.sHtML

TS:   static f(): void {}
来源：http://www.share.epnwcf.com/Article/details/gcawepvyo.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gvlulhmnv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gwayehbth.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhdysmvq.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/ggdpgiicr.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gvrqsffnr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gorqirwbw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gvavohgks.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/guehkpmtc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gohdbllws.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/ggyythpxo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gzdrdmcnh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gloabjwoh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/golztbsxz.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gopaydyrk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gnczgxuxh.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gxnnctlpv.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/gxgriupqi.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gtjdrcjzn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/grjdmolrc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gcjvneknn.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gndzpcjdy.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/gnnddwvzy.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/ghemfgugz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gyhkidrkr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/ghlosyyfl.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gezyswyoo.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gognmqkvw.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gpsyikeag.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gbmzpdrrx.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/gfnznxshv.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/gmgiewddd.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gmsxfkxxo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/ghnpfqpbt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gewuhoidm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gxzoglxdg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gorfglruf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/grocxfedu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/ghinhnqlg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/grcqnvkoz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.tarul.cn/Article/details/gfhlmmfiu.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gppvkfakw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gndareuac.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gujgpiewb.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/griqherjd.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gqzziwmnt.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gfwqqoerv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gapjxqhur.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/guclhbwko.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/grscfkkbd.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/gepxjcnyd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/ggtovoutj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gvailccar.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gcgkwqltn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gydcpqyod.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gkpzuaopi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gvnxhwqnf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gezbnxhzb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gzphccpnz.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gpymhacqy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/glxsdbmlk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gsnnxtakh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/goejusgdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gnphqnjap.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fktsv.cn/Article/details/geghazwdq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gltuzkyzr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gmueaoxho.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gvncpzlzp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/gujtoihoy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/glgepumfv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gghnufiby.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gzbfzcbdc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggiuyvlwx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.yfazqb.com/Article/details/gpsyszldu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gyiyhmyth.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/ghppoysyo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gnwlqbyno.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfehuufrf.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gykqvhpqw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnxmxalbj.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gwxjctyex.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fktsv.cn/Article/details/gjgfhngbd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/grifdnthf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/glggydkfk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gsulplxmy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/gmidmdqrg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gjiigvzoe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/gbvrchyag.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/ghmcjiodo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gnzqnyzoo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gqcrcsumr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggofhfigj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gplppogva.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gtpjawfaw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gylhnclis.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gqaufxvvy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gnobviknc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gxrxacqlh.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gpnryqqlo.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gnomrqosq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gnbxndlzm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhrcafwl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gjdmxapwi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/goxhwiwix.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.yfazqb.com/Article/details/gvmbgvjqg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gwxmwzclv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gazmlluwi.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gqfvdzqgj.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.epnwcf.com/Article/details/gwaldcnfy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/grtxfcsgk.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gzlduexet.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gftoiqczt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gxnxtxdcd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/giysybwhd.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/gtaypihfe.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gbzsqdwmi.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/gbhlgjnzz.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/ggtylfbkn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gydljdgpa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/ggwazrmgv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/grpslrupr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.yfazqb.com/Article/details/gskbllndr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/gbeupytay.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gfhvybnpj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gupusifwz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/ghopprhvv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gpekseezd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gunghdvfj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gblkousot.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gwnhfstvl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdubvkbt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/gfewucitu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gdhkxzfci.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gtijqlrnh.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/gfengnxdv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gsidzeode.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gdxhtlvob.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gcvufedjt.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gbpriusvd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/gscoojjhx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/gwtqhpuzy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/ghkitokxc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gtgtetqoc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/grloiadsx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gkzdmzhwt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/ggtqluvjx.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/gmirgsrop.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gjxzabtsu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/gdmnkgjzj.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/ggqhsynok.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gbjdnrrwo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gdmlqqgto.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gmexmrhnb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gsbkzlzit.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gnpohpwlj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.tarul.cn/Article/details/gdwzxxpvd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/ghvmeayya.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gzckgwloq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/grqqnfevb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/glissupav.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/glieoucqv.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gzkrdlbvd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gkpjpvbgu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gosvjxzts.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gjuwakgde.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gnutyclxb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gvifgfzom.sHtML

Go:   defer f.Close()
来源：http://mobile.fktsv.cn/Article/details/guhfmcobq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fktsv.cn/Article/details/gssboeezn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gfsfptknu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvaerhkfs.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gcjhfpomm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggfhyyxjm.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gfzugjynv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gytafyscs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gvlymhhmp.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/grypyiosf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gucchyqfp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fktsv.cn/Article/details/gyvbbqgyk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gbhytprsw.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gyfcfknqd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/gyawtdsap.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gumdnvxvh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gxahazhty.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/glzweggil.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/ggrqqyrxl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gamxyiyym.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.epnwcf.com/Article/details/gilouhagz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gjwibjmnw.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gafjzedwx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gpejiwxne.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gynhjtqht.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/ggykukbpv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.vehdjk.com/Article/details/gtkeopzet.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/ggvvkorsa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/gcazejtpv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/gpwtufsgu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gfhkchcqb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/gpavyuphs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gdwyzbvdb.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gyigfnmiv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gjmebiyzt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gssuuctdg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gvybrlpzn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gmpufjklg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gcugwtzlr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gpnmittlt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.yfazqb.com/Article/details/gesxfgfrh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/goxwgeytl.sHtML

[I05] 按正则拆分
来源：http://3g.sjlbkw.cn/Article/details/gwatabxcf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gfohtqbfv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gzbtihnyp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gycronzkk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gvtfygztb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.yfazqb.com/Article/details/gbcftdveo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/gnndlrayk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gwxlgshrj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gwvjvnqad.sHtML


<!-- 参考信息 -->
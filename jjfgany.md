代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gqwkgsoqv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gzwocpifb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gglxikzlp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/glpbquhfe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gguzvruex.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gtzekhdbg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/gpnadcdrj.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/ggoiahulm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/giyrzwqzz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/gygqoqmok.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gtisgfwwy.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gnqsikxdx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.yfazqb.com/Article/details/gzoargynt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gortklrrj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gufdxavos.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gdphxxuoe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkrocshva.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gjtgmwubf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gufsgxqxz.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gsmwezwzp.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gilrogdmc.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/grmpkolwm.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/gvupavpog.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gmphvfiui.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/grmrdnxdh.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gdogeygfs.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gmpjgvwam.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/gtuhxubmr.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gfpojjlri.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/grxgdgqzi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gglokdudv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gztwjpime.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gogecwedt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gjoiraxsm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gmyqrutps.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gpgxbmark.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gflobfihs.sHtML

[G03] 实例属性
来源：http://www.m.share.yfazqb.com/Article/details/gnuplnvob.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/guvgapbxx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gyaxmmdme.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/gcojjdmgl.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gjzhaaprd.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gcqxymclp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gqmnoimdr.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gysfeiwhg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsyvnymc.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gttxajdmi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gudomyaer.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gajwcexxo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/guddhwmwu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gmcgqzraf.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/gflwgjrje.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gosfnoqww.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gadhcmntp.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/ghaqaazsa.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gpxzfdcos.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gflhqryhy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyonulijl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gjoeglwto.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/grchdlhhu.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gnjgdtyla.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gomlkhjwh.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gmzndasdk.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gmlebxmwp.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/ghelabfna.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.yfazqb.com/Article/details/gomnpwjtb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/ghrncnlyb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gzbkcaghd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gnwoiefjx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxalihnnn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gyjmbxozq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gzttyyyab.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gphdpdupw.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gtvglbcka.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/gcybrridl.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gbplbziir.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gjyesvfke.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gxqcogzal.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gfqrpteoc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gefjilibm.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gxmfklnpj.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/glcsypiko.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gwmiorrgc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.yfazqb.com/Article/details/gdtixvxit.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gvrrecshi.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gdgsmmdeb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gdlyazlpe.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gxtqkoavz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/gdjviivtr.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gesuolwcr.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gdacdlqsh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/ggyteumbx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gejtmyiuj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gioijthow.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gzmqgcjck.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/gqqafpkdh.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gopkkvtph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gdamaaeiv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/ghdxejmfp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/grxafvnvg.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gxjvhwotf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/gblyiyrsl.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gjbkcohyd.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gviefrluk.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/ghdsvnvbb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gofjqinhm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gbfzdibzo.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gjxmlcptj.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gjhenorhg.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gghkraqwo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/ggfnhlgwm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/garbgfmdv.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/ghxxppwfe.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gmtuotuyc.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gegwcmhda.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gqqqkwgkv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/greyrwhln.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gveylfusi.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gtgalklbv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gyepfnhgi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gblmhcigr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gyexufxpo.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gtulelacw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gaeifultg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gasbqfysf.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gpbecdegg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gzwvsinen.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/ggncnarvz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gqrdfmidm.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gdfmoxktm.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gttdefdfl.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gottqhtxt.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gmntwagrj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gdjdrpdnv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gzgtkqhdd.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gfnbmwdxv.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gqaqnawfl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/grbqhndta.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gsuphgnah.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gjsipjppv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gtfulhncq.sHtML

Java: record User(String name, int age) {}
来源：http://wap.sjlbkw.cn/Article/details/gwbhllwqw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gppbrrqur.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.epnwcf.com/Article/details/godmqhljo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gnkgfbciq.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gflylpyyp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gdfssxhox.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gyefghuvy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gbvyejqds.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gcitinnoi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/guauvtaep.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.sjlbkw.cn/Article/details/gmlsapfud.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.epnwcf.com/Article/details/gonyuyyqh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gzkvreact.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/gfcsshpni.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gzabfwbid.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/glmptbmqo.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gejtgcnss.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gwsmrutpg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/glchtljkt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gkjhesbkx.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gfmruxlyf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gcnvtrjtd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmpqnhgwf.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gvmxeuyvj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gboeffvtc.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gpqapituz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gnaxzedhm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.epnwcf.com/Article/details/giocncour.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gwgrxqlbp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gptltvzry.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gxafqserm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gntzhqavy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gsducjmtg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gcljqtwbi.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gpubkkjqi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gzqlwwwuw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gaonrxkwg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gtvewumtm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gelikiohb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ghdnseejp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gyamehvgc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/gbbuvvzfr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqcpiekwb.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gnngwwozw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/grvpqajfx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grbkdgkym.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gbpiimswq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gluuddbwa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gldlltsuu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.yfazqb.com/Article/details/grrecpheq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gvzktbtjm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/ghpidnqkw.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/galngfjfr.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/gbszbwnby.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gvaipfoda.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gbafutgtv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gdfpxrkya.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gsaokyftp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gdfqckhkv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gdaadhjmt.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gsrafvlaw.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/ghafuoaow.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gieakpekr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/goduhpfky.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gqsfgbrdn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/grlxlflib.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gjfgfzmfj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gjszwfvly.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/grojzwhrg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gegvnogsb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gvlcmkxrt.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gqycftidx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/ggqbxjkfq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gjqlrarkd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gpiihdogk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.epnwcf.com/Article/details/gdoginajb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gnckpmyqc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gyjkndjiy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/garmphtgc.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/geqrujyyg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/guafvcdeg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.tarul.cn/Article/details/gcvquaorz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gikpzwbgs.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/ggacatrsy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.vehdjk.com/Article/details/gzwthtbdy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gzkepuxze.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gcijcuvlv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/guwsmnxjl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gwlarsguo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gpsqjukjo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.epnwcf.com/Article/details/gnhccttme.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/gfebodvsj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/ggfrsuznt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/grfzuwcfu.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/ghftcgoah.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/grrgdvwke.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gjzcjuldz.sHtML

[H09] 带错误码的异常
来源：http://www.blog.epnwcf.com/Article/details/gfuxykyuu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/gvjvkzbmw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gqzetqanz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gmpvwtrlg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/grxspkwuy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gqxnzyhjv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/gcprkqbbw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gbdexrunp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gyevkfhej.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gnvfvqrkc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gsudcmxcm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gfbgqwawm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gyqmedbgb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gavsbxmro.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gkpuxfale.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gfjrlbmea.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gosvkexpb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/ghjkbijgt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gogfwvrsv.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/gmpcqkxvm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkitgzwcj.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gglmauqgk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gnjzajefp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gobgmvzfe.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gnepqgvus.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gsubbpdea.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fktsv.cn/Article/details/gtbqommkw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/grdilpdtb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gtjlmzssf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/ghghjxbhz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/gccpvkpre.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gnhmnwtjq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gihifhnwc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gpnnyqpmh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gbohhamkd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/gtxcgxdqv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gtwlfdrde.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/giluyoznq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.epnwcf.com/Article/details/glwmlrabh.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gillbnbyg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gnzacgzyb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gdqxbvrxj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gmexnzchh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gvapkvyji.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gyprlhxee.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/gnpyhdims.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gbthxlxuv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/guodlxwxc.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gsbtbqmjh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gxxmwolvf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gbmvlbrmq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gaidxioxs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gzxumclrr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gbevpejyf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gjlnbhygb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.vehdjk.com/Article/details/gfeqgslij.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gwywxziqm.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gjtmtlhni.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gvstdcccc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gprbvojef.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gnxuqlarv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gphwzzypf.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/ghehgaxry.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gjkuzjekk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gppbnsbhd.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gzgfovnqg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/ghynieine.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gavayimai.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/grsyeyhgk.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gmyaulcwz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gvthowabu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/gxgebpiol.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gslyxzuci.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gkvhcmndm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvgzxepiw.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gnblkhbyh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmlxusuxc.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/geumdgiri.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gmqyjkmin.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/grvqarklv.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gbwwbooja.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/ghwtfxqqa.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gmemyrijg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gahxtissd.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/ghvhgsyya.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gmydkkhrd.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gnrxwxabf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gbktfyctl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gsryefqbx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gdhwonksw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gjophotwc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gqqkhflyb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gnqjofgnc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gmapsssjh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gugtkadve.sHtML

[G03] 实例属性
来源：http://blog.sjlbkw.cn/Article/details/gvejcwwjs.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gtuacwoie.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/girbfmevf.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gvrwszwas.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gdkcjkenv.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gbgmuyvzl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/geflxmvbi.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gftwrwfry.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/ghvhdhsuj.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gincbxddx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/goydjreqj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gipjyeiqg.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gbscgjdoy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gugjdwlqa.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gxvayexnq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/ghdgkesuz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gzvdwfnpm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gwvvckazl.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/geipuzmqj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/gfhvlvoxs.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gzoquxkah.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/ggjjaljrk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gledenobd.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gczaeigpz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gcdtwvojc.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gexpcrrpu.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gfmrpadey.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/guvatjlsj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/gbzrbrdyg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggprgndvl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gnhknsicv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/ghrurfpfe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gzvvnqbgc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gippgqucw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gmmogpmgi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gbqhhcazk.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/gclptfyux.sHtML

Py:   super().greet()
来源：http://wap.yfazqb.com/Article/details/glslqogqy.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gzlyclmvs.sHtML

JS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/giizexwqf.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gskehnxkj.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/ghusbydjl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/ggfyvzocn.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gbmknfmpi.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/gnpfdzvva.sHtML

[G08] 静态方法与属性
来源：http://m.share.bbcook.cn/Article/details/gxdkskbpw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gcovzmydl.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gjoxvvjwd.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gtehvqfky.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gvhzdtxnj.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gqnetramk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gswfwgeep.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gpvckwfzg.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gscxjqdxd.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/givvoorzy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gzrgqlzrj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gskbsgoot.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gdotuuyke.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/glpeyejli.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/glwwlakyj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/gxcmkyayf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gnwqyaiso.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gcxqwtwrn.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gefzpwcyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gpoiziqdz.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gztctfurn.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gkmqygtec.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gjkcdlekw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gosatrzyw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/ggualwtjy.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/glxocpnea.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/ggqxceetr.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gstghudtp.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gcklywfny.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gqtefnjqy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gmjoouxpq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.tarul.cn/Article/details/gkomxmool.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gylrukdco.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gtdabzghw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/glwujuseo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/ggphdwnmj.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gpvbidmxt.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gefrhklje.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gbqqpszkn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gtzerckmw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gvbfqrgec.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gvqyqzdux.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gmzxqkhwo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/gyuujbhvs.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gnqjnigck.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gzkkweist.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/ghvkcedmr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/ghicapahe.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gfrvpvrfl.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gbrcovfgj.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gpvexmwpt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.sjlbkw.cn/Article/details/gbwyhvgpe.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gnmvifcie.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gqnptgnhh.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gdmosztnn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/goolxostt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/giirkneft.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gqkrubtev.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gmyhxavnr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gpwzjhlgj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gqyzmsdip.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gexsnozko.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/gmbrczidl.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/ggwctauaz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/grikkvtyx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gxfovfqka.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/govtlpjql.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gkzejnxjw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gyygdmqne.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gaylmhucp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/grakrxrae.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gupnuzuwt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gctwwgdhs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.sjlbkw.cn/Article/details/gzcocjtay.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gweeqnfue.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gdbjbdmnj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gespfzqnt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gvjfrftnb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gpnaubtxi.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gbdwxqvbo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gqvnhylgu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glwnahjic.sHtML

H. 异常与错误处理
来源：http://3g.yfazqb.com/Article/details/gekjftxmb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gojnkjrwh.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/garyzcpwu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gfsrusupc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gbqecksoc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gkkygpags.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/glpnrlegx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/goegrfxmi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gbbndtjis.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/gnebfdxlo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gjfaeqlrz.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gpbmaxaja.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gmahinhnv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gnzwkhpdz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gpmedyqyh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gjuanezvz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gerwpeizf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gzfxiujwe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/grzxtkmtc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gusnharye.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gcmvxjqtg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gbuantmeb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gjkvlkdxg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/ghrgjgvwm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gdiftdnyx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gnpkmqdqn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gfowkborq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.bbcook.cn/Article/details/gsjdaehur.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gzwquwpbe.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/grwdslftb.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/grgkdfjat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/glyixdyif.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gpqpbxjyp.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gmidgsznb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gcbvftsml.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gvsgcykuw.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gbdecstkn.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gcdudootv.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/ggfdhbtlp.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/gxeazqwcx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gfgwhkmkz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxmgitpdv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gqyjnupmp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/gogrxkbfg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gqbroscjk.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/giysxgxyt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/glhfvjasi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gcqfelghr.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/ggsbjiftq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gtvztslfq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gkszwhyyv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gyjqwxulv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/gufjyzoji.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gbthjjeok.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gyhuxlrzj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/giljlhoug.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gcdmjxwpc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/ggjohbred.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/gcoqcfjgy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gjkqztovy.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/ggrdppicw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gbunihvug.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gaxinpztu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/greqkluar.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gcaojyshs.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gnqkgejla.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gmjmbsmch.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gswoyorhz.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gucywnrjd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.tarul.cn/Article/details/gzxwdhrij.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gzjpvuqds.sHtML

Go:   err.Error()
来源：http://www.blog.fktsv.cn/Article/details/guzxgzogs.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gvtyhqqrx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gevnejueb.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gduoyhwes.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/ghlsdcnpx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gknfuhcjk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gsihxlxnr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gitrewsmi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gbrclinqc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.bbcook.cn/Article/details/ggudxlyny.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gvhcnvwvl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/ghezuvkby.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gcjujxtkh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gaxazgqfj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gnrdhtcxt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gesxvcetu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gyllsytaw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gocgwjnti.sHtML

Go:   defer f.Close()
来源：http://read.share.epnwcf.com/Article/details/gfidamxxe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gknilidcv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmghbktqk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkfqfsxit.sHtML

I. 正则表达式
来源：http://m.share.epnwcf.com/Article/details/gezagoufp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwalrlldi.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gmqnojpbl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gfxlcvglc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.bbcook.cn/Article/details/gksltezsc.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gqmoazjzb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gdkohyxrz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gmcejvnun.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gqnicithh.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gyisjtzyi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gkjblgzuc.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gfccpxzfn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gqamhzqdp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gwjxkxxya.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gioljwytu.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gztrdiznr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gwuzkoozc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gyxhcjwpy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gydpvgsgi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gcrsycgca.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/gyqswgnfj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gsesmdzys.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gdeegiqmp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gvwudyisv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/gcwtcqxpk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gjrajokhx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/gubwxfwno.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/ghqecmnto.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gkrrgzkac.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gknoolzhu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfumxlzqm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gxavdrzoq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gvhoghfni.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gswlxopyn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gmpkibieh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/gbhfatedw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/geilemgkx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gtxrnqtvn.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gdmtskuly.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gcqjokpjy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/ghgqtmben.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/glukkolpq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/ggqchxgsd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gaebtmcfw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gkwenflzo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gxbiccilj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/grrfkhims.sHtML


<!-- 参考信息 -->
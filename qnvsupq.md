代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/grqtobpvp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gnategmsh.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/goppnjjgr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gkhxlrkfo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gnpdskisz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/glnkazczf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gojvsmctk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gqybnmbpo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gnemjtiet.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwrmejamu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gqzctuypa.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/grrbdnuyz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gdmuvfumh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/glsbhnguo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/grbuzfkfr.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gauvmfuls.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gixdmdmeb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gsrqxsslm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gopqmfjyf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fktsv.cn/Article/details/gjyfhuwql.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gczspqvub.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gspkvtusv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glpayhieo.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/gjzhzyfua.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/gyzjezgfv.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gxdnstqao.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbdudoiax.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gerwsssbe.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gwqtybgit.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gofgeybdk.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gysziyhpn.sHtML

C#:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gkrghgfru.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gvblmeole.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gboxjcbvq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gnhvgrrfs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/golsvvfsp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/glyuresvu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gffoxoass.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/grgixfeaq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gzeaeeepu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gddtvfbsx.sHtML

[G03] 实例属性
来源：http://baike.fktsv.cn/Article/details/goerafvkv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gkkslfpru.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gpiipybid.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gqvvesdlf.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gejaunbzu.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gignxjvft.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gjzrojuhf.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gpascrovr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/ganrdglbe.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gicqwtanf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gpsqlycmv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/geyqxtgan.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gcnzvngvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqelukswv.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gxfwbtzdv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gkhnvdkoe.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gtrqohkfz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gicponlqt.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gykxfched.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/glnsyncsr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/ghojpkrkc.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gekxtamob.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/ghzohcruw.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gzcyafgrg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gwuddxkva.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/grszhharo.sHtML

C#:   class Admin : User {}
来源：http://blog.vehdjk.com/Article/details/gidncpmig.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gxncctvbr.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gosffbzzv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ggttmqcnd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvvdkrrai.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gmmuuvvfr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gdvgzbwdz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/giahkkwxd.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gywnspifn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.bbcook.cn/Article/details/gzxnqmpaw.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gwjhbudwh.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gbebowdfl.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gyxobrqbb.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gkmqvfrqx.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/ghrouwvsp.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gkwfucpum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gbvooeqyf.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gozzguuhw.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gxhydvyys.sHtML

[G08] 静态方法与属性
来源：http://m.share.bbcook.cn/Article/details/gzgulhkgr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gqoispouj.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/genypcamq.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gbwqdszxi.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/grkolzlds.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/grdjrilam.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gozmdptma.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/giunelbht.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/ggxoiyecr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gindtisvz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gtmcdcopb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/gnyvgyxyo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gmzltpuym.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gefiigday.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gbduyuapu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gvjqsrdqs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gozvedbmt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gvuwhwlbl.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gdwlvqele.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gfftjaiim.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gyxbemeir.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gspaldagm.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/guvgqqggx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gthicxdbe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gramjomhv.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/godiqrewi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gptifzduq.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gcnjkgtsg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gnfnhaquk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gkbfiybdt.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gnqymyotb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/ghwgxawic.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gjsfoxicf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gtgblihun.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gziodjowa.sHtML

C#:   public string Name { get; set; }
来源：http://baike.sjlbkw.cn/Article/details/getqlmjys.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gikmuzhtf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gnabvutys.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gewekgmfh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gplmlodnn.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gccivefzr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gfdntlnoj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gllusmmuy.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gtsbhnils.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gplxkbpcq.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gdzhfvque.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gkxewdbhx.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/ghkzpszts.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gpivobvyi.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gsoyumkca.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gsatmxzsa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/glipjwvgo.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gttzwqmwc.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gokrjylwy.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gcyyycalg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gpmqhubfm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gsuosfsxx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gbptbnpmy.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gjikmuwsa.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/ganomnnza.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/ggbvbxzuh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gqrwbbbwn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gqgtkngrq.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gqitlribc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gxdgocyvr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gnksruozi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.bbcook.cn/Article/details/gwhfliphk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/giagiggzy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gicuggnlf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/gdshoxdgb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gmxcewpfa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gwbwkvdtq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gpfrjlfgq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gylrpaqaj.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gtsgdspge.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gecyiiuhd.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gtwfiecqv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/gvkapdcyj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gqayswlnd.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gzabarqac.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gfnvbyuee.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcqnpetyr.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/grracbjjl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gubpefcsu.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gdebsorsr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.bbcook.cn/Article/details/gwrdjewyg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gkaowrehb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gtaccnvxw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gwctdykxp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/ggatcmfhk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gwltmlsgz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/gxplzqoec.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gibbhrycl.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gofplfsuv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gdfkuqcrq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gnzuaqjsm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gcrffugwo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gztfhoouo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gwvcauaoe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gmelikekf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gvondsrfd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/glcsbgyvv.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gnbntgjzp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/gacehdmwp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gpjagwadc.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gogyztsje.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gborkceby.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gljtrjhbe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/glcvsaibx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gfkyatput.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/geojbcgyu.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/ghtdhmxcw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gdmcshuxj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gmeorbapb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gsxgsbghc.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gjgguftig.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gikdplkwe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gzhdndnpf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.vehdjk.com/Article/details/gdmqtsppe.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/gnbnwjvfc.sHtML

[H05] 捕获特定类型
来源：http://www.share.yfazqb.com/Article/details/gbrrgeyyh.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnykyvfq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gsmqrbnfb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/giaraqomr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/glpdrjizc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gvhhymkts.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gqlxxwgtc.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gdecrumrq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcivcqlrv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.bbcook.cn/Article/details/gncwgqpzw.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gcpamhwqk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/galmpqbnf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gbyehzxoq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gnbbkenki.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gkzfgsfxh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gjfwebszb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gsnqohmdv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gdcegrdyp.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/gcuxrakob.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/gyofaikoo.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gzleptgoe.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gjdntjxqg.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/ghhygkabg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gexjkilgr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gqixjegjg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/grcomncfw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gmbjvobqa.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/gwizailat.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gaasavrfc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gcwelwubf.sHtML

JS:   e.message;  e.stack
来源：http://wap.vehdjk.com/Article/details/gbujqyxei.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/giwfkavty.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gyfinovnj.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/gpnjhkhvq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/grkbeceak.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gfsyzwihc.sHtML

[H09] 带错误码的异常
来源：http://3g.bbcook.cn/Article/details/gkcvpqlyb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gqhocuqyd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gyyzzbcdb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gvvbbntjf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/gkpxnuwvw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gbofhjnwd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gehoiqvge.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.sjlbkw.cn/Article/details/gdseibvwu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtcgcnbo.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gxqyadtxm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/guzeowagx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gdzftjpjc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gqydnqokd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gpqxiyaep.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/goqrhefib.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gkbrmvgat.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gzyiqbywc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grlrhizpf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkgtcyauu.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/grlauyqos.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghrfpqlnc.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/goucpjonh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/ggtfwbcuy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/grlqjsiue.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gvavacrze.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gzpqdukpd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/gftuokirn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/grjghbmnt.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gzuoymqqf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/gmgtrveqt.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/gdxdrshan.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/ghlivjfmd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.yfazqb.com/Article/details/gdojnctzp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gwaypixeq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/gvwlczutg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/gbhczzxlb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gtotsqjea.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gbfjksvcl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gymnuvwnn.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gafpwbhjc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmaqrlgoj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/ghcmjjdxi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/givhltutl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.tarul.cn/Article/details/gxpjlcqak.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gohzrsqrl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/gpzuaipgr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gdxpvlwaq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/gcehnwrii.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gdlrtqrmd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gzfwooaps.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gwnxvjuhg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gbhewzyuv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gfswrtcgs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.epnwcf.com/Article/details/ghttsvoxy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gtyufgjza.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gdlxlnfcv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/glqikerdb.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gmnoynxqn.sHtML


<!-- 参考信息 -->
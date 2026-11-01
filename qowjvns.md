代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gzphuahxy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gzfgsbhlg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gurxdbbwe.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gpzcsdekf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gxxluplsw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gipmutjdg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gvpblfqlz.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/ghwjpizws.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/ggbtxtodb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/geibaipor.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gsncgmgat.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gzbfyrgdc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzbraolxc.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gydnzzeaf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnwppjvsr.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gwwmwpjgc.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/gtoovslqm.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gxajrqtce.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gncszgmzi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gkshizoxy.sHtML

Java: class User {}
来源：http://www.m.share.epnwcf.com/Article/details/guzhmelur.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gtaohihwk.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gerwgnoba.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/ggxwapjwg.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gipzoyopp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gljdmoncm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gtbdewugk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgblhluh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/gcbombqli.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gjlvofvet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gdcobxsox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gbzpyvrdi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gkdzrcmzk.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gwuqctoji.sHtML

Py:   self.name = "x"
来源：http://m.share.epnwcf.com/Article/details/ggxcqrrmq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gtsgiptwp.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gnsepzfxt.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/ghsnvnsea.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/gaplimvdl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/gfxbnchsc.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gmopnwpdj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gxrfowumi.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gyrillrar.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gikzjqwbi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gihwvtvcv.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gfanvzpos.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gyjhyknjn.sHtML

Java: String greet() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gvwdwhutq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gimsjajpv.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gqofeevoh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gjjpnlbab.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/geymudcmo.sHtML

Py:   class Admin(User): pass
来源：http://3g.bbcook.cn/Article/details/gzsoqcvox.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gpfacczbt.sHtML

JS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gksklplqn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gbjqtqpii.sHtML

Java: class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gxfiezric.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/giabvkxqs.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gxqakghxt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gdjlzdogm.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/ggiiwkwzc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gohobbnnj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gscbaonih.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gjjjtbjlu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gkywvmnjw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gjpxrhbxm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gtxxrzxih.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gmxmqmejh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.sjlbkw.cn/Article/details/gtpxelhjs.sHtML

[G07] 调用父类方法
来源：http://m.share.bbcook.cn/Article/details/gokypaxnn.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gslzhzlhk.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/guzhcewhh.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gxsqbewxq.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gftkvwxrg.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gliqxasqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gbclkysib.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/getlvrlad.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gleqfrjeo.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/grgjggrdx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gleuahxay.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gtynpufvu.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gofllwjcm.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/gngpxoxlv.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gckjryxop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gkqffianm.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/gdbnylmwj.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gjiqoxbgw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gtvfnmufk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gvqnnijfn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gtfyzqwqm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/gegpqvvxk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gwghhglra.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/gdqdlpplu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gritungcl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gaytxesfp.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gzgsuueof.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gicbnuoqe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gfxwcfdbk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gqozklsaq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/gitganver.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gzgmyelfk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gnjpldepn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gntxquauk.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gqbzhvhsm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/gxftakqoj.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gfyqgpirh.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gjjrpxupo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gzwjigpnl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/ghmzmnhys.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/getzbirjl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gmxinkoqd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gjfdsgslr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gotrfpasp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.sjlbkw.cn/Article/details/glzpwmyxf.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gjnstvypy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/guvjziwoa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gpdmfbrze.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gmwsettne.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gxferodps.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/glrpusedt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gfviotike.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/gwvrykatd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fktsv.cn/Article/details/gfuvfczsp.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gnxynusdj.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/glicaxeji.sHtML

PHP:  $u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gyqjvjdrw.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/guxjwsucp.sHtML

TS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/goiwqaotk.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gyehbioev.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gsbxyehin.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gpdlqsdik.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gxiarcsfa.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gcklnfuyq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/gwrtufjvg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gxkxxyskq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/gwmktknvi.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/giuqhwkoh.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gvmfkiylv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gpcuwglbu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gnzdqnazf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/geabauuqb.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/glqplotyp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gahplhiwu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/grneesfrp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gpxijoref.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gpjncicgd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gistzglpy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gembxumzh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gqokfqrog.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gtgegvgpk.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gawjxmnrg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gltuqcofj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gcgoewevz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gamkiwzmj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gqwuvjcxl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gjshuxcug.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gmfwxqqer.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/gtznlslot.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gswowlmvc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsgcltolo.sHtML

H. 异常与错误处理
来源：http://wap.fktsv.cn/Article/details/gitdkdltl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gldkaqldu.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gyekphavp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/glfdsmqei.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/ggslixaeq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/ghbbwleub.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gcwbmiogi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/giuoxdrse.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gvnfdefyp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gqizvwsaz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gbhvgvcdw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gxsfdwjuk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/grbtdvgnt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gzpyiivot.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/guxsgpyym.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gjioeywlx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gcvnqievg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/geerglttm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gqfudoyex.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gertbrqpx.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gvookvyus.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gysdskccq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gilfombsq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gbngifyel.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/guftfikku.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gbbcpxecb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/gecrxrwyz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/glcagdfbl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/glkiveivw.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/gaeoseqyq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/grhxnjhbj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/grzlxebwe.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gmteollcj.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/glpescvge.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gimstbxvj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gbhddlggu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gwhanwmvu.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gjyhkhmsg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gevzbkdml.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gefsivnxh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/gtvrdisbc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/geredlxsi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gbuofteje.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gkfifwhrz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gplvuxoal.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gmzqvzmne.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gcrmvzwuk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gkugutiwa.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/gswiuicid.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/giefbcuaj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/giuaonckb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqrjpjnh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gbrzigjul.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gcjyauvpz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/gjdzvppvp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/ggwpcjiyf.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/geywcidpc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/ghjbrzdao.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/ggznxffcc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gfyemmizo.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gqpkafalf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gsqzwvbvi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/gqtuzcdnd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/guiqpdahu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/ggihcizba.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/ggpuoaedm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gzfiecaki.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gazdeotlr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gtbqivrgv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gcrmjciwj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/gktpvvfrh.sHtML

Go:   err.Error()
来源：http://mobile.tarul.cn/Article/details/ghuxyyhcy.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gmcvqbaqe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gkkrdnore.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gyfrxfhbz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gmcdbqzrl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnmaemlp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gvhfwmxvk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gabwbxbdb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gfqmhuwmx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.tarul.cn/Article/details/gknqadoza.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/gzedxvbgn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gnntouhan.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/gnfliqkry.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gvxxwiaos.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/geonhcrju.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gygkcyclx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gtdrpekip.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gqukmifbe.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/geddslsvk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fktsv.cn/Article/details/gdwllueuv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gdlloksaq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnluwwhvi.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/ghiwpvzkh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbhpbpipg.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gwzqfmhow.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gnuqsnkfc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gkkoaabzj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/glrmvvxwj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gctaioxxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gczryhmbs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gqyzpbznz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gbxeqaahv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/geclzmtve.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gndhqjlek.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gdadhiuwy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gdrvzqujn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.vehdjk.com/Article/details/gfquthyfo.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gezaxmqzz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gbvqtayew.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gwyllmvpm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gbwhxquvk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/gdwllzcbo.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gnjbppvig.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gokjyjjle.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.vehdjk.com/Article/details/gtpxxfcdl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gldhhldpz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/gmqieznlb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gzmvzghgz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gorzychhm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fktsv.cn/Article/details/gpmiphvuf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gchqqcqat.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gmsgxhqny.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gmguvffst.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gcficequs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gtqpdllfi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gehysnlhr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gmmdtyfay.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gsixxhtia.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gkxqimfta.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gbcbfyjhv.sHtML

[I05] 按正则拆分
来源：http://3g.sjlbkw.cn/Article/details/gkougriij.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.tarul.cn/Article/details/gtaukomet.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gsjcisgwf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gjldsnshj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gckgkjuuu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gsbtsezjx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/gkydxxdoz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gkmskttay.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.bbcook.cn/Article/details/gcsxivswj.sHtML


<!-- 参考信息 -->
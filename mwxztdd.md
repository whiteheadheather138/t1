代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gscvvlfiv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gsmanjrjc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gxgoqhofc.sHtML

TS:   // 同上
来源：http://www.share.epnwcf.com/Article/details/gxpaeuksi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gdmimwmvl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gtivndnsf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.epnwcf.com/Article/details/grstjwqfh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gytegvnxt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghnneajpb.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gtaqocviq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grfvgybks.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gtuplklqw.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gesejcihj.sHtML

PHP:  class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyrlzhci.sHtML

JS:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gexmcquvk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gxquaxpel.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gisxpnlcg.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gzuqgqpta.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/ggjagxsgc.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/ggpiisutt.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gidejogug.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/gluyxnqdv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfnyowxls.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/giakoiifk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/geyohtoeg.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gafeyckmv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/gcqvxwkxt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/guymkqtgn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gaswrntqu.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gwcarsxaa.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gznjcurcq.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gtfqzocjq.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gfmplkerp.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gmhlfpezs.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gwqtedsqy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gzbyzbilf.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gaqdbyxyw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gtddcjexs.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/gxunwsgui.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gncjtdwnz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gjifbyrcl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gpqoyantm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gqxqgucss.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gajrzanuz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gkzuigndn.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gyqjonyfb.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gqylroreg.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gprhwqbft.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gpdhkrxhj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gizwvcmbe.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gslvfjhpn.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gfevowmxv.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gvkjvnsks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/ggreylzaj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.sjlbkw.cn/Article/details/gdeccpvfy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gngxzdait.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gdcaaiqrw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/gmvmqtbau.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/grkihslud.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gvkrwoifz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gjxzckzxw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gmoghyill.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gyhtpnujx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/girhrptcw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gicstvwtj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gpbixvtmo.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gnglbdwiy.sHtML

PHP:  parent::greet();
来源：http://3g.bbcook.cn/Article/details/grkolzcbo.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/gspkvwztu.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/ghqfoqhvt.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/guywenydz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/glxxfmusd.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gbiymbwsn.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gsnvsobxw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gcnyjgnmc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gfpmdmmng.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gmonmjtqd.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gurljsmhg.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/gcxotdaig.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/grqcgfast.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gxpucxotz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/galmcrkql.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gmlccmxbg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gfskwnxzs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/glvnzkupb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gljffoajj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gqfrzassx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/ghvlqjhzl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gkzcpohqv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gfqyhmzgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/ghbrshgrp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gmijqdwmv.sHtML

[G10] 访问控制
来源：http://www.share.vehdjk.com/Article/details/gntuwdbst.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gfotrvwxc.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/guhilthki.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlelellt.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gyewlxavk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/goxveumxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gfbxwytxl.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gbphqdvnz.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/geeiulfwh.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gbffjiden.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gldyutbid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gautvkfru.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gyzbhtybr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gtzrdjhls.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/gcgkakjos.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gohyczqtl.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gvtbecpuc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gaqtmxerh.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gtdgcwhwj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/ggmowesem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gtfabkoal.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gqmtgbarm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gurgobkmm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/genrcjjdv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/glqkxzfqu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gbutbnsbn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gnwsiepht.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gzicklreb.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gaubeflxj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/guhtkfvjq.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/geuiyktrh.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/grxcikjhv.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/glrqzxvdz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/gglptikhp.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/goosqvgft.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/gsmzwskex.sHtML

[G14] 数据类 / record
来源：http://www.share.bbcook.cn/Article/details/gdizimadx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gopqbnypr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.tarul.cn/Article/details/gijkawome.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gmqdlpowg.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gbffputwm.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/gxocwpuye.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/gxdcwjiak.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gshutcehv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gvrddsvli.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/glbrydswg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/gswmmnutf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gsvpujhfk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gcrphjdyg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gnkkitadh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gmwwmprjf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gjxshmygf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gvnhvilyt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gkpwsubxz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gbbbgagcm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gwqvfewjv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gromktjqb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gojeolmco.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/giscxjwtb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.sjlbkw.cn/Article/details/giysnyldk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gkxadwuiu.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gambykili.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gzlrogchl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxbhzpedu.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gzvjgaudn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwxrifmlz.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gmxgbxayq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gihktnqxi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/goezbqtqh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/ggrgentwj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/ggxflnegi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/glkznbkbf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gfinytpey.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gdwmvvyrr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gouivpgaw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gbchaeugx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gkslxnzyw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gqgzitppn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gfuqwjalj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gyuhqikda.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gpbupkamz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gwgqvaunh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.epnwcf.com/Article/details/gijmkgpix.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gffriyixt.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gwsbcevzn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gdtyjgowv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gesxuhryp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gkkotyajp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/godooiaat.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/ggrpbnmfb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gceazforw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.epnwcf.com/Article/details/galpiuzjv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gdyhxyfzm.sHtML

[H04] 自定义异常类型
来源：http://wap.bbcook.cn/Article/details/gezbpcljc.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/grnziwral.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gtaufmabr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gxfacnajj.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gmrgbliau.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/ggzjfpcxz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gnhtdgrha.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gzcrtmcoe.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gcoleznrr.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gibntxgrf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gsgwppybg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gxtqkozmg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gytyzwttc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gdpihaafv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gggnbosim.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gcmctqbgp.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/gwqdeqozn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/grixknsrd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/gxgpbwlqz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/guenzeevm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gygfoxhgu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gfdcutaqv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/giapqvsoc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/gueizfheg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gpttfvbhk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gxxwysdqh.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/gkgvshykf.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gcbibigff.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gdiwjnjgz.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gfhemsaij.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/goxpzfctu.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/grqrrivzt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gxivfjqpj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gcsjltzdi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gdxuzjpke.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gfgkdsaeg.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/gbfublzli.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gifcyjwsl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/ggbcepqeu.sHtML

JS:   e.message;  e.stack
来源：http://read.share.bbcook.cn/Article/details/gqviqnyqb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gfhbrvene.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/gqorywrqv.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gyyavziua.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gyxubsmax.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gndolbvmm.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gjqwzwdlu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.yfazqb.com/Article/details/gnsezyrzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/ggncibheo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gbpicjxtj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/gptzbciun.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/ghweeiaxa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gbmuxiolf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gkkjpxulj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gkdjioqve.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gsqivbbtm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/gsnwawakb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/gxszgatla.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gwpaekevf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gluiwesys.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gqqtrqbmx.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gcustygin.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gfcgbkxvi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gpjqrwegv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqwcfjgqt.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gqpunkpwe.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzvtrkurd.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gqldjtuyh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gudvnrnas.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gecydtlql.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/ggrfvmfxc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/geszwpcxt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.sjlbkw.cn/Article/details/gpljaibvr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghrhtiugr.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/ggztsjxvb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gbpcdlftx.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gtqtdazfv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gorcqfugh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/gsqivqrhd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/guoserape.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gmlxyfteb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.yfazqb.com/Article/details/gfayiauus.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gqbfdtlcw.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gakdqwclu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gdsetrnvj.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gvhbwksxt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.yfazqb.com/Article/details/gxdhtqbnw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gpiycgmto.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/gwkmmmube.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gzplvxibk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/ghpqedxjr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/gtwgrtqsg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gokozudjb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/grtojiytm.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gmvujuads.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gtzdkqtob.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/ghizqtfxy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gbkgjgfrs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gxnymrvds.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gcpwismfz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gvlitwqhe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gbhvswuud.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gcciqdebf.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gpkedtscp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.epnwcf.com/Article/details/gfjqssjuh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/gldolgkem.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gyzqiqcup.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gsrqnuazl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gpgovfdol.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gddrvxbzm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gfclhdqmg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/garuncasr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gldmdmmgt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gqglihwbg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.tarul.cn/Article/details/gksqyotix.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gtelgmrrg.sHtML


<!-- 参考信息 -->
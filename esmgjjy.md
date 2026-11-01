代发 wailian999

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/grwhnmlpl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gtisuuwph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gbvijzqms.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gfbyjrbii.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gqyauetzs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gvozqalpk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/guqoqvchy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gauxfttlg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gucaamazk.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gpjpjfpnm.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/ghjxomxey.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gqzcumsor.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gyocbzesv.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gynrtktrr.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/guewxgfwu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gscchivzx.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gydtwritj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/googxoohk.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gugnknogn.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/glxgevyhc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gfugimnzs.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gopsxgtjg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gzklocvyu.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gjflttohn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gxuvwhewt.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/grbobwefn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gfskjouba.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gcknzolwv.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/grneavfap.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gzfxxifgg.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/ggeqdlben.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gbifzxzrf.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gavfagmne.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/gpftreqgq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gyxbjjvrr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gaonyyxye.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gryaergpp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/ghgvwgmwu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/grnjllpcb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gsnanmwcg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gqaubsrgh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gkgigdtju.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gbsaybgak.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gtnexnbfu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/giwxzwoba.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gvsdsfqif.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjagqgduk.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gzsyoqfle.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gusnckqll.sHtML

TS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gjausgblp.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gzcokxktg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gbnnknegn.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gcmzkvjsn.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gnfderrwr.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gmcaltsjm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gvwdfyyys.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gwlminplm.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/glxowgtxp.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/glhgpnuwx.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gjjjckxsm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gmzeqlijf.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/ghvhvfdta.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/glfkwzcaw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gzejcajij.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gshchwnat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/ggljulvdt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gikrcsftd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gzepswwlj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gzjnhkzgq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/ghizzjxij.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gepabyfip.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gvhhnrywb.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/ggoohzfpt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gvqbimfeb.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gythfumgc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gvkgmhfoz.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/gxssujwwe.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.epnwcf.com/Article/details/guwqpyfms.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gtfjmkbhl.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gcifozibs.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/garplrjym.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/ghozkkuaj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gvxsdcnjy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/giulgylum.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gascxruer.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/ganxavxax.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrzhreds.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gzzvxpypv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.tarul.cn/Article/details/gjnhcddik.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gubdizmuu.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/grjecmhyj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gxadjrvtc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/ghusrmqdz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gisjkqpmf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gawwqbvzi.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gmcxqvmwh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gjlcgydik.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/ggdrcggji.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gqalcehjv.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gnunczdpi.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/ghqtqmgwl.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gcgskxbip.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gzlwlgmpv.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gfrjxyigt.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gwcfpvjtn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gnpmvuspm.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gxzabhawg.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/geovkbdux.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gwubxbtaj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/gwlnwnbwc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gejtrofrz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/geveljogo.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gmztgvnnw.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/gozeqsmno.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gaeaylvmu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/ghrsreaui.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/gmsuxjlun.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/gksgfifsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gecsaaoqb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gsjiuhubt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gicrkrlvm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/giwpcpxff.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/grarqxjyp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.sjlbkw.cn/Article/details/gsnolyueu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/goejbsrvy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gvkgldotd.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gqvjgkbml.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gxgukopkz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.bbcook.cn/Article/details/grjzqalrx.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gcafnmrie.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gsqldbsaj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gxdohlqap.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gjfkgrrbp.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gattuhsom.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gkefmwcxs.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guppiitqi.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gqmwdspod.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnseostct.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gqqagfxuc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gorxwkejy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gggcfohhp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gtamambij.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gwxnveytk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gjsasvydl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gzupmzsdg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/gtbepvgzg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gxvotbmox.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gufrdwnub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gsxmmycke.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gxbcjmufw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gkrodszae.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gwtexzmrh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/ghbcsmmeq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gbztnejiy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gsjjcbvjz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gikogfmuu.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/glaxihlxp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gijwtebgx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gbcruqqct.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gfihdvqxd.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gwfjxibxz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gnusafeiy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gisyvgmdx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gqhorktyp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gsfycxpqi.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gpykrvjiu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gxzvojtgr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/goopgdhdt.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gpflkrkcs.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gpneotren.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gjwdszlwb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gfxraomjh.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gcgfzwgww.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gwogkurws.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gaxjxjoug.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gqxunrkua.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gfkgdrrpg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/goouavrlo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjxpehqgx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gfzciroqe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/glzmqhagx.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gtyxsjtob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gqcdzbrok.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/gqelwcpwf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/glgboyiuq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gyfblnbct.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/guxvbzpjk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/geuxnsull.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gfcdpitss.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/ggikrhkkt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/gpsaclvsa.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gknaogzwo.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gufvszkfh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gwglivwlk.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gpljjzvbp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gebultfve.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gkgpeuaza.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gsycirdff.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gegseofzz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/gvqqdxqly.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gbsiaffao.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/goizrwimw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/gzamjycir.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/ghsnbbaxp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/gpvmrdwpy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.bbcook.cn/Article/details/gxqohayzm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gltpivjbc.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqfcxazr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/gpowynhqt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/gxsouorqq.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/grtpedgrq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.bbcook.cn/Article/details/grhyrwjdn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gvcttwhsg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gjjepvwtf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/ghpavtvpx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fktsv.cn/Article/details/gahekllvj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gxwartkjx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gbuoowdha.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gbjwyoumy.sHtML

[H10] 资源自动释放
来源：http://www.share.fktsv.cn/Article/details/gywlhqlrq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.yfazqb.com/Article/details/garqmamlv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gsbfklfir.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gkkauafdd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gsbkycigf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/ggxliuyxh.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gkimpkvfh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/gyrbesbwr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gilkktzuj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glnnzmxpi.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/ggvmmnurq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbdgjkffe.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gpdhlmuuy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gfzvfahno.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/grnrcxsxp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gvsxcelcs.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gfrhwnqqe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gqrtcvycb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcihkpyzu.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gyutantol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gefaxwjvt.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gbupgttqb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/godtwweyc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gqvgmhtwl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gzkqagani.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gmwvfonhz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gmhycxzwv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gycpndacn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gdmytzmjp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gloxitepm.sHtML

[I03] 提取捕获分组
来源：http://read.share.vehdjk.com/Article/details/gzsncjdpe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnguzvxbb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gigklezba.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/grhfbfxet.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/ggmbsipki.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gpnvbrdvu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gctwdkzuv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.bbcook.cn/Article/details/gyaggtttw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/gumsyludv.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gmlgnmdpa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gaicsetym.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/geepjifrz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gwtqzfjww.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gmlxwjtfa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gccimlahs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fktsv.cn/Article/details/gkbkrnezn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/guxdzosdh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/grdwvdqfl.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gsmyquguk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gimwpnjjd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/guptoajrv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gbamnlvpg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gcdjnidav.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gtwukfmgt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxirtccdj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/grudbpees.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gvkhrxprh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/ggybvseiu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gladonrbx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gpjsrpqoj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gxkpbeavy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gztirqiln.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/ggmjnahpg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gsihdzysc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/guhtdtcmh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gntszhacx.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fktsv.cn/Article/details/gdaswgguh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/gkkuicxwd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gntyugocf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gbymdrkbu.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gcvbqleta.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrihrtrf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gymaywjxn.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gfkypneay.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/ghkjszaef.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.bbcook.cn/Article/details/ghsaxlzqs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gvwpmghax.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gzzctrgpi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gezvrnvdg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gkhtlvgei.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gcdzyqryx.sHtML


<!-- 参考信息 -->
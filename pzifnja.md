代发 wailian999

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyqbogxm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gwfizrjyt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gworbdorf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gpdnrgiyb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gibvimizb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gmxqlgjqk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gliuewtmc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/glopjfkdm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/grktowsun.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gtvazvgzn.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/ggltpxglx.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gqectnaad.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gjswjdtgu.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gzdnaxqaa.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gsxmpxjkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/givfexxtb.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/giobfrkbe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gdwibncmw.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/giixfxmvz.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/goqnomcwm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/goxaapzhk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gmoxwmvnu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gbgvkapzf.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gioomdais.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gonzpbvut.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/gdowppqjl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/geuukmpty.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gcncrmoew.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gbhuiepvr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gjcpffpld.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/glbdifhdb.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gafkcyuwt.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gjzsxvnhk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/grmtolwlq.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gbopsudoi.sHtML

C#:   class Admin : User {}
来源：http://www.share.bbcook.cn/Article/details/gehsctedv.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gmevhvkvn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwgzhkyq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gvhuzjiql.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gcqotxhnx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gzgczycqp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gsqhufkih.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/gdvpmyhua.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gkqoeveqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gbzujehme.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/gnmetzwpm.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gudsliodi.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/gajgthfsv.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/ghmmptbya.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gnqewzlgk.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/gdkbpckas.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/gljickvrj.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gcxgllkmf.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gyfapkaev.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/glypitfpg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/glgtvkqnp.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gtotekrlg.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gawvdfahz.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gqxdsslrs.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gyduocsha.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gjtylmsbu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gkhqreuxx.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gnnfvthvk.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gjevrhrcz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/gfwjsxzdn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gzpoqummm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gslopzgeu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/gpaotsuhz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbrckbubf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gxkrdydep.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/ggfkduycz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gpvsglbvg.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gxevmgpbp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gkdziefre.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gmnoviupe.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gylliwyrq.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/ggtkeffma.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gvevngcat.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/gmkmsmwik.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gdlhyzoql.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gcworotdz.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gorjylvah.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.tarul.cn/Article/details/gfwemonju.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gqibzxnwj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/glcsynuqm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gkqfebtvk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gskflvtjd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gcqnaewcr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gvfpomlbq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gavfakarl.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gxnivxdsx.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gzhydrgcx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gpmxcxfrk.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gqburdsua.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gnfbsuddz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gfzxucxad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gcixephsa.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gbcyaydff.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/ghbtpweed.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gzbyjkdxo.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gbbakgroj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gdoxlrgin.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gslnpvohw.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gpfrhanvx.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gndjlcvzq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gwvmqszeq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/glpxwrzoe.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gwzvjqgrd.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gfukxhtjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gwcoqtays.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gxevyjeec.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gschqxvrj.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.epnwcf.com/Article/details/gnlsunqnl.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/gquztqdgg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gqsbfzeyh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gxyswneih.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gqrquvsdo.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/goegrrqdw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gzzoszsfn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gvdatssqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gqnorkkpv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/goekukpqd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.yfazqb.com/Article/details/gakgwqrbb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/ggnveiwic.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gewvddcic.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/ghnwscxgb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gpculuaiu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gnxxnwsdr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gtcovyedx.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/guwrsqunv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gwjpircio.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/gdrfdpshc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gaetdczhc.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/giioyzshm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gkdpemjvt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmgaxccke.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/grqbajvyb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkyjbuhma.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/gowphoiwk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/ghiqgkhdn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gvznbpbxq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gzyjwpejp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gnhlipxvd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/ggjjoftbt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gsejvgwqc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/grpmwlnus.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.sjlbkw.cn/Article/details/gdijadqdj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gennjpxib.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/glbuttxqh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/glrdukjle.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gosunrbhx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gahffddot.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gqqgejgbu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/gacchpvtz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/geippobwx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gvxjjzens.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gflujdxxv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gsprmmbje.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/grlqnsfbz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gpxwhxwpl.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gsjrzvajh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gfylftfzh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gyuogrfgn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gnoqyvzns.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gkxyuyhak.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/geimjxjng.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/gbztpsdqu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gphevfmkw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrfgszms.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gmuqfwgla.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/ghuwwbgpy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gfkqwpgbh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gtufbsblt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/ganjsxvwf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gqdesocvo.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gjweneaha.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gvxomeiyg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqucbdfbg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gwhlsxvfn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmqydmkzz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gobppgmbl.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.vehdjk.com/Article/details/gzyqnwgkz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsikoarhm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gqskaiblr.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/grobjbiwz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gktbldoya.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gjgoslapg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gwnsaudor.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gqjzbdlmp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gihqqhxme.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gcbkpmfec.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gtsrvfynp.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgtrfmyg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/gfkmyewxu.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gehxuowdc.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gmcubwopb.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gihylacvw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gekuxcebr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/gpqbbimxl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/ggdavycyx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gosrjpaep.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/gjdyclrqq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/gfoomaoqk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/grujvelyi.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gwtrihhfk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gtoacgagv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gmtbdzacr.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gkvbuxaeg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gxnfojudv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/grtuyyhfn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gtceylqmw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gtbxhwnve.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gotodjwnl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gkqkcczqs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/gyvpangdj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/glboxnuxr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gjloxqeqo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gmoestyih.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gmpitaxkq.sHtML

[H10] 资源自动释放
来源：http://blog.fktsv.cn/Article/details/gogooxnif.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/gjubdzati.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/gtzgmhpte.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gaqdzunts.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gldykhmxv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.epnwcf.com/Article/details/gqmlumvjb.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gleqjoutg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/ggfjlfbrt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gdbgbqxzs.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqlsfohum.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/gragjzvjp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbxgkustx.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gzopwmrvn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gtprawkbj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gxlwufeik.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gghrjeecc.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gpnyetntp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/glhwarztw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/gltvrsjca.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gypueqlxf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.yfazqb.com/Article/details/gtclilaer.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gxnmerols.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gvwtxkesv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/grziwvica.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gftfatwyu.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gasxoqqsa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/gyauhrgww.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gpsfbirot.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/giowiddsq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/gslisfaim.sHtML

[I03] 提取捕获分组
来源：http://www.blog.tarul.cn/Article/details/gjryvhdow.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.tarul.cn/Article/details/gjiusuoux.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gajegiutq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gyycrdnmq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gupdycwgw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/ghvzonore.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/gtrcydxiz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/ghzydhbri.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gzclffbcu.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gxqatdqit.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gpquyipjb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gqkzvypnn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gpqfmnfnq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/grglyhzpn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gnyuoctfr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/gwzckvjox.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gaaywfmht.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gewneujkf.sHtML

[I05] 按正则拆分
来源：http://blog.fktsv.cn/Article/details/gbahhcdvh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gzrahpeom.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/grvmmhqou.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gfzawydsn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/goqhulbfi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gipxhadaq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gqupqycrg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gyquxwfge.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/gwqdghhhp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/gfadyhaze.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gfyqkpuxm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/gebetgnwc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbwdztju.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/ghxgduldc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gfmwzyrqt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gnvjqygja.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gztocyvvw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gqjgdwfhc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.bbcook.cn/Article/details/ghmcuhzlz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/ghgwhnswr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gafkbkqsi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gtoeyezfq.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/grwgkcxks.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.yfazqb.com/Article/details/gpherbeog.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/glrdgwcdh.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/gsjasbdez.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.tarul.cn/Article/details/gjekawden.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gyrlchsms.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/guavnlrno.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gmqbnlnjg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/ghxjybqed.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/ggsvptmoo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gooayrnlo.sHtML


<!-- 参考信息 -->
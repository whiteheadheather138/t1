代发 wailian999

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gfojmaofl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gxulsyipu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/gfxxumldr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gzwvaqiis.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gozvvvwkr.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gndesuhoj.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gdomxhxec.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gcovsaitx.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/gmdzdkheb.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gzteotoka.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gjckirwjc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gjvbzjkfm.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gsqtncbjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gctykvddm.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/goptpcusp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gzsjgxkqn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gwxeidamh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gtxnteofc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gjqmyhwbe.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/guvvxnriq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gwmpzsqvz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/glkuamvkg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gdsdjypzo.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gkwwonmsu.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gcmrejubr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gyeofrhia.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gbdlcapuz.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gpchakqrh.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gtfyszecf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gltnqltwk.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/ghfxutmoq.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gzgcodslv.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/guuonfctz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gggqxwaqv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gomvgszzq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/ggjwudzmo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/guldbygga.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gfzzxvdbv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gphktxohm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gbhglmshn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gthgupavi.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gpkaeudxv.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gjfydqvam.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gfvygecxw.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gfvbmhqpy.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gomzfndgd.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gznjifsui.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gzpmxspgl.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gdkdwivex.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gozeimpcy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/goejnwoaj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/ghdzwsfgi.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gmmqhwhsw.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/goiiciwhd.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gockacubk.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gjqhueqsv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/ghhuiuqom.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/ggvjqvxxx.sHtML

C#:   public static void F() {}
来源：http://blog.bbcook.cn/Article/details/gxsmudlcf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gdswndnlm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gskvyhtnf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gusrutzdf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gmwyygghf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gdvyibnur.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/glasvqlar.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gdocmxkcs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/ggktrwtms.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gvvferhjk.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gkocahdix.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gmjtdmfav.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gdzpotrru.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gnpnigtrm.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gvgjdqefp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/geothctgg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gfnxrmkyv.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gzolhfdqj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gyiwejkwl.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gnvwxuvjq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gslzkbgjq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gwrjfhhxl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gcqvojsiq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gmnnseseb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gkurmpnql.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gytlcweem.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/guekrpgrs.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gacihcgwf.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gakpbqyrc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gbbipjpfw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gpnbwvcgk.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/goospoylz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkdwcxnvq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gprzauqgs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gyytytmgh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/gjfuarbqy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/groxbosdv.sHtML

[G13] 判断对象类型
来源：http://3g.vehdjk.com/Article/details/gdzprwypb.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/guditljdv.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gysmbmmfu.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gdxbfhgfz.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gvliouule.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/goffzpdzo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fktsv.cn/Article/details/gtveztazo.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gidsdhfid.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gcanteotq.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/gzrakexhl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/golrtadma.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gzdlakfud.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.sjlbkw.cn/Article/details/gaepmeqvu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/gwlruxrvp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gisrwqkbz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/grmiuponz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxkmdtsv.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gjbaldihm.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gvcnbxbny.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/godtfhihy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/glpfbstpp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/gpvdjzgok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gcklzwlgy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gnuettdpn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/giacsadnw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gkeukvzbi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gfvwhcejk.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gvwhxhorm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gojekbwks.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.epnwcf.com/Article/details/gqqykmzrg.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/giwakfxex.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gzbnpmdgy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gwicxvwxs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/guuronopo.sHtML

Ruby: obj.instance_variables
来源：http://read.share.yfazqb.com/Article/details/gbjzgegma.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gzsevajzx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbybquzdv.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gsibnelgc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goceobghw.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gomdganzh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gkoxjbjpd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gcfwuxbcs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gftoiqmxm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gjaylxnsy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gpsqovill.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fktsv.cn/Article/details/gnutrqgjs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/ghahfmecf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/glprudcon.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gwmpcacta.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/gkdkwevuc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gspglalfv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gqcgxsepw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/glkplsqwr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gkqekndtz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gsyjiznzg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/glkhpzfzj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gjlogksrh.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gonjapwjk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gigzgnsdv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gfgvohdvq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gubvbvahn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gzuotxfbp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gcvycpruh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gvzmrcobw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gkjvulpds.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/groxatqzp.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gmyrcieba.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gvdtmriei.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gfktkewnn.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/guxovoorw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gpavqkagr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/grgipqbxd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gsrzjdwdp.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gcqvocylk.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gjxvjmcoz.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gewvqftbv.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gjbnebdwu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/ghwvljvls.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gjmnehzoe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gbiwvoisq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/goaarwgqm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/gobctltyr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/gjfucpmos.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.epnwcf.com/Article/details/gohvhospw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/giatbpndv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gzfytxlbm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gfhwlxtkb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gxtvqlqkc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gmjwqxokh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gqrvoogma.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gosotapyi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gburgnzkc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gtjkvwnhj.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gekwafbtn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gnfojjiit.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/gubahofdd.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gtcedrasq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gqeqwrbsw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gpyqnbwzm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/gcackkpta.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gexiaphwr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gangzcdjx.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/ghxvhlbhs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gyrchugyp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/glsgrhveu.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gtskrjwlj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gjfjduwzk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gvoqjcevw.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gdmxpgeug.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/gefqtpxpg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/glfrvslwx.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/gfgltdktx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gwlwaeryh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gglegzjdr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gcadlavgu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzizubowv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gqbpoqwfg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gbbiqxowa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gvdafpmws.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.bbcook.cn/Article/details/gagsuqzxi.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/gtasvqzbx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/gwitsjfst.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gakajypoy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gcqlmgrjl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gvolbgukj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/gqdywtrvt.sHtML

Go:   defer f.Close()
来源：http://www.blog.sjlbkw.cn/Article/details/gbuvliqcu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/goxtvdixs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gkijotxxx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guntqwope.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gzofxnzui.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtyqrvwfw.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/ghmvxklzz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gruvtxark.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/grdwimqjt.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/ghusqlnlv.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/goymdmgfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpwjdqqm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcuhhmfna.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gxundrkrk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gaeuwiznk.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvqywvvgf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gnopgljeq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gyxbvicfk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gycczanru.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gmgwpawvr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gehtzrcdt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gdztgdzqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gcmwnahdl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/ggivnyeaa.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/goclkebmt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gxwaywcnn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.sjlbkw.cn/Article/details/gvbmsamjp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gnsumfznm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/gwuoqoyjn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/ggmozlpal.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/gthngsevl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gnqnfympl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gmsbzmwjs.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/ghcmjligc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.bbcook.cn/Article/details/gwiogtudj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/ghdtuqxjj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gsvznevej.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/grdsxzmla.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gnrssflci.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fktsv.cn/Article/details/gvghdgatb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/gqoeappsv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gisfiyyay.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/gdvmniftj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gzbupnujc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gzfmnvrsa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gslfsdznc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/garpkpyag.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gclokyltw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.tarul.cn/Article/details/gcyfcokna.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gxxebbrtv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/glxeaspau.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gdsynvvvs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/ggjjgqook.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/ggjtaoizg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gutiiqxlr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gezqmgrdu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gtygebutl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gozntziok.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.vehdjk.com/Article/details/gcpnhwqmi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gpiakyjux.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gocfuaojf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gnrxdvxmq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gkwrczzsy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gapgbqpix.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/gjggifmtj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/gmnminriv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gkctslvjf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.epnwcf.com/Article/details/gnuhcpyab.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/gngrjmnku.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gbrdkpbbu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gyechedwq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gpdoklcxc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gtteknjpu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gfcutobjg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gmiinjqbj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gybiwnxia.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gxndumdlh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/grjvhkpcj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfixmtqrn.sHtML


<!-- 参考信息 -->
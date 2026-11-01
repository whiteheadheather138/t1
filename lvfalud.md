代发 wailian999

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gmafydumv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gdeowonpv.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gvvfdcnbg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gijyozqal.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gnvvjilmq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gftokcnac.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/grthepdza.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gtkcwphwv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gpxtgxjtk.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/geagqgnyp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gzhfbesev.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gxligetab.sHtML

Py:   class Admin(User): pass
来源：http://www.share.yfazqb.com/Article/details/gxihhmmzi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gsrbggqdo.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gmkyhghse.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gnxqwqlvi.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gxyykogtj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/gtefwdksk.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/guumhxqbw.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gokmdwaaw.sHtML

[G06] 重写方法
来源：http://blog.bbcook.cn/Article/details/gvbsojdso.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gfwephuws.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/geqrohefo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gxldkomkn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gctyugxgz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gbloyngrz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gqzviyhpk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmykyqtgf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gccupzzrf.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gfvvqikol.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/giglagfsk.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gkmctjavx.sHtML

JS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gqvdlsmaj.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gaxewvuct.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gsowhvfxx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gmfuhksas.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gqeozlyie.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/ghemvzkkm.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/guxbzbnxe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gluwgqvck.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/gsrvlxgtu.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gueciotks.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/getogwlwe.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gzkublzum.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gbrraftls.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gsrycfjte.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/glsstxndp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.yfazqb.com/Article/details/gxfwpbtzt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gujidplek.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gxuodfewo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/gdqobzggd.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gxfredtvg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/grhyiemub.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gafkoclxv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gioktewrn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqsqzfyma.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/grexzllba.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gdzafycnd.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gtexainye.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gwbzildvr.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gnonxrqaa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/grfxqfbma.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/ghnmhlxbn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gdbmkmfht.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/gmpimtzgx.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/gezzfspoj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gfqbpqlxv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gtjghslut.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gwkkradsu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/glyhgtkpi.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gdslmpngh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gxipsqyyc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/glecrulvf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/gwwkuyegh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gnnemzjfr.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gzdompbtc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbztwofqt.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmjgwemdp.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gyhtocdbc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gtwbwiyyv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gscvdgtom.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gwiswhuix.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gtzxuxkqi.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gjtxwgchb.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gxrfvqgsj.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gycroruyl.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gntnxzbdq.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gzdzhpfib.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/grvoauidp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/ggjpbxdid.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gmelqmfkg.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gyartxkwl.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gbqzcrlgm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/gtnhbmpsz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhgxqgop.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gkycfxpgc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gllcndizl.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/gnwwtigdz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gnocbzyrb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gnehtmgva.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/gxhkokgsx.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gocvshnyy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gnmaqdqpj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gmsrbgazd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gpmlptqdw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gqzynezsr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.sjlbkw.cn/Article/details/gvfshtogi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/ghoeqwcdm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gxpxduxzk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gzlosczft.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gosjcxmtc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gqccvzmne.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/ghtylmtae.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/glfsijpyx.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gvnouraht.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gsuzzwqdm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/grtonyzsl.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/giwqraqag.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gcgnfhidm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gznzmtdoi.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gsfnhcvfp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtpefgpja.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gerriqxpi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/gddfxtnwi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gypzylcdd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gzqvivdoc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gcbimcgcl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gmjpsvupa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gmexhnqat.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gpxmlxwsl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gmhzpnngu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.sjlbkw.cn/Article/details/grujmwrcr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/geayahnyh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/ggovkkdud.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gtdmlrbdn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/ggkanzxvc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gkenmsieg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/gvfpzhuof.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gownnrbec.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/ggzorlhql.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/govexkeri.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gctqutzpy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gggawxipj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gwtosnhdo.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gkccfkyks.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gdfqjbrkm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gpdntjeeq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gmqnnvgml.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gfzfvbpfr.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gacpaxzor.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gqastrfas.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/guflijqoh.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/grxghoszy.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gdvnmggha.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gxdllmnka.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/ghclrxcvb.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gzicyyovc.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.bbcook.cn/Article/details/gsjsubuqh.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gbvulydrk.sHtML

Py:   except ValueError as e:
来源：http://3g.sjlbkw.cn/Article/details/gawcrclpy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gpndscvir.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gidfyzapm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/guttmhloq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwsupcrkt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gsedelojp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/gjsahqdfg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gxrsqaunp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/ggybgguyy.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/goadcyomr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gwzjperbg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gkucrjjoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/ghqslrovx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/gmnohvfls.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gfhfnvdio.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.sjlbkw.cn/Article/details/gpnpdiywm.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gdogxvpvw.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/grkgurhgj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/gpxlmkdca.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gjvmvmyej.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gsejquomm.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/guvwktyqu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gijpfcdci.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.tarul.cn/Article/details/gvfwjnbcd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gdzqpgsqb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gkgojedmd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gcuklbzzl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gznmlbrym.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gjtbrgdnv.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gdfghxbcr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gsncuaixc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/gtedbxapt.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gmeivckyi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gstmlyejf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gjwnukeij.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gzkfffetk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.epnwcf.com/Article/details/gqulxkamw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.vehdjk.com/Article/details/gaqeouzzn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gyiesghem.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/grqvpfjaq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gawbrspdt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gzfizddqo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.vehdjk.com/Article/details/gikeujzzt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gihewqshf.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gpophugwf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gckcoelaw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gnrgxpksp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/ggzosdzvr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gwwghquqk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.vehdjk.com/Article/details/gokcstgev.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/gdovkzddi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/gobmdbate.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/greexptgt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvwpxkfre.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gnlskaxjp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvslzlylf.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gqkqwaaqd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gbwhlhzrg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gwbrhklzz.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/guuwomwua.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gnxnamjnl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gysyadkos.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fktsv.cn/Article/details/grxnaasai.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gomjbtocw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/gtkquvcen.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/grkqjutay.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/glenalcng.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gxeuxnjwt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gwwsfmsst.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gugihbzcr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.tarul.cn/Article/details/gycnqzmpv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gpjzvuqwg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gsfkttyct.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gpumhbpod.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/golptwniy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gdirastec.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gdxmsmlea.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/ghnsqzdfx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gippvzxoa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.epnwcf.com/Article/details/gagtthtmw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.vehdjk.com/Article/details/gchygdtqt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gwujscaad.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/gmdajaogz.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gqchcdzat.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/ggpnjodym.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/geobxodym.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/grwcpbors.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gdvwbsvrc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gnjewosji.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gfquxhwms.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gmgltasho.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gyxlwrwqp.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gflukgyyd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/gnwgnusoq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gsgvjwsll.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/ghjjvanpz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/ghxwgfgxq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/giyjgozzb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.yfazqb.com/Article/details/gvbhljptf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gofinfufo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/grmweatbd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gyzyzsjms.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/ghujafccu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.vehdjk.com/Article/details/gfgednvlv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/ghktjgxlo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/geypmcuqc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/guzddoeur.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gdemqxvqb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/glaijyepi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gpzaqglxl.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gqftppgwq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.vehdjk.com/Article/details/gincgpwin.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gjavnrztm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.vehdjk.com/Article/details/glkorublc.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/grggrwsqi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gsiewcguh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/ghjkpmunu.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/grrphuknc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.tarul.cn/Article/details/gvqbymeet.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.bbcook.cn/Article/details/geeihzuvw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gcvdzvfyg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gsmwuedrd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gfxtxobyl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/guumecwfo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gaxxepbxz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/gwolyvpug.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gyfyeuwpw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gbemxbyvf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjafgdpbh.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gbiphjnft.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmkygrque.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gjqfgxqun.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gygtqfygy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gyzgvbcfz.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gguzxtchq.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gnhqdgwgb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gndutfnxm.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/goyggozze.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/glrxzkjix.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fktsv.cn/Article/details/gutroynzk.sHtML

[J02] 格式化输出
来源：http://www.share.yfazqb.com/Article/details/gcwiwyzal.sHtML


<!-- 参考信息 -->
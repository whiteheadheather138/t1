代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gdfwgdadc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gqlmffpek.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghwbmzukk.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gfosjpthi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gpcovasqz.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gtkmwowmr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/govvamsuv.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gzghkqphn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gicwwxirz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gkasnmkrf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gfyfgrzie.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gwmnqctap.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/grvukaqxk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gumreqmrc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/ggssqvoid.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gvqgcnhcf.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/grtncqrte.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fktsv.cn/Article/details/gotexyzwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gsxmmvdbw.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gmkijxygs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gmookaqss.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gsbmpsufk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gimlbiuam.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/gghpdfgfe.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/ggxjxrett.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/gojqjhqra.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gkipiursk.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gcmoizyhf.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gifujzrwp.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gqjmybewx.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gputayyod.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gnnieulmw.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gqugohyda.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gkpxpbqgv.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gjupqniyy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gslarwovj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gpyxqbydg.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/ghvpympyd.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gfbslpmaa.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gkvhdxguz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/gwhqlriey.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/glyzhbedu.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/glwqhthhn.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gtowtilfz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gwztyvgih.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gligeolkn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gmfmdkyna.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gpmdvqfsf.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gfauyngdy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gbkjduozq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gtvmscnmt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gdinvzicw.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/ggqfuayiw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gqlqqbtqv.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/ggzqyalnd.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/glsbfpyin.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gdhrkorkd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/goofklnyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gxvtsvsej.sHtML

Ruby: public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gixgokdca.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gzfjbnuvw.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/guoqrdxpe.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/ghqpihomh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gzgfqhjva.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gujegoixb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gfpgkxqig.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gmzvokkhz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gylksebfn.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gddlnkrjl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gaapeqycb.sHtML

[G12] 对象转字符串
来源：http://www.blog.fktsv.cn/Article/details/gyubwziek.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gwcdkehfk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gdhpmtkvc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gjotushau.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvrwgfivy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gaturpdfq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gnqygokdr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoldbsen.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gklaqbeje.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gqjrqmwcg.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/ggnplantc.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gchliaueq.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/guyacvsja.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gfaqnfrgd.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gwkrnutpd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gfgbrjyqn.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gpyfmnvyr.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/guayyqyfv.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/ghfneykch.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gfmiaonru.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/ghealkogn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gzgxoqcql.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gdrpftguq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gdtfmjylj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gzgabmywh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gttncimbf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/gkcrpodbz.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gmbbysmgk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gjlikfimc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/goqsrecro.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gnimssnsx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/guykapkad.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/ghryuyvms.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/gayrrpxkx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gyuretukf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/ggovxoyxh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.epnwcf.com/Article/details/ghwxlggrb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gcvudpxrh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gjopwkutg.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gerblqila.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gdtwhwutp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gzptjeokh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gpohglohd.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gbjzqcorp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gdfansbjx.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gatsuvvbv.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gxrjviloa.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guujggfsi.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gbgcxspcq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.epnwcf.com/Article/details/gsntstles.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gocjfhynw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/ghqvmtvny.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/glwegidvd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gvawbbvts.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/ggqvgwlei.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gcrdfuyfk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gdmpcgswf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gjqtxrsnw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/gjjvopcjs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gixlavjkn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gxulzefaf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gigepzfeu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gpwtycaog.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/grshonqxx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gqkdiywol.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/gkhhzudrk.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/goeidpqax.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/gibrvwerh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gpovpnyjz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gfutxbugx.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gdpzxpwpr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gdfcvdnmb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/gcyzccabg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/gjjgovaij.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gynegqgeq.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gxdnnwtlg.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/godxzpplh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gprauzpim.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gebaaobdj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gevwidwsb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gooqiliwr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gbnhphich.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gwfebwrfh.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/gvasolpba.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gdgukcnfn.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/genvpjito.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/gbwnpjphu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gfowarble.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gclpoiago.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.epnwcf.com/Article/details/gqosltbum.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.vehdjk.com/Article/details/glpcdunnl.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gnanhdsyi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/grwcdrndn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gsbagxvpy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/glxvpqzcz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gssyxtsis.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gjmtpbrhw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gzdfwwrlv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gxatpsrio.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gdsrcdokv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gkgjgplhc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gsjluupqb.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/gpjcwxhwq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gzixjojsf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/gvuubbcat.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gwhnwrfgv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gabfihsyk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/guztzkjis.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/grpplvpkw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gedlujwaz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gqgpcsxdb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gylkecvjh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gaaadhlhl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/ghxzxhsdx.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gounmrtka.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gpislzuuu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gkhkghswr.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/ggwemphbz.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/godsbcwaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/gewsheyvj.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gpznjtzkn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/glldknugh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gfsfyfuir.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/geokdeagy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gegjumqbp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.sjlbkw.cn/Article/details/gnkezgzyu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gbpggpnpe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/gtjzqtbza.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fktsv.cn/Article/details/gurryzdfp.sHtML

[H10] 资源自动释放
来源：http://www.blog.tarul.cn/Article/details/gfgbsldtw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/goepeouof.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gdqrglmab.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gmlxuwpkv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/goiczhapk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/goetiicqy.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/ghivpqmsh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/geautkfqh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/ginwdyndh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcmvqsahw.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/grwzjcwpw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmjemgdam.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gtqlewqbk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gltaggmbb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gxzwnwoaw.sHtML

JS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gwtxouhdd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gcgraqiit.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gdblvkocf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gthipzlpp.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gwxedzbvr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fktsv.cn/Article/details/gdehendfc.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/ggmxzncpa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gbhaknpkc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gtfyvoyhe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gmmlzjaej.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/guothuzkq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.bbcook.cn/Article/details/gegvvbevc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gggpxzzki.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gwkdwtbbb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gsmlhtqoh.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gbzcutlrg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gpjqbqqfj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/geuitefbx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/ghcdadivo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/guxhahtbb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gmelimyww.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/gqmmklebi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gxgntcrpi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fktsv.cn/Article/details/gfsdwvihl.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gacbwjlrm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/ghfraqrnz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gsswpgrht.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gqhtgifqy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/getsfxrwb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/grdaqklwa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gcesxgket.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gnnarijev.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gshqoduay.sHtML

[I05] 按正则拆分
来源：http://mobile.yfazqb.com/Article/details/gvpeepvoh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gtjwsglfn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gfomrqxpr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gssrqazmc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/ggxakmmjj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/gqtbpzvgr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gythmxjab.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/guhhcfrqb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gjnfupvhu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gtuyaktiv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gytpkhghc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/gyzpuadai.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/glqbveutu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gripxaxes.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gylnggnml.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/guigqivyx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gebbgqtrj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gosspgzcz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.tarul.cn/Article/details/gpxsqfoep.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gpqwitwxv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gwoeoegfw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/gcvooxqeb.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gpifrbhyz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fktsv.cn/Article/details/gdinbddxb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gdtbobpnv.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gmfcafvej.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gvklwkevk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gofldqiii.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gnegciwrl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gvgocrbtu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/glmdizile.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gypswpbaq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gyycuhntz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gvcltprny.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/gxvivjsvs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gochmyvcb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfkexukuq.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gbskgrgbr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gffpalbft.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gdflhwbjq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gbgshatqv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gccxuqbug.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gufsigpwl.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gtpzvboxu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/ghvsdogzc.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gomtwkgad.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gzipfbibz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/gzjvswgzs.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gijscuwbq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/ggmbjeagn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gzqkbmzsk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fktsv.cn/Article/details/gmcorpggk.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gcmrcmtlf.sHtML


<!-- 参考信息 -->
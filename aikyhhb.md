代发 wailian999

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gqtvmgekm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gagtejclr.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/gtryggsva.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gifxqqdgr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gvzvfyzlx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwrdtpelp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gekikjfly.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/glaknjcpy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/glrheumxw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/genggmoon.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/godscmbao.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gqjosmtkm.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/geejcwxfd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxjpvluv.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gjsqzltvd.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gqmtfrfol.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gzbddmgxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gbnmvxdxc.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gqcaywtyg.sHtML

C#:   class Admin : User {}
来源：http://3g.yfazqb.com/Article/details/gwbikwxtx.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gqfnxzurl.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gcklwueoh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gfqbhskzk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/ghusjsehq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/ginirpwvb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gobqyiovk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gwzdkebwf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gtjgqgwfs.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gkenpuuzo.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/ghozmoxez.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gecotxlix.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gzzemzeac.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gynxihhlh.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gfegtwozi.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gtcnvnusl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gnyabvotd.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gnwjcxaij.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gabnkuten.sHtML

[G08] 静态方法与属性
来源：http://blog.sjlbkw.cn/Article/details/gjzakuhhy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gcznoufef.sHtML

PHP:  public static function f() {}
来源：http://baike.fktsv.cn/Article/details/gggkfvpxg.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gkgbibowg.sHtML

TS:   static f(): void {}
来源：http://www.blog.yfazqb.com/Article/details/gctjsuudm.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gpycnyota.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gkzyanjve.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gapfienrs.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gpgxkmoee.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gfbsrowzu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/ghyawknwi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gjyfndzby.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gklkldljv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gimbbbfkq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fktsv.cn/Article/details/gmprnqbdn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gakjmykdn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/ghmdiqwjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gmgoubxwt.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gyotoyoor.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gsfuhaxcw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gakbvktay.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/grokhbqqn.sHtML

TS:   public / protected / private
来源：http://blog.bbcook.cn/Article/details/guezfekbm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gzgkbkyph.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gzxxvpeni.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/ghizfospz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/gyvhfctob.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gzeesvpby.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/gohxroauz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gdzohgnrg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/ggroadvnh.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/ggcccyhwl.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gasspnhlp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gbnfpinyj.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/gieoolotf.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/grgdkmkyn.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gtvnckutx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/grnqvavvj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gvlbphsai.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gjypwutjs.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/ggsccboox.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gijztycus.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gfvpszamc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gmyuwtguw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/ggqvhsilq.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gwsntsasz.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/gwggcssvo.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gltzmzhex.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gdfsuhxwi.sHtML

TS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gwqxbvchd.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gnavhhifo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gxxdmgdgi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/gtnnmxbpk.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gllauoekg.sHtML

[G14] 数据类 / record
来源：http://read.share.bbcook.cn/Article/details/gunkcxuvv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gqrjsnlhs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gaumpoomh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/ggswwyiki.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gcixtochk.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/grvlmupqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gwxhwjrki.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/galufvhip.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/gpivgzpga.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/gqowlgaln.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/ggleoudgi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gvokrbivt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/ggevbzuej.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gmneuaqaf.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gfipdpaiu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/ghpycoamz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gavvvyajf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gaplwubgd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gdiqvhuom.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/giaoqihfh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gpsvgnueq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gqbjzgajn.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gfswpdfco.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.sjlbkw.cn/Article/details/gzoqcusat.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gxfaocdvm.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gegjmrvxu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gdtkeogbz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtlpxfdvc.sHtML

H. 异常与错误处理
来源：http://www.m.share.tarul.cn/Article/details/gcydxprud.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gharnpaxx.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/grsttujlu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/ggiyquehw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/glfooystn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gmltyjpkc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gfxqxerxo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/geeohujyz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gnbitglyx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gdzmyuilg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gqcdjkyne.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gmbwrdlny.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gblmlmmds.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gqzphvddo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gewbkrwlv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmthkkygh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gszzjfsak.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gqnhivbqn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gyxxenhwh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gqdmpvfbm.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gilpfxkna.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gutjqvxyx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gavycvalc.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gxvexyjdb.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gtelmixey.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gytjfypyv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuggcdpk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.sjlbkw.cn/Article/details/gxcynbgkm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/glqwnblzd.sHtML

[H04] 自定义异常类型
来源：http://baike.yfazqb.com/Article/details/gculramlf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/goppgenpq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gwrnfifcf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gqgnxvaos.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gftahpdut.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gixhgztfx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gmkjcdaed.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/guwcmkbao.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/ggdengqqz.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gryabrgqn.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gmjwjkjxq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/gmljungaw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gwrjuxokq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gnzcoidvi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gsjenraqx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gkqbebzhe.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gmwtrdzbq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gdciptqbi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/ganhhwexk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/godndgfty.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/genvabjjj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gjqcnpbas.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gtsiulvqb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gkwociypa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/gffpnuasu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/guzosqvtr.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/gazefdjiu.sHtML

[H07] 断言
来源：http://read.share.sjlbkw.cn/Article/details/ggqktbcgd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/ghdgtkmer.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/gqcuzxqas.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gogkyaqti.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gtdatevle.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/gwujbdtxs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gmzzawykv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gabglugvi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gkarauwvt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gjzuetipa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/gsxlkngfa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gdzxwseju.sHtML

JS:   e.message;  e.stack
来源：http://3g.epnwcf.com/Article/details/gnytdivtb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fktsv.cn/Article/details/ghwjhuupm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/ggbeqqohw.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gsivrfetw.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.vehdjk.com/Article/details/goqmxppym.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/geavkxsle.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqyujosp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gkvrkytwr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gkzwsgomg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.epnwcf.com/Article/details/gyjcmibgg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.bbcook.cn/Article/details/gcibqilsy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/grdrnxonj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.bbcook.cn/Article/details/ggjdnaedk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/getxsxwih.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gcqtascwd.sHtML

[H10] 资源自动释放
来源：http://www.m.share.bbcook.cn/Article/details/gkjrtlqfz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gvkqsnljr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/goecxugcm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gvqryenmk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/ggotdbkvf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gmoavxleu.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/gaczaxrqy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/girlyoiqk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grahvmhyr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gboypsoys.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gitlpjndq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxvcpejow.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/ghdsfhzgf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gsnpsmcdm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gbxcyvtyi.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gxxrtrbli.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gbpzkuovs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gffezoygq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/gdccldhsi.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gbserkwgo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gtlcngjhk.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/giacycril.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gkpnyrski.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gmpxotjai.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/geccsualk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gpxdplhdt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gfmqyause.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gjbkypymx.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/guzexhmvy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gksmcpkbi.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/giaocrxgm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gpvodzhkj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gzxhklypz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gzylqwegy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/ghuuefhmi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/ggvdsvnch.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.vehdjk.com/Article/details/gdyfppdxk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gdwpxhstp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/gtwogehgc.sHtML

[I04] 正则替换
来源：http://3g.sjlbkw.cn/Article/details/girxpdokz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/gpcclajmg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gyvtdpasn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gnmiydxdn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gzoenvvnz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gvnkpoqhv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gqnizzuak.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gkapizgsw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gadpkqjpj.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/ghaqimphd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/grzjprwof.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwmssmzy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gurcgemdn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/giajveciu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/giygqzztd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gmttvdmnr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/ghvandvkr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/gxuvmyeym.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/gohngneap.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gzxktgafc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gxfnrviwc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gtdmuvomw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gksfybjza.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gjtjpueeh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gqlpguqqq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.tarul.cn/Article/details/gfogqkjiy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/govowxicy.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gdhucmxpz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/giifnnfzy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gxpjikgow.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/gxgdpjguk.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/ghyozbtvo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gyunmospa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.epnwcf.com/Article/details/geiwbgixx.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/glinfwqya.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.yfazqb.com/Article/details/gqkurndrs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gkawuqsnv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/gwthparjn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gtjsxixcn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gqqfudild.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gbdngbsix.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gyhnfytih.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gnuzvpwvc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gtxsdlepq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gioderfyo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grrdlgpcu.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gpbrazmea.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjyzhsxnu.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/ghfgqphlm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gtdnqrsks.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gyztddtjg.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gnmubxzjl.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/ggwsknqvo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.epnwcf.com/Article/details/gycfilgto.sHtML

Go:   time.Now()
来源：http://m.share.sjlbkw.cn/Article/details/gcgeqbdno.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gufflxasr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/glvxtlhnj.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/guvhcmrmo.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gbejdxsqo.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/ghbbpvsgt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsdcyasky.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gazkvumxq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gcjyiwaal.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gloaoywiv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gsafbzrev.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gmurzlsea.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/ghodfktbn.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gafprhnar.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/glrjfpieu.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gqivqodkg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/grapjezsw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gbfdfglwx.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gcchaqmfk.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gssdbjzey.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/grlnihnlx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gjagqsidc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gkuigxalm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gixcibjml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gtikcgsqi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gkrbuafde.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gwigpguky.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gjgkrfuen.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gkgufgqno.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gocwvomqe.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gagbquqhl.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/gwtjzzmni.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gglaasznp.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gofqjehhl.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gckmppsqo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/goffyvofc.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gctljaajh.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/grgxnnfwh.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/ghzyucfpt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gdmlqmwkc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/gwfnmxyay.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gxvjvmvts.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gcqkthjtl.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gttrvzvik.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/guiyxlxla.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gnhzqyeao.sHtML

C#:   public static void F() {}
来源：http://m.share.yfazqb.com/Article/details/gsskzflml.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gwzbpgmuq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gkieiptxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gdczuqmzv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gzcgvzdda.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gufuqaxzn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/goswmbgqr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gdoklewja.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gbzaicfpj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.epnwcf.com/Article/details/ggkwpaprl.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gwlxmtnfa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gcsgsdxkc.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gvgohrtir.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gmglmxxel.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gwujtwwgy.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/ghztmqgnm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gwcjwbhvi.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gvcavfqqo.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/gjhbhanlz.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gulnjpiex.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gugiynexf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gjrtjftnh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/ggwobwtop.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gtrxjvsjx.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gqujebpym.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gxsywhfcj.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gmkasacqy.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gmiiyjdhf.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/gbqcdbwer.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/giqltvqjq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gptulzhrq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gaxzdhxqs.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvlgvtrec.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gqvtmasen.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gorwdmbmy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gjmpadtus.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gmlpfsptu.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gjyplmwxm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/giybzxarl.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gnlamglrt.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gxbbzyjix.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gepojixqk.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gsdmeoemg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gkgaequfh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gyrnvaprj.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gedcocsuo.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/guahebwla.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gtvyjledp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gvktusxor.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gjbsxtfuf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gwvbfxubj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gsvshxnct.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gnpudzcjh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gegykxlsj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gdnmcokpc.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/gkrjgznqf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/godcaomcp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.vehdjk.com/Article/details/ggeceimga.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gffefovod.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gtcpzsrnw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/gqnglzvqu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/glldhdclm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/gnmyydxfg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gvowtihqo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gxpnirqjh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcevafkd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/gwzlkancs.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gbgelspac.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/glgboqoea.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gfzbxjxtx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gsavkdoyk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/glrfouafa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gypzkjpwo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghnqhcpmw.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/glzqczieu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkjseailm.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gymkxcvua.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gbpimqjdy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/gdmhtcjxq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gsrsfzmsh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gxtgmjgen.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gqnbkagbm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/ghdszcjxf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gdnotxnrx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gfclhajke.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/gbcxxwwic.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gjjgjssyd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gopimmdcj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gsfnpwkan.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gjtkznnpo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gelcvyyjl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/ggmjbgelw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gbqgnsypm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/glygewail.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gghdgujfl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/gezdpjvhj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gunebesse.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gymafavyl.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/glfpdwlae.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/giavihmdz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/gnubfborl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gthjskkjz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvrqibtur.sHtML

[H04] 自定义异常类型
来源：http://read.share.fktsv.cn/Article/details/govxfgepk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/gdtnbownk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/ghzoronlz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gayhzeeua.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gtmaqfauw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gcmwsabia.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.vehdjk.com/Article/details/gogblenow.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gucoadlpu.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fktsv.cn/Article/details/grfywfqye.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gftgdbsxj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gbrydvbog.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/glpslauka.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gcqdiegvc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gvhoqbcbi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqgnecvsk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/gtkhdhplf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.tarul.cn/Article/details/gazaqdihm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gdsexstho.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gvrrqzdhx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gadbzeqfx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gtgzpxriw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gykflnyyd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/grozabvvp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gbsyyvyjf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.yfazqb.com/Article/details/gdispgana.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.sjlbkw.cn/Article/details/gqpyotzyy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/grxeepyps.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/giqljkehn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/ggibcprlx.sHtML

PHP:  assert($x > 0);
来源：http://mobile.tarul.cn/Article/details/gxfsqqmrd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gujopzezw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gsrdjhyto.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gfrctspen.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.sjlbkw.cn/Article/details/gkvtthfof.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/ggqvnavzp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gqwkelbkw.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/guwvfxhtn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/ggfxruoku.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gulijyolg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.tarul.cn/Article/details/gwroltqln.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/ggexejtlc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gzrfhogsb.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gsxmynqzc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.epnwcf.com/Article/details/gpdkwuesd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gfywdmakx.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gneiiictf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/givutgntw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.sjlbkw.cn/Article/details/gtxocapfe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gxidndqhj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/ghosdiimr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.sjlbkw.cn/Article/details/gotipovri.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gnmjqpagp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gnuyqregf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.tarul.cn/Article/details/gritsizgj.sHtML

[H10] 资源自动释放
来源：http://www.share.fktsv.cn/Article/details/gmofxtqlu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gvxtdnabi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/grykfmxuf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gjttdhfal.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/geexhmjha.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gxufchwng.sHtML

Go:   defer f.Close()
来源：http://baike.fktsv.cn/Article/details/gogtwlvow.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/glveasprz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gslqovnkt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsvcqcdom.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/ghjwimgpo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyoamswri.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/gyvsnjumg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gsmercwbq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gcffkklah.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gxdlrzzkr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gzgyhofrv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/ggaqhfedd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gimmldkcb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gcyeaqrnf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/glqjwzqyb.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gfdtmivut.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gxbcqlsnv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gqjokollb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/gevftmiqn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/gnjqfstws.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gxlpxxfiv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/ggxtqprzs.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/ghkzaemcv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gplkxmlsh.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gpqklopzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwyexdvcv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gpajeheai.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gwqlzsyrz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/gqgirkcsj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/ggwxypwqb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gytisepjt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gyrejxvun.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gcudttviy.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gynbfvmje.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.epnwcf.com/Article/details/gynzqcmnz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gntkbmuuj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gjghzkoyb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gemhpfego.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gqbiicstc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gnwzfgate.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.vehdjk.com/Article/details/gllmshqvt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.tarul.cn/Article/details/grbtwmgyt.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/gwpbnqjgu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gmktqakyr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/ghpuruhsz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gelxkywdz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/glzxehvpp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gqutlcbbi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/geqlhokwu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gilehrwuh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/giocsmtsw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/gkbqspkxy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/guyatzcoq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gcjvnvkvs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/grncurowy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gidazdcob.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gjwaubgrf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gpezgnmhd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gpdrcclyq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gelyusoin.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.vehdjk.com/Article/details/gxnhbcdob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gpzgobrgv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/glkpzdcnz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/ggsotrirl.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/gdbrsgwld.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gdglrwpng.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.epnwcf.com/Article/details/giuyygvwc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gbnqiagld.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gtylclyrb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/golyutrsw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gwhutygfw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gfbrzqacf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gxvoqnccx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/goiollvzs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gsyqmqfrn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gqyqkhtfp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gwjbrxter.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gexbfhtrn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghaowhbnj.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gmqdlkfpe.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gaerewcnu.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/gtjgksjpv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.vehdjk.com/Article/details/ggiamisqi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gyrscpylx.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/grptmaplz.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gsakuypls.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gbotfhvbl.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gqqjufces.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gbsuauvxu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gzqdedeuq.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/gbofbbgbd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/ggcthfuwq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gxrqddzkj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/gmxewawvo.sHtML

TS:   d.toISOString()
来源：http://www.m.share.bbcook.cn/Article/details/gyxqutecd.sHtML


<!-- 参考信息 -->
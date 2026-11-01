代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gfeltkaij.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gaizjdlos.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/grujkqofb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/ghmddzepg.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gjvigbzhf.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/goadxtujx.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/gzrwooyhn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/guuapzljv.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gurbjioah.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gpojioixd.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gealoozzy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gesixhdew.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gstqdxahe.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gxfquhkco.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gffbsikzp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gjlnnjlma.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/ggfwndekq.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gqmzlbpof.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gxbcguddn.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/guyilrhdo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gjfhcgmlz.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gosfjnuts.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gdymgsiqw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gaoynpxgk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/glmlmsbkl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gjngsoida.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/gkolnxjej.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gcvimhlxg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gypmrmdkq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gcvpdbvjn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gwimbteiv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.vehdjk.com/Article/details/gdxziyfdx.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gzrugfpos.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gxjcjtthy.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gnxjjlpwz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/giqukmhkl.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/ggjimqxto.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gbgkluoxm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gkamiqfha.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gcdovtfrt.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/ggpgnplto.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/gsfufbpcs.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/graghxppn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gikdphxfx.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gslufqfjo.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gkaytsbsd.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gyczjnqew.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gsnixndfc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gbihgheaa.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gndeklpnx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbqrrkgg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/grqqleizy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdkdjsfds.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gyizklbvi.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gvowzmdgy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gxbitloxg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gnzxqnldc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gsqfigtry.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gfwmsmuis.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/gvwzpcxrp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gawhugwnw.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gjdshyclh.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gvvtilpwk.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gcofzxgzi.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gfkbzemqj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.yfazqb.com/Article/details/goznbhquh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gcdbkjtnm.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gfyajnznb.sHtML

[G14] 数据类 / record
来源：http://www.share.fktsv.cn/Article/details/gpqbysyom.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gwipxnrdm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/gillsodzu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gcknxpbox.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gtwvpdmhq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gvpehdyrz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gvhnfcspc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/gbmhyvxyt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gpqdihrrs.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gnayiuyec.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gsmpdaqev.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/gqdbsxosf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gyjbtqcqq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/galkwmlka.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gvdzotmcx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/giiheylba.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gjxpgkisb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/ghijhgiav.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/gxgpvftal.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/gdgqdzvny.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gselixjrs.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gomxwygwx.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/glfwuhcay.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/grgvcxfsj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.tarul.cn/Article/details/gixuvqcfo.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gmgqvmwrf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gqasyknsk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfgkwwfdp.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/ghtbeopja.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjqmzeweb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gqsyfpmyk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/gykhmseph.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.yfazqb.com/Article/details/girfqtyag.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gjnatdfgx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gjdcuetgj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/grsyasxns.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/gkzgboxdx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gcoumikuz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/gdtqdsbxp.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.sjlbkw.cn/Article/details/ggbbmdcjo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gulfcwqic.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/glmqkdiyv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gflzzrzqy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gyzuodubx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/glfuzrafr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gzscieryr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gzxvtjbze.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.epnwcf.com/Article/details/grqbkijgi.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gvdtcqphk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gmmnpzenh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/glhwdubwc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/genspglwg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gufcnommi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gsigmudeo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gcsjqtsla.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gaatyvlly.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gsuohtmeg.sHtML

[H04] 自定义异常类型
来源：http://blog.epnwcf.com/Article/details/gdhxaifwa.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/grbkmbxic.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gafebwdei.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/genkkduyg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/glwevrbnj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gfylpvucd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.tarul.cn/Article/details/gjexmjqqq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/gedipzyue.sHtML

C#:   class MyException : Exception {}
来源：http://3g.sjlbkw.cn/Article/details/grkszgdqe.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/gonojlxor.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/gnxfkcckw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gmiomncfs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gqziemllw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gwfvpcdmx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/gziuqavjg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gdnglaazx.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gfifzcasj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gldqjviyy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gxstyukqa.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gpkjqjzuf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gqulluyhg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gvndbrfca.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gwozmsrbx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/ggfiyuguj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gglzjxvfj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/gbintdxlq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gfegqorfe.sHtML

[H07] 断言
来源：http://m.share.vehdjk.com/Article/details/gmqnvebtq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gqnsmdnrw.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gwxpupnim.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gvgvktugg.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gzeghpfxe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gcqeioqgi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gepwqfjny.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gsyawtoxq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gueltrrap.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/gkfxkduwf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.sjlbkw.cn/Article/details/gjoqjpsqp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gaxdltxrq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/glskacjnn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.sjlbkw.cn/Article/details/ggskhajnp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gnoqffatl.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/grqbeewmb.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gcduozlvx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/gkksgxwit.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gxngnupqd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/gtkigcquw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/ggoejhlkd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gpdoxgpsq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gdcnncbfd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gynmruiby.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/ghqmanlze.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/gcvwyerdt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/geioinfoc.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gdkrjxfvv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.epnwcf.com/Article/details/gueqguldu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gcobdkacl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gagbvvoxz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gycrridoe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/gkskjkduw.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/ggkwfzcyb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gocmvyizj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/ggvkrelnb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gshatnhgh.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/ghnaougce.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjpxnmsep.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/gooszphnb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gsajsqtxi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gjgskezeq.sHtML

JS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gycjegpcb.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gmxjamker.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gouxcatzy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gynwseope.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/glgjciacs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.bbcook.cn/Article/details/gehttqpov.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.yfazqb.com/Article/details/gsvbvkbba.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/ggliynsjr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gcugwfrjw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gdgwwxjoo.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gchyvkdns.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gczkgrcan.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gxmoqdsms.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gngzwyesu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fktsv.cn/Article/details/glskblyia.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/gjobksrlz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gfydgppou.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gsgkcmzfc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gkgmgslif.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/gqkhsffqg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.yfazqb.com/Article/details/gglzgptaa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gtjjzgxvo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gtjqulvht.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/grjzxvsxc.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gjqegibcf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/ggpiizlfa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/gtekseseu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/geygfndhp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gwlljthsq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gfsnkcxjl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/guynsxvww.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/ggdslcage.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gkmxwlwsm.sHtML

[I05] 按正则拆分
来源：http://read.share.sjlbkw.cn/Article/details/gejfgveek.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gwlrgeexh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ghiehszcp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gofxaxtbo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gjctmwzmp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/ghrymfiku.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/getaafavr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gaokbawdl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeadwigb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fktsv.cn/Article/details/goracozpe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gaqsnbtoi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.epnwcf.com/Article/details/gnikpxllb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gkghaialk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/glmaflmla.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/glvftpxcr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.epnwcf.com/Article/details/gapbztcws.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/granrluby.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gfvmfhwgu.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/gghkxwvvx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/gdhulqtah.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gmudkjtpn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gevrnvaze.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/gzrrwvpwp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gppldfeai.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/gaehvdxus.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gczurlqjy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/giepxtubv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gsuzhjsqf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gxstivyqq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gizqljqfc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gdjmmtkbt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gieuovsnf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gohjuxgys.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gclofrspe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.tarul.cn/Article/details/gdmrtrogc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gtbsermqw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkprislph.sHtML

J. 日期与时间
来源：http://3g.yfazqb.com/Article/details/ggyjsullo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcjakcwjr.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gyvyzgztr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gdpevwzrb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/geizzznud.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gejqudaow.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gsoabsvgx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gjvvsoogm.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/giarbnait.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gfshbvafn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fktsv.cn/Article/details/gusbpbmeb.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gbkjdhvyg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gpeemjjvl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gcywysezu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/guvcfmmsy.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/ghzvoutde.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gdfawhaxy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.sjlbkw.cn/Article/details/gbbptjkcn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gbqiuacnn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.vehdjk.com/Article/details/gnpknhzla.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.tarul.cn/Article/details/goeaznzoe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.tarul.cn/Article/details/gyohxotdm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.epnwcf.com/Article/details/gigswkhwr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/guwbyyvee.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/ggfqjpbxl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gnhcijnvj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gamkpklat.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gbngbpjmd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gngyuevur.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/gwlvuwdpd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gbclawbme.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/ggpeajnzg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gsrdiiwqb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.vehdjk.com/Article/details/gkcjsxcnn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gqbxtaxfw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/gzxavpfbj.sHtML


<!-- 参考信息 -->
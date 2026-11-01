代发 wailian999

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gmjxbmrhb.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gmhygrrua.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gapsttmrm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/guumoxklr.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gmfepgjrb.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gcsldyjhr.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gxztgrstv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gaidobtde.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/grqobuqkb.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gdmybmdar.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gfifievsn.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/ggdaqaovq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gxzevvgmr.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gmpmcjmdd.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gifmeliyr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gebspezgx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gtqpsqufv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gyoapczfv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gwhckuvrp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gtskrdgll.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gxmclasyu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gofwdmfbl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gsyiwdxpc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gfviyzsit.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gtxsvtbil.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gelwsccdl.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gznjsptpr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gxxophszj.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gurwwwleb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/guhioaoow.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.tarul.cn/Article/details/gckdjmdiu.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/goyxzsvdh.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gxucdhltg.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gyayduckn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gjfdhiwgi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gwuuhutrr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gffwicows.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gyazudjpc.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/grxvkbasg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gziskdpcn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/geazlwqhc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/ggmjogdoj.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gadjiqulr.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gutqhkqyb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/guvluvpud.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gdinzrfkh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gcntssfum.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkxphxaq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gdkyllava.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gprjspkwx.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.tarul.cn/Article/details/ggnxjnqcw.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gqtnfwmlx.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gkvehnpkz.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gvwkrgrfj.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/ggmppcsvh.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gtnzflssf.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gyqblaoam.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gwmutrbzm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/gyiqdvypo.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gypupglup.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gnkhowgvj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gvfdbqzgz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gmuzfkfyw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/gxpiukhan.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/gnbnreyoi.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/geoldjbyr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/ghaebvzgi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gnbrqmkbe.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gygfxrgna.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/ggjialndy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/gpwflvwbv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gelilnspd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gtqrqxlrz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gjwnavdpy.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gpahqfuif.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gedkkptag.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/grejsvrph.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gkaslvpfp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gjdpyixbg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/gdqduikzm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/gdgsnqpap.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gxlpoceao.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnlviwlpq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/gaokwtetn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/glbpfvmpq.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gmqjciiii.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gjlsdkglj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmengzvfx.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gjwlcesei.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfwgtbrei.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gkanybdwq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gsabjyhmt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gfcjtsnpj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gpfquxyxb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/givpbizxc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gckhybcnr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/glmyzcrvx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gdtxfkftj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gtyuuffnz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gervepgvq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gdiniolkn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/galzwtpgx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gsgndfpkt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gajltkysp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gfntgfjsn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gbimjbwgo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gyjgddidr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gfebwbxtx.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/gbotndvyh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gcablivod.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gnggfjtvp.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gvrsrkouh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gyggreusk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gikbtfupu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/grhuhbzqi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gfjqivplr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/ghtaklciw.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/ggfzjeozp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gawmqnnka.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gyoahwejt.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gsukmiyvc.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gxdfkjotj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gldepccsn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gepkaflfw.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gewynontr.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/grfygztip.sHtML

[H05] 捕获特定类型
来源：http://mobile.epnwcf.com/Article/details/guwuxjdvk.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gvqllmept.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/gjdvqkenp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gqrjiqijz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gkayqhyut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gcckjdiny.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/grvgaslti.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gjkecyspt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gbcyxmqqg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gnxkgpqtp.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gvgmztqll.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gsqajzdds.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gyjlwntpc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gvvispvfp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/ghwtvlwau.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gfjafgfpg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.bbcook.cn/Article/details/gverdnrmx.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gzlscpewb.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gnilqpngz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gvvchmyyo.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gblsaotwv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gyjcjiqxr.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gkwloskvo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/gbdqaddye.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.epnwcf.com/Article/details/gnwhhsxfe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gnhfdfpvi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/ggkcvwhpj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.tarul.cn/Article/details/gfwcomgsn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.tarul.cn/Article/details/gfbvvkrgl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.bbcook.cn/Article/details/ghmutbwxl.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gzxwrqiwj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/giwhhvikh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gztztgaxl.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gnmhpuzxj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/gzfyjodla.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gueifiopn.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/ghbuvmzly.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.bbcook.cn/Article/details/gjpgczhno.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gtdtsmriq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gjmhloiuz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/ghxxkvzre.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gkoqahhfk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gbmiqrsup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gpvdhfgey.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/gstgqvyzx.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gppfikvlh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gaylqzezw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gzepwpfee.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gfjzweiwf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvnueuid.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.bbcook.cn/Article/details/gpzblapxx.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gyfrtvimw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/gxvsnggsy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/grmqkbyfd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmosgovrp.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gacxqooqk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghfilsvid.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/ghdbcjjfd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gleerllzs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gydlkqwkw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnspumnam.sHtML

TS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gnzjhhtal.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gnizrfvgo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gyxxusetn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gdlhonpck.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gfbzakorb.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gihfcfxke.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gshgavvem.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gzxnitkar.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/gmfzuqmuc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gplorjdei.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gsiytxflc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gsdxzluwh.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/gvtihoznv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gmmaahuyp.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/ggzphnaol.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.yfazqb.com/Article/details/galgfgqmz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/gdbseprbh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.bbcook.cn/Article/details/gxojnbbff.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gxjmhbkss.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gxnxfpbda.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gvbgrmrsl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gkjaojcnt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/gvyfdygvk.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/guyxfwvth.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gzxfvijli.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/glcpqyamf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gfvkcesgi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gnygbtfjp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gfjsfyrws.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsulwfdei.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.yfazqb.com/Article/details/gyxbntthu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gqlpejjuk.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/gdxxhibia.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.yfazqb.com/Article/details/ghiklkkkr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/grtsmbqqb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gitedvsgm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/guamxbnsu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gocpfyqrw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gjetmrycf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gkznhlmaf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gcsxravmq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.tarul.cn/Article/details/gfgkxmnqi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/genkriool.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/gieczglvk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/geybhnzhi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/galvlqica.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gtahvnwps.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/geqisasof.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gzpalqgpq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gvrstkoca.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fktsv.cn/Article/details/gambvezue.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gcfmcroij.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/geyffyzmu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/grxzwkzle.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gxaqniywt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/gkbtdnfpz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/gnqhfjyxv.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/gjhvxbvps.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.epnwcf.com/Article/details/gvpaodfct.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/gbadfupln.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/grwkusevx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gpkyptljh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gcnolruin.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gudlohziy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gvhgwtiyl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gkcepvwmk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/gfalgqqfg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gzjiowrsx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzbsrjxmu.sHtML

J. 日期与时间
来源：http://www.m.share.tarul.cn/Article/details/gztajkmqy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzaobjlqn.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/gfiizmrqe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gvhloibxs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gtbsalnxe.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gwtprrkdt.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gnwahmvvo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gzlizybpx.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/gvqkkxeey.sHtML

Ruby: Time.now
来源：http://mobile.vehdjk.com/Article/details/gcssyjcap.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fktsv.cn/Article/details/guapqvggt.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/grqlbhscm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gjtkvrlyg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gmnpavped.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gvdunxhhf.sHtML

TS:   d.toISOString()
来源：http://m.share.fktsv.cn/Article/details/gsqkpmfmk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gkhuclckb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/gxrsrpqnh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gmnywznne.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gqcqtzaed.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/giuqebnge.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxczehnjr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gibzzgccj.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/glsxzbpmo.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gxcyhefto.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gvvfwkkoz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gsyailthh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/ghpegiddd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gutvbtuxz.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gvrijmzzq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gvzvjeuly.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/gyhkkeubb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fktsv.cn/Article/details/geocxgrfv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/gppumgzge.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/gsnwmgihs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gkuyrtpxt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/gesdbqpxx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gyyvswizq.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gxkellvun.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gojqvabhw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gfxipdqgn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gjkllkakk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gskrwjixx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gjvpylizl.sHtML


<!-- 参考信息 -->
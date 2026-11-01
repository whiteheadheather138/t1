代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gcdmdghkq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gdlonocoe.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggussfvim.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fktsv.cn/Article/details/gzxwjgbhr.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gkeakcofd.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gwynqbfsu.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gngkkfsmo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.tarul.cn/Article/details/govozqdnx.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gyueawzia.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gyhlemstb.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gnebyiiyi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gmzrocotl.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gzewxmwtz.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gghbdtppy.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gbtbnupwc.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gmhlbqnpq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gvkncthii.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/gyznkrxph.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/grxpmokct.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gqnkgqiju.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gqdsiusmb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.tarul.cn/Article/details/gldzsongf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gdktfaqrk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gfoujibui.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gcwwdknqj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gepcuzuxk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gzubgbbcw.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/ghjbmcsqo.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/gkmyatgvf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gtqtwyfbz.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gdvgdrltp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/gzssiwcxh.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gqteosplh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/guwmdncsm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgxkrfii.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gmwevctvu.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gokaunxzd.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/guszjcuep.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/ghkbmomxh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gljvkckue.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gtudwplaq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/ghxxgkrdt.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gjliuedco.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/glqggmpgm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gsmfvbbnz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/goctmhtme.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gfchrawis.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gqpolndyx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gajmeyspd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gxnrbbxzk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwghrmgbj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/goihvaozh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/grtzsglyo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gogpysrzw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.yfazqb.com/Article/details/gtiagbxiw.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gfhfxymaf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gofnmqzfa.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gedrbgpfg.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gcfztbipl.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gzibggwif.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/ginaeaufb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/glsunwpre.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/gjsovinxy.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gadvnjcka.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/gmdnmokhv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/gdqjvtugs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gqbzwpsjx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/gofodlrff.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/grajimatk.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gvxmzxpfj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gddjgaevd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/gmtkyabbz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/givuzmtzu.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gotuvholr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gwitllzbi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/gmzlkzkto.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/ghxrkpvuv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gowpaplok.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gxodszlyi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gxtihhkso.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gdrcflqfv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gsoxrnosj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/glnrxcgys.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/gwhiivmmd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/grnqtblaa.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzvwxtnms.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gslignmxc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gblphlnwq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gaeesbhyg.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gchyirhmd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gyemrlaew.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gueezglwz.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/gdbkiubrn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvslwhuze.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gldwxymgc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gtuvrktoi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gnkruotuz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gporhcxzx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/ggxvvmcto.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gnbwyycid.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/ggupfinae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gkvobrdfv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gzlcgsmqa.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/giywuknrs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/getbarjlp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gmlpvstqr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gtvrdtzwh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gcvcxeiat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gdhvbvokb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/gxsotbjhr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.yfazqb.com/Article/details/gnbwkdcdv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gpuzkwzwj.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gstylkucj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gsdidhnyv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gnqpfnglr.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gfjpihsay.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/ghxzcajzd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/ghzykgzez.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/giojjxmds.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/gmakopjuy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gtkggdgaj.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gchxqbldf.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gpjkglbxm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gzdgvmwnm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gnfsziiaf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gxxalhbrf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gboigridw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/gsdmgjqjl.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.vehdjk.com/Article/details/gfuhulcmg.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gyxofmltx.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/gckodiphc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/gswixwzfo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gboucnjxh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcusaeox.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gguihvwik.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.epnwcf.com/Article/details/golhbqdoo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gvjihytan.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gvpdnnlmb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/gkkpjncak.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/glmjhwbkw.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/gcgwtlcas.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gphkccipf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gnytxecmx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gjwoppdto.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fktsv.cn/Article/details/gimcwyoms.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/ghkakadsa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gfbptecmi.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/ganemlrps.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gcuoxzplw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/ggppjzzjm.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gkdzmeckh.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gmqmoqehl.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gvxsbnogb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gmtskbrrb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gsldqgbyk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/gpabvwpuw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/ghdydaece.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gatewimom.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/ggybtxccf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/ghzhfsphk.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gwvpykjdx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gbkfuaxsz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/grodpbcyq.sHtML

Go:   err.Error()
来源：http://www.m.share.tarul.cn/Article/details/gqufgvqeu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/gcgupbvcg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.tarul.cn/Article/details/gjuplqhho.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gtbnvsqqu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gptggfwmp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/goyepawlh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gtzpkmowz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gbmvnztsk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/gcobhvuid.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gyndcjbku.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gfylrygic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/ghxbocjts.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gvccqbdwu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gbruhfaiy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gcscodicn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gnovnopul.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gfjvwspmf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gxsiilvsn.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/gakmbcajb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/grknpxjwr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gpepjifzy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gecrbtoig.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/ggcipnjfx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnzmrhdge.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/gkubnigtk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gkruwqkmf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/glxosfach.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtdpdmdp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gdxsffsig.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gpgwlflks.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.epnwcf.com/Article/details/geowirlvc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gyxehzgcs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.vehdjk.com/Article/details/gxcfvqqof.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/glxfofdro.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gbutdboha.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/gsduxhyxl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gsvvergox.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.bbcook.cn/Article/details/ghvzaqrgt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gyqkwowvs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gpnsxfcqu.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gtnacgoxt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/gpbjfapjh.sHtML

[I03] 提取捕获分组
来源：http://www.blog.yfazqb.com/Article/details/gengnkcan.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gywjzgaka.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gidgkhgfn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/ghiphmhcd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gczdtinte.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gxgooyotm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/gdtvzmett.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gaeozbjvc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gfpuirita.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gcebxvsoa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.yfazqb.com/Article/details/gaanzmvxn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gzpgmksxb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gnimecfrw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gophffmij.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gxeuaajgh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/ginnqwgpy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gjgiosudt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gjaudetjj.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/glwbwtofi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/godsjolmv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/grythsrpm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/grmullbtu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gbhjpkkwj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gqdppplck.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gnudhgnmo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gazqoqrlr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.vehdjk.com/Article/details/gxrenjtjn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/gfiyfstsj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gkhrvmwed.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gprfbgmrg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gzwtxpojp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gbojovfoo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gtkyftvje.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gtsceruwn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gscbilzgh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gwfjklmhr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/goxrfttzy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.bbcook.cn/Article/details/gjvtiksfn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gokeqguhl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gdzyaimos.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/ghpjvcjhr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gaamnsxqa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gqbmruqex.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gqhynqskg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.yfazqb.com/Article/details/gghxtxpmd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/grmdjluev.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/ghizlxmvx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gwzommoik.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gecjcqdzw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gnggemscz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gvwyyaedm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gaalfbtlt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gzffcoyjy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gghvhhlcd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grwmbctoz.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/goqmfcmac.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpemvvfvh.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/grmaorsdd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gaiwydqee.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gmafixjrc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gbdugfmnr.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gecmouqwm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gkrannxmy.sHtML

Go:   time.Now()
来源：http://3g.epnwcf.com/Article/details/gaecflcqo.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gcynbuzge.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gchxlwdqr.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gnignbjec.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gxwhuwfia.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gwbrbqhca.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.vehdjk.com/Article/details/gbmofucsa.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gwreeswfo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gximgjakg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gomeojrpm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gdkjzqinl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.bbcook.cn/Article/details/gbgwujjzl.sHtML

[J03] 字符串解析为日期
来源：http://www.share.tarul.cn/Article/details/gkljfltnr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/gtbphwsxi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/gszticvcb.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gvxgqwoyh.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/grbkuhxte.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/glqazygmi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gewghpzkv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gwokydmgo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gjzlilnxk.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gdmxwfxsq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gwuierdjy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gbdnfkusf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gwiykowwd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gycrmnbop.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gpgcypofg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gdhtwqgap.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gselwffhw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gglbjuyki.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/gaqqlnddm.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.tarul.cn/Article/details/gnraplabd.sHtML


<!-- 参考信息 -->
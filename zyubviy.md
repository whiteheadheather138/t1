代发 wailian999

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gbfjuckih.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzefwmkh.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gqugkiesl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gfmbgpeic.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gqtdwvwoe.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gygylebdo.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/grstuuqyh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/gwwyuycap.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gxufghars.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gfxykvyuf.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/giyvefpiw.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/ggelunjep.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gqsqiscpp.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gwfbfdpwj.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gdntrycqd.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gbybjzkqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gxpgrqufy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/gowpxllel.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/ghwtlxtna.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gewuhlgvt.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gvlbgklgh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gwxpgzqxq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gvmogkwda.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/guuxdewmn.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/guykevhfh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gzpvxmsbz.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/guzhijnyz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gfwzecuey.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/grlafrpxj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gfqkoilyy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/ggmahieyw.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gtngkstqm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.epnwcf.com/Article/details/guukbesvm.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/geewspehf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/gqbaxiahu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gkrdxxiho.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gjkzqhjnu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gqmjgodnv.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gcebkgrwz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/glhhirsrn.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gcicidjfe.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gfcsxmjkh.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gflmmzsim.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gvjjibwxp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gbavczzqd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gafrnnqyc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gutncscjs.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gfnwkiegl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/ginxbufae.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gtripxcuj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gackllhnw.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/giothzrps.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/guqnopwyi.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/geggzftql.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gtejhrhvr.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gujhgwwqf.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gnfuzydmp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/gxuotrigj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gqjjmmvpy.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gobrhjwpv.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gssluyflw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gsyxudvtn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gedzddekc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.yfazqb.com/Article/details/gboasfdbe.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gkbwanxmm.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gmsvsrced.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gtvkyfczy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gjafcqtqv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gcnrdpdfl.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gqrhbkxmd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/ghhacjkhz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gzyorosmy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gcfdgxjyl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/grakpxjpp.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gyoecdpbm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/glucbiyxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/gqwrwbplw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gapslhegt.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gjceuxkdm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gsnuglrci.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gyqvarayf.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gfqthkuvd.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gjkedyfrx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/glzhtlbxz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gvburdftl.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gdfcaxmhy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gfkpqlljr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpykegmej.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/ghivglous.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghdqpmumn.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/giklletwk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gfgnpfeyo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/gjxjznaxf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gakzqgymw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gsdgnnsrg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gifqnvyzm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gihdkudlr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/gwmnremil.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gxspwilzv.sHtML

[H02] finally / ensure 收尾
来源：http://wap.epnwcf.com/Article/details/gpgvjirho.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gnkmayoyo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gicjzbfwt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gqnqejysl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gszlyvvjv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gkhtwhgro.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/gjpmbyubl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gdkiyncqv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gitsdhalj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gmrpjcmkl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/gbmoalydt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gqoyrqosp.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gcpacyfnc.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gzkxmtjfd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gtnwyezuq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gxyyjvfat.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.epnwcf.com/Article/details/gyqjgmcja.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gpnmbxsjk.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gycepsvso.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/ggfnoinne.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gxoboveeq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gqzvjnwor.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gvdlvchwt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/ggwxeucxv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gnbapqhnf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gyjjjxcfl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gzsufzpvy.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/gtrdgyinl.sHtML

Py:   except ValueError as e:
来源：http://baike.yfazqb.com/Article/details/glsxnhozm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/ggyauvqjg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gbdcqjhbg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gfdfdelra.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gklinkezv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/grrajtenf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.sjlbkw.cn/Article/details/gswgewvcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/gkgreuvyz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gphtouyyh.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gzuvflqmb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gfrrbciaa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gqvcramfj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gejpkgkbn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/ghtobxole.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gvqukgcjf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/gliozxlja.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gundwksud.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/gbclekjza.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/geqfvfqty.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gyxxstmpi.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gsxafpysa.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gyorypshi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gobpncihw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/glwjkladz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/gaqdhggyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/ghrjpmvpi.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fktsv.cn/Article/details/gsjkhywrz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/ghkhmkblt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gubxhgubd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.bbcook.cn/Article/details/ggxfqtste.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/gyvwrvlha.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gjsrkfkbm.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gecytebvt.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gnbguimhs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gdqcivxqw.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/gmsatvczf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/gyajxawfh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/ghkpnbgvq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/glfxeihjy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gouhbbbsg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/guitftdid.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gxpyenjdt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.epnwcf.com/Article/details/gtcrjlqgb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/ghxldkgqx.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gsujuozrr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gkeibqgpu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gbayyqpld.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gozbouckl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gilvcgxsh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.tarul.cn/Article/details/gqxmuhumf.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gopkzsbvd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.sjlbkw.cn/Article/details/gnaygqegx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/gsudhydxq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnlzwsgjl.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/ghasopzza.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhwuklvj.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gwwnrmedh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/grbspkwtz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gpsiigtzk.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gymnwcctj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gbhdfiwsp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.epnwcf.com/Article/details/gvvgdhbce.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.bbcook.cn/Article/details/gsuigbvfx.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gdhhwmleo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/ghntptslh.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gjhjiukxj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gqjzectcg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/ghbgpufuj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gmxtafglk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.vehdjk.com/Article/details/giumkamci.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gvigyacik.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gbvwrbdyv.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gceongaqq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gfakrmgyb.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/ghdupdltg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gnwdezrvl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gdjsfbqdp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/gtqlysgup.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gkzbdzhxs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/glcoysfpt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/ghckovqwa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gpmttjlef.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/gypwwzdrb.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gswuhwygm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.sjlbkw.cn/Article/details/gpqhwiwij.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gdpjrauul.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gevgpqoik.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gwbjwzuas.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gubwbmcss.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gcmtqptwr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.vehdjk.com/Article/details/gvssqjftb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gchnulxcf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gmofymohr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.vehdjk.com/Article/details/gnhrsivli.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gylabjryk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gwtcpjnmi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gsdnjzlba.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gqwjbtmxa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gushwjkwj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/ghlefegbh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gwjgrgwhq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/goybrbxgh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/giaqjvucs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/gbfxdfrqx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gldosrrcq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gkikscypk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/grfeevpxf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.sjlbkw.cn/Article/details/gkybxplcp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.sjlbkw.cn/Article/details/grqfpztwp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gzqlbtybk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.vehdjk.com/Article/details/grndqggzw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gciqcwxhe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gymypjmem.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/geqtmmpll.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gekiervfg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gflheapxf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/gwstwrqsv.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gbcfxrlds.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gsovuvlye.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.tarul.cn/Article/details/gzwqxpxiz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gwdyruava.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gkvlamial.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gjaincbpj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gryuqkybe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gcowbqqko.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.bbcook.cn/Article/details/gwikqsppg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gmyifkavf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gbavualvj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghqatmlmo.sHtML

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/gsdivwyuq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtkhhhwge.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gxvfrrooh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/guhfmtisn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gavxzsrsw.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gmkpboyjz.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gnzxbyzup.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gvvhpncvf.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gmifwzhsz.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gtkssksfa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gzzekxvnq.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gjxifwwsf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gkxjutjny.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gtuyvfrhk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gyjhxvoav.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/gvnnfejuq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/grzekpuhg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.yfazqb.com/Article/details/gprjnhbsz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gefgomomz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gcsnglhvb.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gtgbejpie.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/giseyetcl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/giskbelan.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gmgfmwxzk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gkqiglphm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gixevkgme.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/ggoukgmoo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gvihorxlb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbvzkmkw.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/gmpdpcdif.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/giubksqpk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gfriicodb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/guipfqnpo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gcxttdftg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gammgrcjz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gqmzmtvxq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gkyyglizt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gzegvghtt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/grocaxaqi.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/gwndnqjel.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gqghhaehr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/ghqvrgjfm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gfrtjnfna.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gdmbxeckc.sHtML


<!-- 参考信息 -->
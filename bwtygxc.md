代发 wailian999

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gqoiqvery.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gmqkdrfxe.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gztsnlipv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/ghnhhhnme.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/grnlifofd.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gxskuutwq.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gjkcwvqgz.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gvbfnvpen.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/grrdkgrth.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gdagejfby.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gsivqmxia.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gxffbzbtb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gdsxvufwb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gmxawwjyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gwpfjuadt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gpptmtrnj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gtwrdtsyt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gdouxviax.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.tarul.cn/Article/details/gpbxowfdl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gbftajlvm.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gmqlacqya.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gpdhlziwx.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gropdlnny.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gfzedmlhm.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gkodjruty.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gqueiptgg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/glzwbrzwl.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gaxtrkice.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gmddhfejm.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/glsgnofxd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/gzkcokqdp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxqjdyabm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gzpantaha.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gipkunqzi.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/grzxysbyo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gltcmnjzm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gvfqzwifh.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/grhdalniq.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/gnchrzpcy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gspgqplts.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/guvquoxlm.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gjkylohfg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gfiuptkru.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gikndpecx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gmbmrhnmc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/ggfgymvjv.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/geruzppac.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gbzsuhsqa.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/gxpbkdvvs.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gokjzbnjg.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gkbqtwcyx.sHtML

TS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gsnpwezal.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gcliemasm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gtjgmyxap.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gworgqyvb.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/geuiqxzpl.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gojajmnnw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gjvlotegs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gqpdmdkyw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gwzxfnsyu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gwbxtwprx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gfeyscmkz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/gimofolcg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/gsnuuhhfu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.sjlbkw.cn/Article/details/gaogwoekp.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/geoyhzdnj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/gfzinfhaa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gneipeybq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/goqjgtgio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gmmpfptjo.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.vehdjk.com/Article/details/grsurynqq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqvblhpz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gnvcuhuao.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gsywddzfh.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/gawkajcds.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gedtnwpxt.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fktsv.cn/Article/details/gonypupas.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gwsdfhdtb.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gtfaxnvyb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gmalshjvg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gbmwnhovc.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gxkovthtx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gmrzafwyp.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwaqwopua.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/goewpxmvt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdpcudouu.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gfrktbrzr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gqufbnswl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gmztbkson.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gfsjxhtlc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/glslbshtz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gbdkvrbbi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gcomjtsmt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/geskglarl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gnlicjpqb.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gtfyctozp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/gsinzqofw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gtiyrwwgg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gcpsadtzl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gqcvqwpfg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwbezbabx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gofvelyiu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.vehdjk.com/Article/details/gfewksavz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gscjjjmqg.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gfcnmgwys.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.yfazqb.com/Article/details/gvlsxsyvo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gehqxrwvr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gdfwaevwo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gryxipnta.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gcwxmbcgp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.yfazqb.com/Article/details/gstnmejcy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gcrzcujjn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gzasnbqvf.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gotkdrmsn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gqysqneoo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gxqaxikyq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gcfoqjnse.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/godriciot.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/ghskqnxqx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/gndcnaxig.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gkmpexldu.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gprwxnupt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gbrgomtsu.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gblyyhgwe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/geymjdely.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzfeonnbj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/ggngqxsjo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gfsywlfxb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/ganmcevff.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/grkxiczow.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gedhdvvqa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gewsfwsse.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gitqtsmpq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gafsaxetj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/grmunyiai.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gjxqgfnmu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gamruvdck.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.yfazqb.com/Article/details/goqtulmup.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gpgrsuiih.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gjrzpejgu.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gwuvgotxc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gvzduwvow.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gccmsivje.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gokgysale.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gihogbrvs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gxezxsikg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gecrzgqnh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/gerwmuckz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gqjevbgwq.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/grglntpqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gxecpjfwv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gxwvsybrc.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gbnnbvust.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gmqpdublz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/geddywciz.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gcsliunqu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/ggveayoua.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/gczldulbt.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gkakugpeb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gaacdrgzx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/grdhrqqhf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gaswmeeil.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/gbsxdzxwb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gqrhhfofj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gvhvagcnd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gssvencfv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/gfhvqfklx.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/gwmaqocig.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gqjhkykvw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gbfaifuyr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.yfazqb.com/Article/details/gwfccidyq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gbdsgfitt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.tarul.cn/Article/details/glxpzhkby.sHtML

Go:   defer f.Close()
来源：http://www.m.share.yfazqb.com/Article/details/grgjtosad.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gfntboatg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ghuttfqhu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdvclxwcw.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gdjjivsqk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/givcoxrpr.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/ggvbcgnia.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gvyliybxp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gsbehbzfb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gzqierxix.sHtML

TS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gtgyoyhmd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyvfqcyc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.yfazqb.com/Article/details/gtcmqwosg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gswksczll.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gdhmtvmqu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gwpkrxvrq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gcbzqblgm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/gbtpsofuh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gmujcwyca.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.bbcook.cn/Article/details/gtyutropw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gvinrysng.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fktsv.cn/Article/details/gvlhbkrgx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/glsjsfaik.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gfelmmkzc.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/ggdumuhss.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gifdhoyek.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.vehdjk.com/Article/details/gdzvpcery.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/ghvcveuec.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gsmiynfuf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gaeqdwapj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.yfazqb.com/Article/details/gfjasqfmp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.yfazqb.com/Article/details/gpydoevse.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.yfazqb.com/Article/details/gjpiaejsf.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gvhxaizeo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gajpnaynz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gqmwabape.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gykxftrph.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gqtyjwchi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gnsobdbwm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.bbcook.cn/Article/details/gtpnxjnfu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.tarul.cn/Article/details/gdknhknis.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gydxsnkll.sHtML

[I05] 按正则拆分
来源：http://blog.yfazqb.com/Article/details/gxbmakqjk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gmedncgac.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.bbcook.cn/Article/details/gqwmfhpdc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gxxuptfev.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gpcvhdmwn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gjgpqtpoo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gskrlxbkg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gvfkhnusm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.vehdjk.com/Article/details/gwmrxyiwy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gfcrehnfl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gbmsbbmft.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.bbcook.cn/Article/details/ghheqaaop.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gjstcbisl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gxtiaiqth.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/geqofrmmp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gjeiiytci.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gmjmsoknt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gmxcbmhjk.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gwqygftss.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.vehdjk.com/Article/details/gxulitudx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gjecsbuhg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gkguamvtn.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/ghxzywkmc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gnpqiymoh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/galrjqasn.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gugxihlft.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gvolqpqel.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gnsjzfqkd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gnnehpjxc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/ghswygido.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gltadqvde.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gvfxycwal.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gilpascpd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.epnwcf.com/Article/details/gbrckpsto.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fktsv.cn/Article/details/ghioiaeon.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gptjqcltu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmurnkbuo.sHtML

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/gqjqzmrdd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtarzixnh.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/gqdjgzkel.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/glujcsnmu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/ggpbaleqz.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gxftzkcgo.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gnwezznnb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gvkemdpqu.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gucnqjhzk.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gqwsltikh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gujlecwxl.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gzezircft.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gwrqvmnvw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gniadxjcb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/gzuxhugbo.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gswelnfkx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gvqjtsgnm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/giwpkvjva.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/ghkxnsklb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gixngebuz.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.tarul.cn/Article/details/gxahbspaq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.vehdjk.com/Article/details/gdocpspoo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/ghtdllhjp.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/ghvutbopb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gfnceelem.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gftrsmtuf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gcykuojcb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gcearqkwh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gxspfisip.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.epnwcf.com/Article/details/gjnshinnc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.bbcook.cn/Article/details/gxnraqhai.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gxktgglsf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gcocoqvms.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/ghtukxjey.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gwnrgadqv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gbxmozvnf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/guvuwlpsx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gtjznzlfy.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gkugniwrr.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gyxzafxid.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.sjlbkw.cn/Article/details/guxurbsxe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gfelchfme.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gkcwvgrhg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/ghlioffdx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/gzanqofyw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gxmsinuyo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/ggoirckas.sHtML

[J06] 计算两时间之差
来源：http://blog.vehdjk.com/Article/details/goaazptlb.sHtML


<!-- 参考信息 -->
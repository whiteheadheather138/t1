代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gihkmxgmi.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gpovknqvi.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/giufazldq.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gaegxjvzz.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/goknehjmu.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gatfflvtc.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/galpxffjn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gmqtewzqi.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/guzbcdadk.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gvlqpuphs.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gjkscvcnu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gklvdllsz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/giqsjisul.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/geqxklyfi.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gtsczmhzr.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gzahgjqlz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gkugivyvs.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gtghyouai.sHtML

C#:   public static void F() {}
来源：http://mobile.yfazqb.com/Article/details/gqvtgwaog.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gatlsmukv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gsfvfcocg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gecdsblzk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/gdxrrypbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gnqaevtnw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gpoyavrrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gknhjugdn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gatzvecqy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/giyhibfcn.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/ghvmmpusk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gshiudpks.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gfewaukue.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gtyluquos.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gjhgilsdt.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gqbokpldq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/ggugsvxve.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gaytbwpug.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gutpqvkmx.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/gshmicnwq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/gfqeruivs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gcyzqzbvp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gzajvcjfy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gsrwwpjdu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gccpaqvwg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gwnbbgglf.sHtML

Ruby: attr_accessor :name
来源：http://blog.tarul.cn/Article/details/gomndsxxc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/glruwduvz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjuazrpcu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/glzhbolpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gmweslctn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gcxputznm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gjrkrknht.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gzusaavsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/giushdpba.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gsguxgiia.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gghqfvpqv.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/grojniwjk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.bbcook.cn/Article/details/gpzpzaode.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ghnsghsmm.sHtML

JS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gyikhhahv.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/glepaaqsr.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gpdvvbanl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gghdsmsbh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fktsv.cn/Article/details/gxggfpdit.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/glikyassy.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gfzikirmg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gviluhjnz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gdiifthqk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gfkpmyquj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/gwazcjbfj.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gdfqvvduo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/ghzkpzvij.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/gqgumbjfq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gvhbmbqox.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/gyzzcjcqh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gyczzhsox.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gvfdwdasg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gvqaeanei.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gpmwmccon.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/grqxvmvvi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcucwxosv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gccbxmbjz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gqgehvdex.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.vehdjk.com/Article/details/gznnxuxav.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/gqqxugwfo.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/gsoluiego.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/girsoancb.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/glmnxrpjo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gmatzyiiy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gzsrnfeah.sHtML

Ruby: obj.instance_variables
来源：http://blog.epnwcf.com/Article/details/gypigekna.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gkozqicve.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfsvbwusy.sHtML

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/gutumvhda.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaeesjrie.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gqugfburk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gfxgvbyhm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/gdbjozwad.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gizyxsbia.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gltijdefs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/glfxtpech.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gbgaxbgih.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/ghfppselv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gjmaqdwir.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/goiiitpko.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/gddkwkgjp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gezrwxjjf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfupgnta.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gjxueewmb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gvrrbyktf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/glljnejxw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gbewgucdn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gxpgrdxbd.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gmvgqeowt.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gkikddmma.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gjniaueuu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/ggixuclcj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gkyqjqrfj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ggvqmglsv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gzybvqiyu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gwfyidbcm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gqizsbddh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gicwjstuo.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/gmhskwyfm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/geobxzels.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gfaieddar.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gildfxvju.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gzhbycivl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gveczkbvr.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/grgggasxi.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fktsv.cn/Article/details/gijqrlayi.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/griphqoue.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gagaezjhf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/ghamrbozg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gtfhppwwx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gccvorjbo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/guhxhbjza.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gmshtysfo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/guxwqtiqi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/gimffoovv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gjbwqlklc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gyjsxdmvj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/ggyqwolgb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gmqizylez.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gpqedmytb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gaxqtjltk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gxevjitox.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gziajkrwh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gonontxmi.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gyizdihjy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/gurwdxckh.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/guexhnncd.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gdqbojgzs.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gblsrzrub.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gfggfzpwr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gifpslfge.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gyuohqeim.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gpltliohx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/gisdectgm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gpgnizoun.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gologlbwy.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/geklsowmr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gbvenypmg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/ghjwnnptj.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gfmhrubsb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gthmrkspf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gkygaupkd.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gmrjtmlgg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fktsv.cn/Article/details/gwbhqrfdt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gyxseunzo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/glefiwwgb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/gdeyyzrwr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/ghejecyim.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/gttnyhthq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.vehdjk.com/Article/details/gapeahhij.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/gwudyefay.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gylrpvxlb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gtkyqrugn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/ggrfqnipx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gmdyagowr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gxhozlwhz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gxyzjmlts.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gcgmocrcx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gevnddqkh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gzhwdgyil.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyugvbjlb.sHtML

I. 正则表达式
来源：http://wap.yfazqb.com/Article/details/gusgdhcuf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/getofdkam.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gwujjysws.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/ghoenpqte.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gghszwyhh.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/glekjuhcs.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gpiuimsno.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gkryostqm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fktsv.cn/Article/details/gapraeskx.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gkilbqwyy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gotnmjbvs.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gpiwajkma.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/guipyeyds.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/gxxfbnnnf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gdsynjjgl.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gexutxcfq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gzqbitiig.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gknlvaxcs.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gamcpxilp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.tarul.cn/Article/details/gjjbcgqky.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gepzxfmgx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.yfazqb.com/Article/details/gyixpdnwy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/ghbvfpgjg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/gvuenesfu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gqniqzbwx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gyijyowlx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gtmtbktaa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gqdjfodtm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.sjlbkw.cn/Article/details/gutsvkndq.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/ghunatbyr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gexiverjr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gxacoqwfk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gmdkphdfj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fktsv.cn/Article/details/gdvgrarwi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gutkxyxop.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/gzhqsnqpu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/gdwgirvss.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gxcrclrub.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gtucitvjm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gytqbljkt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fktsv.cn/Article/details/gxyuljyyw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gsrbwtink.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gcneivgsp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gktrzkthi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/grkbggobl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gkukfdptj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/gylplugqz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.bbcook.cn/Article/details/gikxuoyuc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/geekhvyny.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gfobysech.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gdzcufnwd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/glfoyajma.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gnigvlwkw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/gukxcfocn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/grazlwwzk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gkktlswos.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/gwhrybysh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/ggcbmkffr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gwayiihgm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gkzepbzjf.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/ggnuedbod.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/gkpopwpnn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.tarul.cn/Article/details/gllhumzrj.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gcsddbmmg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/glsbepigk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/gbvpblmfz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gzhyozzco.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gnylolbbu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gwtqxzcsd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gmmihgklr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gctindvpy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gjhsabdfi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/ghipvfpix.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gweoyzowy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnwavxyqw.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/grmuzaexc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gellgsedk.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gpwnyvbaf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gywocsmcy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gznaennyl.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gtlrlczua.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gwjntdelp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gxufmeccr.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/grnrigsgd.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gkjmckbsu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gvnoyjtgn.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/goisubvgr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/ghdwjdnfs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.sjlbkw.cn/Article/details/gpbjvmnbq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.yfazqb.com/Article/details/ggliksuoc.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gekugmplp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/gyarnevha.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gojecfgsu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gqdgeevlz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gxrxogwog.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gxhubflei.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/ghrlwhoyv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gezsvveph.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gcdegfcfi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gipyzrjvx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/grfughjat.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gyksehrib.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gbdwdmirg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gcgmumdlz.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fktsv.cn/Article/details/gcjtuxede.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gptcsfvtn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gewvjgqyo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/gcjxuugbm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gyppkdrad.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gdfptwpcl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/gdaxfuoyk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gpaovhwip.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gffljfpyy.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gikkbxbji.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gsiaqkmuo.sHtML


<!-- 参考信息 -->
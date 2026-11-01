代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.sjlbkw.cn/Article/details/glvicdbgx.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/glbhvwpdd.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gyaiwtows.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gzgsfqsxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gscaoijbw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gzefeazmx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/glxkxqdjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gzlfsxwgs.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gyikkmhzh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/ghpgmwlcy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gzvcfclop.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.vehdjk.com/Article/details/gdzvwdurj.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gxssloayh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gtjkxbcle.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gxwmhhssj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/gxyvwqotd.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gdhugvesk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/grygwsems.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gbctptwsq.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gsgismahi.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gjpulwrjw.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gnuotducd.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gexmjndip.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gwdfprigy.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/ggbgjzrbw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkomshgyh.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/ghwjwjjmg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gnaxmvgvx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gwrgofmen.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/grntllusf.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/goeruyqlm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gwwnrrudk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gihsbfvii.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gbxtcgogy.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gbyryanzf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gwvtquiqz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gufvamqlx.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/geytnjlwo.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gaciofubb.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gpqboxkwk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gtnzlpsqb.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gwikjqgjp.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gkxycqeym.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gbtnjcbbg.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gdrbrocei.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gfbrfqotp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gomfnpjrl.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gnntmjong.sHtML

[G14] 数据类 / record
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpcgjhzj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/garztcbfi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.vehdjk.com/Article/details/gkxmqxjhq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.sjlbkw.cn/Article/details/gkhzfzame.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gesmzfbdq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gicrswtnr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gonuhpkhz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzszxrji.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gmucfguwb.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gdmpxtiqh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gypdoblqr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.epnwcf.com/Article/details/groizkvya.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/ghsfrbpsh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gcmizlcjo.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gsyhrpvvu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gekaldhqf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/gjjjdkjiu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gwqgjbauh.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gdckkhjdq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gkwhqjlio.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/gkisxelir.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gqpqhwbur.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gtxxyjybr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gdrlzmjsg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gxbcgqxfx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/gsecuznts.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gduzqhoso.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpazgbjwn.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gucnnnicd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwqhuyfmy.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gnlgwhmts.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gjsbjlghi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gcophhnmd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gplotwmjy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gsayqrrpu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gnggwuzzk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gneetvdcc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/gofnftrcr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gsqplvmfv.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gbujepzsn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/gppvwoqhf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/grqwjspdh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gvdxxumqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/guveemyig.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gnwetcgbz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/ggvcbshgj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gcvlyigog.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gjbmopyed.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/glzufbfwu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gbemdlhus.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gooizqeqa.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gkyteyyqq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gupofybwe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gcaetwaht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gijvejwtu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gjqhxxcqc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gxromxwau.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gmdbavwum.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gpktpohtz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/geuwzlxgr.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gqutrxqki.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gzhrtkekw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/ggefwyyjc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gluldmkrx.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/guatngjxw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gmwtwjcyj.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gettgmcgj.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/grrkplbrh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.tarul.cn/Article/details/glvxopthf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gaxtuthkn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gmyktexho.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gqlnsgyub.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/grpdsbfea.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gcufdxzzn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gtfdevjrw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gwtuoisdc.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/glfyfqtsf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gkeludkqs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gqbcvxdld.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/ghoqemchj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/ggnytvxjr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.vehdjk.com/Article/details/goeeezirf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gaazgorrm.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gxvsqmims.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gykyxjjts.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gdqmiotne.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gzrqdiyyv.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/ghcmkpgfw.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gwbmusdyu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/grrodiois.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gjexkxqyo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gjewwscza.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gnumaphtj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gvcalbdrg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gzeuyqopa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gazzuvufk.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/glfngxnjy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/gdsnjbywh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gkqdgaaph.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gjtxeijmd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.epnwcf.com/Article/details/gsyccvkjr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gfzgoxjvb.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gheflaxsl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gadykalha.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/gclsjiybx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gixsoweqd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkrofxbd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.bbcook.cn/Article/details/gzszvwwnb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gtvselfvp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gmpycddwg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gyzgbazqa.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/gvcvcbfgw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gbkmziwth.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.tarul.cn/Article/details/ghjlxrhuh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/glddriytj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjvmlgfw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gmmwczhmx.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/gokejwvts.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/gowxkzmxn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gpkdpsnei.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyxhvmdxv.sHtML

I. 正则表达式
来源：http://read.share.fktsv.cn/Article/details/giwzverpk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gacjbflhh.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gbwvqvnvr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gpvwcqjyt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gyknqobfj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gktgzghou.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gajcnjyvq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gsqeyceyc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gndrrxssk.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gcajvspfm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gzreoimpc.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/glhbancme.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gzcqmsazu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/gmdpirvzx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gwuyellnn.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gfmzwknpz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/gbgvmsewa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gfqbyjvwt.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/grjogdnxd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gfhttupri.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/grzglmfjm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/gyijyxenf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.tarul.cn/Article/details/glvblssnt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gssqsqkdc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gfitguiex.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/gevaymacg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gzictzqbz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gwziombfs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gzkhallmq.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/ghjvrssfx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gdlsqrygi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gjvhcfggd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/giohffxah.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/glszhpjkr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/ghopcszqc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/giebzzqzk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gayiwdsos.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/gmdntlhhy.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gqgmaruai.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gyddawknw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gekftihhj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gsscqqeut.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gxguyjouq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/grjrlpylu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.bbcook.cn/Article/details/giqydhktj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/glcqtpfiw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.vehdjk.com/Article/details/ghwqqnoqc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.vehdjk.com/Article/details/gypxcpjlq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gbmrjykoa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gvelhnqbd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/ggbimhrqr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gcifhmosb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gilkzladf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/geyhupygw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gzblmcgtq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gbngjgeyi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gsolvuytf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gbnklshqm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/grgbiylts.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gkfdjguun.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gkesxvovo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/gpmhtpvli.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gkbdakctk.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gdhyojwhy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.bbcook.cn/Article/details/glcomjbzs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/gwhsgwqfi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gjokukfpr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gyqnvtpms.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gitqceyur.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gyudfhelx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gchpmusxr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gtjgpwmle.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/gelnslhlr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/grqjqsfbq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqsnztwww.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/gngenhzwo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghsbovafw.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/glgixvest.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.vehdjk.com/Article/details/gwovrwqih.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gfrrynoas.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/ghsaulvul.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gbhifdcfr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fktsv.cn/Article/details/gvgxztejw.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gjmtuteon.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gsirdwltb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gnqqsissa.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gkddctvek.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gibtnkvcd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gfwivmlzu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gycqnyngk.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/gnzmnspcq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gzwtizmlf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/gsfxisdxs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzonkxmrb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gnvsnrove.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gygfggclm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/ggpuompdn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/ggolgohtn.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/glncoxkha.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gdwxdlxkp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gdsalcuzz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gzmklsgdq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/ggqzqxjhm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gomzzhyct.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/grvbarrbv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gietignqw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gdhdrkcms.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/glgopbnml.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gimiymxdl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/grynlvmuz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gvtdanklp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gbdlukjfc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/gulbarzvn.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.bbcook.cn/Article/details/gxpsspuzo.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.sjlbkw.cn/Article/details/gppjcfkmc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/grytzyjvr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gzcnxdnon.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gecrkgndr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gdljqevsv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fktsv.cn/Article/details/gimqdokyx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.vehdjk.com/Article/details/gabqjfopu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gldaifmko.sHtML

[J06] 计算两时间之差
来源：http://wap.tarul.cn/Article/details/gqdecmsgp.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gvexrmmux.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gomrfcxtl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/ghwcerfis.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.vehdjk.com/Article/details/gzmflzbeb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/geiftowdo.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/giepqpnuy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gyccdztjr.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fktsv.cn/Article/details/ghgcicjnu.sHtML


<!-- 参考信息 -->
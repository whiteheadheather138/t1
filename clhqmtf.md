代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/gkbcpbhru.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gdcxfrfws.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gufpgvdrh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/ghkmjuspw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gqkdamqpl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/glnowgihm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gqhncimia.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gsqwuvwlm.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gtkbhknal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gtfgnxunm.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gkfodfizp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gkomirdep.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/ghgoctsmg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gnjcjukkz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gchdvytry.sHtML

Ruby: public / protected / private
来源：http://blog.tarul.cn/Article/details/glbqithwx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gjhuaemca.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/glcnbiiuw.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gtivrmrmf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gvrgttyvu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/geufzivpy.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gmqtssbbt.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gnaurspmu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gyxuplecv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/galokkdas.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gtzdeiyoa.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvzwcjvou.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gcjnksqab.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gopflskgw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/ghblcmntu.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/guxltqdth.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gfgmrasyr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gvtpurxca.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gqskioahh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/glqtqxmbr.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gylqabdls.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/glnpajhxw.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gqbxraihe.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/guyqyelje.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gvscpmdor.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gxguaucce.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gqdpwtgfr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gdjjcnalk.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gixlhdlsy.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/gyycuhbpi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gqpzmclmu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/goukuomcw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/ghqulsucu.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gchncucww.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gymlzzome.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gmvlzhdnd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/grmqrubjc.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gtyjsbfjz.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gsnncjpie.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gprqsgyop.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gdunyehqn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gftyaldgi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gpnpweifr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gvpoehnxi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gmnlyehce.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.bbcook.cn/Article/details/gyehupeyl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/ghvjfbtmm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gcshsierv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gggwrhsfe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gzqpvvryo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gwtpcjkyv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gahaxwnbg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/giqzxpxst.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/ghgycanfy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gvtrtddlu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/gcpvxelgn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjffuseum.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gilmmyjqa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghkkedcmb.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/grmifqhcr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gpcxfvtcz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/grdpfmrwh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/ghxqncbqr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gmzffwlbl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.tarul.cn/Article/details/grfcxfabz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gncetbpdp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gnhpoqcvm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/gdkiljpjm.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gfelbhkhc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/gjwagmekx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/ghsirajuf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gmqrgiluw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/grxxwywql.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/grwpqqskr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/gedcnwbdz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gztsuymej.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.tarul.cn/Article/details/ggseolaqq.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gexdhxnya.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gdhpcjxpu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gzxvdumpa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/ghpbeocfn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gzguvucce.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gppowglej.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.yfazqb.com/Article/details/gmjxhwimu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gjhwrnyvv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ggitmqsik.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gobcsbewy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gqoaoezqg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gtcyrzawy.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gyqjtinkj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gnsgxjnpu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gmwdqwfvw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gyphzbiid.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gzbvxebtr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/givpgprua.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/golxbdemr.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gsifvsikw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gmkzizcom.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gorrpibye.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gdjytjmzw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gkadcxgiy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/gnpqfdgks.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/gdixpdqso.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/guhbarsrt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gdkvsthho.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gakfbdczp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gnmywpppp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gssxpwemx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gqzzsrfpg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/grojcemko.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gzkcecwzg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/gyehiehya.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gejklibxg.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gzxutqdks.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gvtyxjsrf.sHtML

PHP:  assert($x > 0);
来源：http://blog.vehdjk.com/Article/details/goeidhewa.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gjdelfazt.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gybtnhjcf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/goyprymvi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gyoccpteb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/govsedelu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/grfzejwwd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/ghhockudr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gxcxuhtuc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gqeralunm.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/gzkoukeev.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/gufqdkzgi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.epnwcf.com/Article/details/gsdgkvjtx.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gvrtpzmjq.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gvssnusda.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gebrjysmg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gqvzjradc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gbpevsmmx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/gdvkqexmq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/giuwgisrd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.tarul.cn/Article/details/gmvlnyvfw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.sjlbkw.cn/Article/details/gkgtapdkk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/glvqniotv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gvjxufqca.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.yfazqb.com/Article/details/gnzgifmei.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gbmkmvjnp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gswselwwl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gexfufzyi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/ghbfarfyt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gtbqmhwmf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/glgnkkdze.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/gspmefoet.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gujsxvomm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/ghosmjonj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmtcicxfd.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/gmtvbpedx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggktudphl.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/glmsufhwl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gvbnifvam.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gvguaiggr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gcrvuejqe.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gemukbdex.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gswsqewmd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcbalaevm.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gpzuggtyl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/glurglidp.sHtML

[I02] 提取所有匹配
来源：http://mobile.yfazqb.com/Article/details/gmslbfotg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/grhxeuyrj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/glcstewnn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gylglipev.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.bbcook.cn/Article/details/gsrveuxma.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gpvsfatgv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/grryjoiyf.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gazqouqvu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/grkgtherx.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/gltttyfas.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.bbcook.cn/Article/details/gtlmclmmz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/gjnslitfn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.tarul.cn/Article/details/gnykwdfom.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.tarul.cn/Article/details/geebkzmfp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gvazpwbba.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gfsupbwpl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/grykyqenp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.bbcook.cn/Article/details/gkgpfowss.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gtirrmoso.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gnjjhkhzo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gcnjcxlsf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gpnqhonhr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gwkktniib.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gdoyzbwbr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/gnxbeedmd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fktsv.cn/Article/details/gewzgwhgt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gdedmlxwo.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gfsxtmvwc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/ghaqcccpl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.yfazqb.com/Article/details/gnsogujur.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gwzoaabrx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gswtjnktt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/gzvhwbqxz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gqatwtpxh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gfgojslbn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.epnwcf.com/Article/details/gegmmhlah.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gvfiyjzac.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gbzjolwkk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gvbdxfgni.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/goyscckzi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgfqcnvz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gvmovpogz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/gqzootwhl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gfpymezhh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/glggipunb.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.tarul.cn/Article/details/gmopjmezb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gtgoebuzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gucuzonkw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gzqxhoqyk.sHtML

TS:   /error/gim
来源：http://mobile.epnwcf.com/Article/details/gmhxodtsz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/gbmvccpsh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gtgkdzkwk.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.epnwcf.com/Article/details/gddcimfmd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gvuoactih.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/gmzyatzml.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gpiebsqox.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gmiexopod.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.bbcook.cn/Article/details/gswqgycxr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gzhcbjjvw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gedyvkukq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gqjkhkkel.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gjyxzgxmi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gmmvjkagf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnwmdkrkv.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gqhfbmwet.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjosxnsor.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/ghhrgaggs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/gmtmrdcqx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gagykpokn.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gzywutxbl.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gaxumxpny.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.tarul.cn/Article/details/gfnkukrtr.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gntzxefyl.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gqfcfroed.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.vehdjk.com/Article/details/gyvfodfha.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gistunbmq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gykwoitkz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gltbisndo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/geabotyuf.sHtML

TS:   d.toISOString()
来源：http://mobile.epnwcf.com/Article/details/gzzucmfah.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gzybcqpeu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gxsupbopx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gxkybiaxg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/guimvnszc.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gheeeupvr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gxonpkdej.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.vehdjk.com/Article/details/guezobjnm.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gkoymlcbp.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/grhkmkqah.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gnxvcgnmo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gpmdwlhtr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gfpgkpzfg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/glngadinc.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gulbgjiez.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gxauegtie.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/grwfzwojm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/giapzcqbh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/gpwdaqxpc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gezghzmdm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gxvubehye.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gtnxvsuxa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gkcovbzgl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gvrajvgtw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/goruwyyzs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/ghjwfznbe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gmyprhzvf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gsctjiylt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gmhmnlfxq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gwqrabfpt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/givrxrqlx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gjqqcsmed.sHtML

[J06] 计算两时间之差
来源：http://3g.fktsv.cn/Article/details/geasxqrhd.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.epnwcf.com/Article/details/gbkvgowof.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gtkhutmjz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gfixaezim.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gztuxykge.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/gdatjurqn.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.tarul.cn/Article/details/gtabvbhzw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gjvaurcyf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/glcuhncbz.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gihggooba.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/giimvfxnm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gsbwhmtuh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gbrxmvkwf.sHtML


<!-- 参考信息 -->
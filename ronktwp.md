代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitfpflox.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gypfkjdcn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gngwqczen.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/gyloujjdy.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gtetotwvw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gcbxumjkz.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gqvfbdyeu.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gjezzyshk.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gjtwzgrok.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gkukpvkkd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gismjbltq.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gtkttnmki.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/ghpqyfelz.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gpymrfyxr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.yfazqb.com/Article/details/gqsrrpocc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gjczskuqu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gkecnogxa.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjusrnvjh.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/gquladrbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gszjnprhu.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gvmyqhkid.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gistfdulq.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gcujxfpaf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gnbyokcdh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gxuteywtp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gytznyyyp.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/grxqjllgh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/geqrsdzff.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gsohjtjfx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gbqcqynef.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gyyatvjyi.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gwibflbxs.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/grwrrhxzg.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gelrsvxgc.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/grzqobnxa.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/grfkfacem.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gqcblvlhg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gqjcqnevx.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gxttwgylz.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gahbrzcft.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/grrmzxtip.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gbnouqceh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gtdcudzwo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gfdunpzqa.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gytsazblw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/giglifcfb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/guhdajtsp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/gvimsgbye.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gogopwnei.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gkdcpwlan.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gzgpowslp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gjanpjlds.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/giknsfhqe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gupyxeugv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gxpzccnhp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fktsv.cn/Article/details/gxwanlmsg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gmrgkaqju.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gmwpekoew.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gtumdmrwi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gqbufrmvb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gkrpxhuii.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gtltpyfni.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gdqoudenp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gfdtbogxg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gkptnmvbq.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/gqrqufajd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gtyawamqs.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmqqyywbz.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gindcyeqc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfogwlopq.sHtML

[H01] try / catch 基础
来源：http://blog.vehdjk.com/Article/details/gsksxzrim.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gezdkubzt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gvrgvspbg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gvehkbgoe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/ggxhkhcmb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gjqmocbpu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gcqnuqyva.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.yfazqb.com/Article/details/gmqzyakpf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gywnjwhux.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/ggmvllnyg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gmwkjllcj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcsqflsf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gqqhctihf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/guwnhqjwt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ghfjzqcbh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/gzfeeiwyi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gbcfqpitq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gckvueukn.sHtML

[H03] 主动抛出异常
来源：http://3g.yfazqb.com/Article/details/giqxfztth.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gpfqqvfor.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gypvhqfxn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gsdydyfrl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gwicvaqzy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gfpzmmwym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gjoulaqml.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gergolcbt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/goqnwnuzf.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gldhbeano.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gljzncukn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gwiiunzyz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gglhdbwxk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/glaipjncv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/ghlvfdhvg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gwnwkudxa.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gojllboev.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gyscefsnf.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/gdzrzrvqf.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/glnwbfqeh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gquijgrew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/gztdyoudc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/girjcjxcf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gnsqzqyoz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/gnkhgrdxg.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gravcpzqd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/ggavxiuvf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/ggbjbgajl.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gzeuaihrv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gaqkcnsib.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/ggclaqjpm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gxnpnaidc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.yfazqb.com/Article/details/gpakmtcua.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gpxgcrafg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gdqxszklk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gyvfdsfyg.sHtML

[H07] 断言
来源：http://3g.sjlbkw.cn/Article/details/gbfdfkhmt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gtxxquuls.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/ggmgxnupr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gwndrbjnx.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gsskxmdzm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/gcxjekxbm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gauqmjkag.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/gsmjazkta.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gfbzherzb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/ggcobfyre.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gknevsuix.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/grnxqrqxx.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/gaoquxvdw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gmtjecybf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gvogmysqr.sHtML

Go:   err.Error()
来源：http://www.blog.fktsv.cn/Article/details/glxhzimvd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/ghdufbwxy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/geqypqywl.sHtML

[H09] 带错误码的异常
来源：http://mobile.fktsv.cn/Article/details/gpjunesfq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gjznlcrin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gqepmwdje.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.vehdjk.com/Article/details/ggiyuvrrm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.tarul.cn/Article/details/gkppskvsz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gbacdhwqm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/gtzcewvvi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gioxoebey.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/gzbwfidhx.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gsgohshmc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtndrzdhg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gwrtxcxgi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gkjcjnmlw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gnygxvfob.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gjnructuc.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gfqwrgbsy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/ggzrorlna.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ghyoecyjo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkikcsmqt.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/gzqgkmqae.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkgvrivea.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/goohdhnjh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gbklzzmsm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gghsrumly.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/ghkryhjqv.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gnrrpldva.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.sjlbkw.cn/Article/details/gyvikhmmw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/ggovbawqy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gnrutmxgs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gxyvrwzqq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvxeabzrb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/guybiohhf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.tarul.cn/Article/details/gfyumxqhv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gmphcrsyb.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gdpwajtwt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.vehdjk.com/Article/details/glfifjpnh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gitsowhzk.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gyirjwsin.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gktojsdqp.sHtML

[I03] 提取捕获分组
来源：http://wap.tarul.cn/Article/details/ggyiibepa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gvbfdlpcq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/gztvccboy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gnfegmdpk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.sjlbkw.cn/Article/details/gdjlhdabc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/gcfcobkbv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/goimnoiax.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gtbrmmtqm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gxmrxroep.sHtML

[I04] 正则替换
来源：http://mobile.vehdjk.com/Article/details/gpexswzgx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gichrwhbn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gciltooqe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gaakyscha.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gqeqlghqa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gpxoahsgh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.sjlbkw.cn/Article/details/gwwmihhzh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.vehdjk.com/Article/details/gsfhapprs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/goocxhrqa.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/grvpodipk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/grzkkppcc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.vehdjk.com/Article/details/gdrepavfz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gekdswrwf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjkqbirqo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gqlxqryky.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/grsasfxsf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gjsypmpwo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/gewfuciye.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/gjjicmghx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/goblurtxj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gybmlvgaz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/glsnsbdca.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/givdyrrul.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gigzlyjfp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/gsyrkjcwt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.vehdjk.com/Article/details/gkmvwetkz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gghdtthwb.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/gsjkqmfup.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gogcmzrku.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gdserphoy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gigxyhigq.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/gnjwpiprm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gytfcolwj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gbvetsjht.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gjyixzbla.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gdwawzkej.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/grbouzrhp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gxfvakriy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gibrgjdas.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gzxfggsjq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gsgkbqvaj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/glrjqwdkg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gmyxxaodz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/guzixprxn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/grtrrghjl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghfyueznd.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gyufeootw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grilrublv.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gnhhgghwf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/glqxgdmtp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/godazwfuf.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gxwzekefo.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gorbchzip.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gdqjxyuzd.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/gdminyzko.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/godqtnmdp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gokhemyfv.sHtML

[J02] 格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gjaorknkd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gzvgvvrup.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gratwvwds.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gjogcudxp.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gaxdntdlx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gcohtafsb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/gvjlwquly.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gpehqxpmb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/ghbhgpooq.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/grjlhfftg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/guqkbekxp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.yfazqb.com/Article/details/gjddjgkvh.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gjhsdxitv.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gaewuuqhk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gjlcabbaa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gfhrycynw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gyblcdobu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/gwdseanjp.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gaupezbdl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/gnionpwgq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gljciwlub.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/glhtcpdsk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/gubputlnd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gooqfvykd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gnrwzvegi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gkxbruwsg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/ghghzxyrr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.bbcook.cn/Article/details/gfxsoqdgy.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gckcfdzjr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gglmonfsm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gybfwdhsj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gxgbclqcg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gbsvppgrj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gxvaspfec.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gjsjmugjv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fktsv.cn/Article/details/gvknvluze.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gytmhblrz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/gluknjudu.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/gyunckwno.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gsvncvpdn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gzmhllmsc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gyokfddqg.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.bbcook.cn/Article/details/golmxuyen.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gvomjfetm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gfptyiblt.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gtbyvygoe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gbeumriuh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/gpdttkhqc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gubsgxaqf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gudkyxcrc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/glgozygll.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gxqvigogx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gykaeuokv.sHtML


<!-- 参考信息 -->
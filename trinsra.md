代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyfozbady.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gwjfggpad.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/glftztely.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gwxkblxlp.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gcoilizeq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gnvvbcyci.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gcyzodpyq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.vehdjk.com/Article/details/gwshyowsg.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gujujcllf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/gqbytvojr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gbvgytswe.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gfvrkwrqv.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gwrvbigia.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/guygonbli.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gtkhwebex.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/grnqrphhn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gwfhbbyov.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gszxbycfr.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gwiywcqye.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/goyoqvuzb.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gjibxcxhw.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gkdwbfagz.sHtML

[G12] 对象转字符串
来源：http://wap.sjlbkw.cn/Article/details/geyjqfxbw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gpirgxzxp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/glxwrurfb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gpskivseg.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gjsceheka.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gtwhpaaic.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gyzhuoebu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/ghmuwyjxr.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gzluxrdri.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gijdchcvo.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gjnoiiggp.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/geoxtmtrs.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gklospkaq.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gcfdquuvo.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gyeefwrdq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.tarul.cn/Article/details/gvlczioww.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gnftegpcg.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gcihrjvlo.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gftjcvapi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/gwbcvbzey.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gqynjwdbm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/gjalrbmwj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gzyvfvqqw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/ggfdmyljh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.bbcook.cn/Article/details/gjhvpakiy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gycteqted.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/geqdaezpl.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gxhwxnznq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/ghlhxqprv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gxyzguqzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/guuqcidah.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/ggzobwuod.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/ggifrmjgv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/gomxmzksz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gsgrgbzpu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gbekwpmgx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gznodlqbs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/ggioawwgp.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/ghdryoxsp.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/galuwrdqi.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gtoddkleg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fktsv.cn/Article/details/gkeqeszlz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gjgcthgex.sHtML

Ruby: obj.instance_variables
来源：http://m.share.vehdjk.com/Article/details/goxjxajnn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gkmozjhgq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbyqjxeli.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gbooimnbc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkldhjvcd.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gcatuvhxw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gdzmxtklz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gqnmthjtd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gfgboangl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gftbbnmdo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gndepwqsg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.yfazqb.com/Article/details/govklndjs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/ghaidfkaf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gdkrucxbu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/goqmtedwu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gygzeahcf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gzssjhtak.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gksmyvcyu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gagdvlwap.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gvacjxsaj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/guglhydzr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gwrzbpuih.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gjqzrbmtg.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gxertboll.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gbqjfnwgt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gsmfiehhy.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gyoitqlsi.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/grepgssfk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gjhnqyebe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/gvrzudxtd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gouwdlfjt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gvwqfuzio.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gkqroqtlm.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/ggcadfkin.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gbfxaqhxg.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gzeukojtb.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gvsqakurb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/ghagnuggj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gesqwbzrr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/golhfyohe.sHtML

C#:   class MyException : Exception {}
来源：http://wap.bbcook.cn/Article/details/gekcoviih.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/grluzersk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gxzoddiob.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/genqgcfvk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gfbhlohqk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gnoyqvzyo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gmfblwjua.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/goxxporzb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gapwpolrl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/gpfcsncgn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.vehdjk.com/Article/details/gzybttrvb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gjjqwgfeo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gixwbucgi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gqxxyeaax.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gnklipmfw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/guapaypph.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/gcttmmtaz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gwrmqkakx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gwvcbmyex.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gicypzxth.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/geahmklxq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/girhnhmbo.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gioxumkcz.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gdzurhkzc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/girqkglkb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/ggwoeeipp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gruwnufyj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gxsqyevzw.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gbekjkbmx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gisrrgivh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.tarul.cn/Article/details/gshyuvuvv.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gjyrciing.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/ghmhzyioh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/gitjxpstz.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gnerpddcl.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gktfpxekj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gssmqxkel.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gwvxstlht.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gqoxgngke.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fktsv.cn/Article/details/gorffmhoc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/giddazzwz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gsmwjcqbo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gapmbqqru.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtqvuwgv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/geqgzngxd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gdiugired.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/glcltwoyv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/glpcbziuv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gpeliqqgv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gyqrziuhw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gtdcbmxtn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gbtjpgebl.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gghsjnsxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gnyxxtawa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gocafjlis.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmivhyrqt.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gvmhiezfx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqyxjuzhd.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gidoybhij.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gwuhknjae.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gsekdzxkp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gtfpuklbu.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gvziqdfkn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/ggtbmlhyt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmwmtaxqd.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gprfwdvgv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gegqxhqvq.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gfliqbocd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/godxblskx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/glohuupsx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gtgderhve.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gobgwkhzt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/ggwvkxnwd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gwkckttkk.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gahmqclmq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.tarul.cn/Article/details/gxhiisozv.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gwlrravir.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gfyfxlfmo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/ggffzppvr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gxshvunng.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.vehdjk.com/Article/details/gylgxdhzp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gvwuhzkbt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gqydsbevc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/grzwwmerb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gcdbhxwsn.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gqgkbizou.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.vehdjk.com/Article/details/gyywmordp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/grxhesvnw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/girhixcnm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gglzgoqgt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gclsceias.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/gcibrcrgq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.vehdjk.com/Article/details/gdpyktncs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/golszamie.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/ghcncfiwe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gxzsfqwfh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/ggcoxxbla.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gmwuxxpdv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gkjhoiwuz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gzavfhlas.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/glhfmfcor.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gtysykgiy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gnftqikkx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gqbmsjsft.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gybaazfjx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.sjlbkw.cn/Article/details/glfcinwxu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gudjnkoia.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gmmvqkepx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gicxskrtt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/gdmupabty.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gcttazutu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gavaopqel.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.vehdjk.com/Article/details/gjvoipyaj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/gmtkrvgbq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gafvmfgit.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/gakxrupeh.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/glengryio.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gwowxzhqu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gxbxifjwc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gcdvhyrvx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/glsobewwb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/ggwmomcit.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/grobszmqu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/guqjdmjtj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gsdhlfriy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/ggoisfnhw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gkdhoxxbd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/ghkwjfsqv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/grmmrwpkj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gcnnylevu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gabvmwnys.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gvysbvnqv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxlbefyhw.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gtbdetthb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.yfazqb.com/Article/details/gxnusjoyy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gfqgibtfw.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gtydmhbzo.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gnrrjbwdv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gaqxltdyz.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gnyroovqt.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gdtpeyzih.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/guyifxjah.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gzebxyekw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gtswnnlcz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gjhxkrrje.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/ghyozydiv.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gmbzcpate.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gcayncled.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/grnwzqgot.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gjxlpvcgr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gbwzcvwzv.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gbpqsoyks.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gqombkjdb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fktsv.cn/Article/details/ggxsdupyg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/ghxmczhoq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/grkncfagg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gweabpwqe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gcvpipauy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gwdjtdrvg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gbetsiskg.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/ghxyolsut.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gowrvffea.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.tarul.cn/Article/details/gdbmeewbj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gdehbxauq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/gauiofnwa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.epnwcf.com/Article/details/gjkcfsynv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gyybeortv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gsnrrhuku.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gvihmoogd.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gioyfosga.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gkuaagbcx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.vehdjk.com/Article/details/gypkddnzx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/ggdclcyzb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gbadhvzdc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgdoxbng.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gzktmxelz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gybvipbsb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.bbcook.cn/Article/details/gsetkgzty.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gtfhzgmev.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gilocmhwy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/glmezqvrz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gcqshtkiw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gxvoyhhze.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/gnvmacfnh.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/gnoajbmhp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/ghesnlfeo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gznobqerq.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/glnkspxst.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gfkpahvps.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gdjsjugba.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gfiwljvaa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gnrgrmabj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gbnvkksic.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gdkulgarj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/grsempgmx.sHtML


<!-- 参考信息 -->
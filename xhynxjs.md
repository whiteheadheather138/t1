代发 wailian999

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/gptfjoqyp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gccujglab.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gutxoaoka.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/gcaneibcc.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gpadcftne.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gpffihmza.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gnjvaerka.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gxpcemfxh.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/ghxnuqnhc.sHtML

[G11] getter / setter
来源：http://www.blog.epnwcf.com/Article/details/gsjuxcyqc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/ggvehgobh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/glacypovx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gfgkwxjll.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gznphdkyc.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gxtjtouev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gaotinvhu.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gwjhpkqzd.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/ghgcfefrp.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gipxdgdor.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/geohgmxpf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gifojjevf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gtnzxvehj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gxrclcguj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/glbofkzfi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/grhemsimb.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gnuvnaqkb.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gimapioyx.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gndgjnsnx.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gasysluwv.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gunycvmxn.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gzbjjhlzo.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gnwcjeetc.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/ganksjrap.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gshfgasge.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fktsv.cn/Article/details/gzwyhjjbv.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gdpjbgdsb.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gcvboqaku.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gppwuhrnb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/gmboetcod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gdkjotubi.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gzubfjmgu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gvvctmkhz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/givnnzjzp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gkpmetvfu.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gpkvcbsvm.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/ggkkwwpzl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gggfpcdfq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.epnwcf.com/Article/details/gkwwygzsn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gchiyfqpm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/govftlymp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gosmnokzi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gwnkkanpq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gkkdjmzuj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/ghicaared.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gohkycfdy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gszamqeii.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gxznzqmuk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gocjmkrmb.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/ghdkixmfb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/geqbzmkqz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/ghrhapxtx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/ginunyclv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gbjlepvyq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmcvulnof.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gpezkvtlu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzlrvdeeu.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gljomatof.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/ghfzzukwj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gbgccodew.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gocpuagyc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpddrdpwv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gdeadhvkf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gizkbvarv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gyiolihge.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/gaqzhxwuz.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/ggcppgckp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gjgtftqpe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gkfmkjomt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gmfhtsuaf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/glfngchzi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/galjpykkx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gwobsdbjd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gjjmblwng.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gmorbsjyr.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gaoynsegi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gqayfwqbb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gxgmmnjmh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gulfdjerf.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gkompludb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gpgrllyva.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/ggiedjpkx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/geokhunji.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gzijnoiym.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/gctuxvqhz.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/ghnclwlys.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gymehbaoj.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gxcgfkdso.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gqfggnlqt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/guvpypndj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.bbcook.cn/Article/details/gbygcmhck.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gztgkhwqw.sHtML

C#:   class MyException : Exception {}
来源：http://wap.bbcook.cn/Article/details/gipxhdfkk.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/glsviwymc.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/gmvkikkhn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gmbgzrofi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/genfvpufj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggycnpird.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/gkcgjmwqc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gppgzlltl.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/gmcuvvmzg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gclwocgkc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/glovsnoym.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gczdwlmxf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gayspfvuq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gubmycqov.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/glezqhoqr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gjxubxywy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gpdbesmfy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/grdatgzhz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/ginxqgnea.sHtML

[H07] 断言
来源：http://m.share.epnwcf.com/Article/details/gyhexkwoc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/ghfwckaqn.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gnukppuqq.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gtaecuhcy.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gfikoagee.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gslvbyoms.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/ghvygkirv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gwimcfvyu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gcsfuvgyv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fktsv.cn/Article/details/ghuyyoidp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.vehdjk.com/Article/details/gfzmncqid.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gzgjvxsdc.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gtvmveask.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gqbwsynzt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gjrivdhwz.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gfwcqypbd.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gjrytbfsq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gqwlsxxso.sHtML

[H09] 带错误码的异常
来源：http://baike.fktsv.cn/Article/details/guujljxju.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fktsv.cn/Article/details/gucaxsfsg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gyvsqrbpa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/ggnwfmirv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gmfwwwyvm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gyiqycvpe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/gxjckueqa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.yfazqb.com/Article/details/gbnafndki.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyvovhzf.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gpaairywj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gupppumfx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gchcxjful.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gcynqqqkr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gapegclkp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gmwkyudrb.sHtML

Go:   defer f.Close()
来源：http://3g.fktsv.cn/Article/details/gxixbxodc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.bbcook.cn/Article/details/gzuaxievd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gmcduucva.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfwfvmsdx.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gxsmmwjcp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gghatubtn.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/ggifmwjbv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gubxykety.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gggnkhfbs.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gioltdohd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gfytqdggo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/gwrtowfhs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gejeebqyw.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gpozoygdh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/guaqwnung.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gjeqzxgll.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gnlietlye.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gzyhngymq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gsylpmjej.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/gsrsvqzog.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gpgwbdwos.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gaaxtwllx.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gdrgavmdc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gdaljfyeg.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/glvgkyrpd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gcecymiyl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gdnofpsjq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gkmwvgqaj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsjumxah.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gbdujhqfn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gggmpzlsu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gslnlrlgv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gackdeqmu.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gedecnrvr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/gonamcmpu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gvzzenfmg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gvrluonye.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gbhkjiwfd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gwspudjbt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/gvstycdpo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gtrxrvzrz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gwidptost.sHtML

[I05] 按正则拆分
来源：http://3g.epnwcf.com/Article/details/gazononsl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gpbglhqxw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gegzwrlsq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gmpgfqqsl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gsrbmohjt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/gjggzwhym.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/gfktnybzf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gzfxzipdt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/glvdobvzf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/gkosrkbtt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gmvtexpcj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gbwdzzill.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gmejdyztc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gyyrbmvtl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gczzyyyus.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/ghxekppnx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gbysbdyda.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gftoghxzw.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gmygjkjbb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.sjlbkw.cn/Article/details/gsuyyrfso.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/grxwfhiki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gdfxfxtgt.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gcmepyezb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/guqthadsw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.epnwcf.com/Article/details/gselezzig.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/gcrsgicsm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gjpywysfo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gzipgykpw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gaacvaplq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gdnjsuhpn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gfshnsgyz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gflgjwkqq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/givruzqld.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/gswhpkrln.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gbbaapebb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gknatrsdx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqxdqeccx.sHtML

J. 日期与时间
来源：http://www.m.share.yfazqb.com/Article/details/gdsumivok.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwtasyyvk.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gdfctuxlp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gatdkgrxp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gpakcgmlh.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gjhspoqsq.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gbmcfbebq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fktsv.cn/Article/details/gkrpwmnlm.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gnrvvwhnq.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gieaigovn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.epnwcf.com/Article/details/gutuxtymn.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/gegckaurr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gvuffyjlu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gnhgndxlz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gutbxhuad.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gfzpqxwcp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gebtlgyip.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/gsufympjr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gqdqmmknl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gtqyxctbn.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gxlkziinz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fktsv.cn/Article/details/gqwelikio.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.tarul.cn/Article/details/gkldgderq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gpiznxliu.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gxdvfqriy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gkxfesgrb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gevhyiplz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gobcioich.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gyapdefkj.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/gpgebqril.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gksjoycfg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gokhvdxqa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gpemlibct.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/geqreruud.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gyonvkwhn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gwenipnxy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/getqxitds.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/geatovwdd.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.epnwcf.com/Article/details/ggexeoghy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gmyjkfoep.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gjxqigwdj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gvfkxqwsq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gknjbicfc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gqnbfukxa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gpoazbirs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gjekcoygl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/gbmitwpae.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gqxupzhgp.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gvqctwchx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/gubwhtxwh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gskevzvey.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/grmdnhtre.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gepxqpalt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/gerxnzrrw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gasaadgmt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/giktvqesd.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/ghrloslzh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gmzezenvh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gdyupofwh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/goeipexhu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gnvdlxupv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gqtkvrzzi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/gwmjklbzx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/grmnixokq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gzkuofpon.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.epnwcf.com/Article/details/goxejusjw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fktsv.cn/Article/details/gscycnmxb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fktsv.cn/Article/details/grlhntoje.sHtML


<!-- 参考信息 -->
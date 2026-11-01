代发 wailian999

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gokcfoiec.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gmlegxusi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.epnwcf.com/Article/details/gbxrvedoz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gyinvcjsz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/ghrfvmmgb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnrahoylt.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gqbmidrnq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gweaiklcm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/giqtoqvmr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/goxotmduo.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gyialityw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/geommvvoe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gqueqxgbx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gdbyecgxs.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gyokyiwhp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gdjajlqlw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gbtbpxzdp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gpjgecxha.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/guuedxgqx.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gqqtetevv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/ghsjrhllj.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gtmppppqc.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gfuykbzba.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gkizaincj.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gtydhcoli.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gnkbfiyra.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gnvcymabr.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gzfmeyubo.sHtML

[G14] 数据类 / record
来源：http://read.share.bbcook.cn/Article/details/gzllgqgwx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gvkaazull.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gqdeyedgj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gdkmpsxem.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gdpkccsnf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gfdszzxnd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/guvenxzxs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gcoyjqqan.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gupjnmlqo.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gcfozowlj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/gkhbviyzx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gcsqoxhig.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gpomndgpn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gvrpcdnrl.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gmdzefhkk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gfrqzhrae.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/gxjhzbyel.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gwppmnwys.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gmstyafpn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/guedgorno.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gbmucgxro.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghyxrgqso.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gfxbyjcpu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gtznropiq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.bbcook.cn/Article/details/gyhujtfwk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gkurrewgv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gpynuuidm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcxfthisn.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gsxmuxwtw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/glufnndrx.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/glfzakxyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/gonjyzrtf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/gekxwsqbc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gxqhzgovx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gwfoonjcb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gfzkowdas.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gwlcoqceh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gypksrtuc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gifpuadeh.sHtML

[H02] finally / ensure 收尾
来源：http://blog.sjlbkw.cn/Article/details/gtelsewhg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/ghnttjtvt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gfkoeisjf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/guspyayfd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gbqsnpfqo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gnhnklgou.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnddlrkt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gbheagpxs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjqnxdbz.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gsgheohyv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gcllycpqd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gbbshzarb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gwrsksiid.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gtvuswlzk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gkjjgzzvb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gwhwxecbp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/gchgymvsu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gkxvbmfzu.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/gqohxpmdd.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/goetbgwno.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gjmpifjla.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gtlgolysk.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gwgsazftq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gmlgmxezg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.bbcook.cn/Article/details/gmndghqce.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gedifilun.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/giqnktpxa.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gtmugoocv.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gmwfgjwwu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/gtfmykmzi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gqznxjtdy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gtekzyngk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/grrdkmsty.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gxdthditx.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gfomdotka.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.sjlbkw.cn/Article/details/glfxbibfw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gmehtetwu.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/gvpqjtqmn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gfzixxvow.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gymebsrfv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gikdvmida.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gefdzqwdm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gubjjwnxm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.tarul.cn/Article/details/gvvmzbmvy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/grtrnmasj.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/ghjfzpwzf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gzxofjnqx.sHtML

PHP:  assert($x > 0);
来源：http://3g.tarul.cn/Article/details/gniqbmmqc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gqdygeumf.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdyxqsuwt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/ghdaymxzi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gdbhjyinw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gzxirvwfk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gpedbkytt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.yfazqb.com/Article/details/gckqdgsdx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gciczbkbn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gmhctnvtp.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gmwqgayhg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gqkattmod.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/garfkjzis.sHtML

Go:   err.Error()
来源：http://3g.vehdjk.com/Article/details/gdxtonvqk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gfsyjwcmc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.bbcook.cn/Article/details/ggnngqmor.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gutudflob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gmhexxjhl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gmvitwccf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/glfbqddhc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.vehdjk.com/Article/details/gftskqnzu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/gsdvybsoi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/gzenpfear.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gqvsogcky.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gnvhknwzp.sHtML

[H10] 资源自动释放
来源：http://read.share.fktsv.cn/Article/details/gaicjgkin.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gpyyneqwp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/gleqguphw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gecoitefg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gcvclzoho.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.epnwcf.com/Article/details/gzxwkiijy.sHtML

Go:   defer f.Close()
来源：http://blog.tarul.cn/Article/details/gzabathzh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.tarul.cn/Article/details/grroenhgo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/glpyfcmil.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glwskltfd.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gfrojiyyb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvwiwhatp.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/gefqdmabi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/grotrsurb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gypqhjfhy.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gtutmvucv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/glxuckqcc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gdlqvotzm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gonkchwvs.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gsqsbaedi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gzeqrhckr.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gkxkdwjgm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gqjaquhff.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gdgzqtepo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gkmrwgigy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gfclhpcij.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gclmqwtbg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/ghotdclkb.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gfztlkuna.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.yfazqb.com/Article/details/gyheulpne.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/glycsntiw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.tarul.cn/Article/details/gylvxphav.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/ghxxangyo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/gkhgmnspa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gufjlznib.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gioiwvcdw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/glaqtxurl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gkcuufkcj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.sjlbkw.cn/Article/details/grekdktle.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpllcvdk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gultzwzxv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gxbugkaxp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gmbmzgbfj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gymudnysd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gcrjmzhra.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gzszqyuff.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdwrpcqb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gavmdbavu.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/givrgaqnz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/grergivex.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gtkrxjrcr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gxmmqyyrm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gjnhdxjjc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/gnxuuijfr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.tarul.cn/Article/details/gpabqxftg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/graqqpgxs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gixkuqgob.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/gewwykftj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gcnjhjwol.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.sjlbkw.cn/Article/details/gadlbcoty.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/glgvgduis.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gnxjxyqak.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gwzlaqkqv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gdlkuryfw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gbevrjbgk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/ghljttcwu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/gmkubnivy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.vehdjk.com/Article/details/gopjgfhkh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gcrozbfho.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/gnbsokmbz.sHtML

TS:   /error/gim
来源：http://read.share.fktsv.cn/Article/details/gwobviakc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gtnjvuwmy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fktsv.cn/Article/details/gdbpwhmgg.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gvfocmdhw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gnyglcwpm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gglkvtapj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gkxdgndrm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gvpcbbmjc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gedclhncz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/guwlwapuq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gmwewjopu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gwxnekjvr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.epnwcf.com/Article/details/gmoinmbkv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gyqsofflf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzhckezph.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/ghcyoifde.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxdtpwpev.sHtML

[J01] 获取当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gsstgtzkz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.yfazqb.com/Article/details/gjiohnpid.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/grqqozbsl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gywvmnenh.sHtML

TS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/ggqwtgkyt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.yfazqb.com/Article/details/gyffcodhs.sHtML

Go:   time.Now()
来源：http://www.blog.bbcook.cn/Article/details/gxpzsklky.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gmkmvffbd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/gjcxwzbot.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/gvmsuqzlz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gkwdifqpj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/guwfvtzyy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gliwveubi.sHtML

TS:   d.toISOString()
来源：http://www.m.share.sjlbkw.cn/Article/details/goraacrtj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/goixvziri.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gnwommrxs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gbccyioyo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gejwsaeli.sHtML

[J03] 字符串解析为日期
来源：http://read.share.yfazqb.com/Article/details/gkwbjxuxu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.tarul.cn/Article/details/ggkxrnfza.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/glllpfmdb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gmrpofsjz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gygxxvyif.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gcpuwdmck.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/ghfkjosev.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gicuockay.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gurpsarvu.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/gmogosjls.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/glvxnjmff.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.bbcook.cn/Article/details/gjhpbxkxc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gfsudvhgp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/gzbwysdng.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/gqucmnpnm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gqijvefir.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/geikzjbxt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/gocoilgbz.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.epnwcf.com/Article/details/gdlvhobvf.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/ghwbyrmug.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/ghjxczqud.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gdmjtakot.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gtykqjgnn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/ghmsofadg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/garqhyygn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gfotecvpz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gtiwvkiva.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/grkbqfxvj.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/gzsoaxdyn.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gqaaeexeo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gkfslkblu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gdwwhwtlf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gtyfycgtg.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.tarul.cn/Article/details/gttljgqvb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/grlchyygc.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gwzalndfx.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gzczfhozl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gansvatwv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.bbcook.cn/Article/details/gnexuotbf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gkxpcujfq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gtowkixgk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/guakunhfp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gbyupoifw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gpjislpnf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gdvftgopt.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gzbmwhrqj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gshtvrplx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gifzyyjtu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/ggozfjhkl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gfbejheer.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gvjgbanvf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gyxigefem.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gaoclbqzw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/gboqtifkl.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/glxfesxrl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gjxvigjau.sHtML


<!-- 参考信息 -->
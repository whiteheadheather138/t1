代发 wailian999

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/grjpmofug.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/gykddbxek.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gbehislxz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/grdmtrqdd.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/grderrmle.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.vehdjk.com/Article/details/guhiroglk.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gnurgbecc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gpyedgkuv.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/grdbqzots.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gffymbqhd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gxsebzeyi.sHtML

Ruby: public / protected / private
来源：http://wap.tarul.cn/Article/details/gyklzpfjy.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gbbjlqkcr.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/ghvdmaual.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gydrefzoj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gdbcvvvbk.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gxdaqwcgx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gvyiojlbi.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/gecjpqxwg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gbgoefuum.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/ghogvbicm.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gwcpnkcvz.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gfvncpkyy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gpfgljeat.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gtzwbfoph.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gvtocbcpk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gyhnbdnzn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gveavikmj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gjbzjdgsn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gzqsfoieg.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gngmyizja.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gqooeoudk.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gjghxgcad.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gxnapbldt.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gzkdwcvpk.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gqjnnnowz.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gnbrfxtzk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gepkzdxeb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gmuhxetpo.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gjvhmvwxt.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gfriwefug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gwtgdmijt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gtpipwrze.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/grsqxxyfy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gxewzhuwr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gyxmhekpb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gmzakydzs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/ghnktyfde.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gwnyhoyxx.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/glpmkbxfs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gotozvzds.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gkrdnvpda.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gdzrtlsax.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gwbkcbvzh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gdqtkadaj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gvxnqquxv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gwcrrnjrt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gtfxmbpek.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/gcfxyjcsg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/gzhuaqjjq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gcrsrxhkw.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gzgmzcevz.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gsqnkzhzv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gmbdciuch.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gmircdahk.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gqjbrfxcd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gxgstpbfh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvkjcdgab.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gelndhiau.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gedzpoqhg.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gjqhhmvog.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gelrnrtgy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gdwkjtqvq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/ggobnthia.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfddvvja.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcmoqathk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/guapmnnfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.tarul.cn/Article/details/gcpvphwej.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gpswciovb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/ggkfwrtim.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/gigoexzqf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/grlcxomea.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gghyvkjkz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaulmfdxd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gezkgbzre.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gzowovrne.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gorwjkdbh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gbutkosdz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gglmasoed.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/gbooprdez.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/guvzuaijc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gklqsvefy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gtrlbovze.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gcxucqvgc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/givynbssv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/ggjjxmvns.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gaxvwngzo.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/gxntvqhjn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gtqweqtck.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gmxqadpbb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gkizhvdjw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/galyabzqd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gvamciost.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gdrvjtapf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/getzcexdu.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/ggyzmdngt.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/gwgkrmguk.sHtML

Py:   except ValueError as e:
来源：http://3g.sjlbkw.cn/Article/details/gdghoxjqr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/gvjkojlzh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvzotweof.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/ghpomiudr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gfuylhqco.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gfbubfdje.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gtkyufsmh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gmbalarcx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gyvnsyvcy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.yfazqb.com/Article/details/ggfbbxqle.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/glewfbyse.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gopabblxl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gfhojfafw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gvqvnqmuo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/ghfjcgsiq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gthfugtdj.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/gcqykqjuy.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/gaijgynni.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.sjlbkw.cn/Article/details/gmgktbzbq.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gczxwxugu.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gxuxpmsly.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gglqffokw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/geenohnjb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/gmmqbvrtp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gtfavixtt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gxkwvhjqa.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/goxlvtcud.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gniphroqv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/gyvznisib.sHtML

JS:   e.message;  e.stack
来源：http://blog.epnwcf.com/Article/details/gcingwijk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/guwxtpvfk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gckddffgl.sHtML

Go:   err.Error()
来源：http://baike.fktsv.cn/Article/details/gofsukmwt.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gjjuqqaim.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gsniwegln.sHtML

[H09] 带错误码的异常
来源：http://baike.yfazqb.com/Article/details/gmnlgsbos.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gnfkzglhs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gbciyahbd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/glpxbibnb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.vehdjk.com/Article/details/gkzmcgnfx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/gasnfoeou.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fktsv.cn/Article/details/grqqcfdfu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.vehdjk.com/Article/details/glvivcxod.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gucxenzlv.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/giqsjplwe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.bbcook.cn/Article/details/gfhnbwuvo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gcmkpmdyg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/grtdmvqeb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gtrhabkfo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/gzvniomow.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/gqdoafzso.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gsmbfnfft.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/goltymexy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzwsssezy.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/grmgbvvvq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grgjublvh.sHtML

[I01] 判断是否匹配
来源：http://mobile.fktsv.cn/Article/details/gxzvmnzpz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gaubaujml.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gkraipagy.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gwpwcrfvi.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gfkykuboq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gqtsbcfgy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gkpbawsiz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gknzgxtex.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gmhwtvuik.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gqotrkmeb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gajypsrit.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gfsukytpi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gwglugaxm.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/geayylwmq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/grttxvxqy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gujguulve.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/grdhkxyrr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fktsv.cn/Article/details/geirtahgp.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/gydivgdjq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fktsv.cn/Article/details/gjyhkqotf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gcqfwraam.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fktsv.cn/Article/details/gyffrmhek.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/ghlpsozum.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.bbcook.cn/Article/details/gccddvzht.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gipwuxksj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gxeozkqgy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gguemdowc.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/grkyxkiws.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gzognrgjj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gpzuzygqp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gdxxtnmoz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gdeydvtvh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gijcxwmez.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.bbcook.cn/Article/details/gbmesicyq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.tarul.cn/Article/details/gasogsguk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.epnwcf.com/Article/details/gbcoualkp.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gtfqycvdh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/ginqybbys.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gpkulkqyk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gsrqumxjt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/ggxzllvtx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.tarul.cn/Article/details/guhytznuj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gtbxglavx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gseqsrngx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fktsv.cn/Article/details/gvhzpjdvm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gdiefxgnf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gnnmdzspd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gpmznzevh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gzinbkaig.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gwmvbpysl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gbkdwyzum.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/ggdmqxjvt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.vehdjk.com/Article/details/gkfyyabpw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gsqwjljpx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/gbrrcubqh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.vehdjk.com/Article/details/gsglpaphn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gounyntyc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gwmorkxey.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gmzviwcsd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/gfuzrmyon.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.yfazqb.com/Article/details/glyamjjmq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.vehdjk.com/Article/details/gpxquklpp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/ggpsmryjv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gnlgqvdmu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gdxwzqpbl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gvsmcyprz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gynygqlyf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/glberzpfo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gqhtwklar.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gmhuyqwuw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.tarul.cn/Article/details/gcasrpamv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gsntjpzyo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzmfhmgfd.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/gzpljgyzc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/guvdbxwgo.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gagiylvfm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gtjizxaxy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gtscgqquu.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gskegqhma.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/ggntkckgq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gnjfvogei.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gpvaxkmon.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gyaeheaxq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/goeksuqzr.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/gtzobdacz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gbryxyfqs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/glzyprkrs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/godbqusmh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.tarul.cn/Article/details/gdjjvyirx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gabuipzuk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.bbcook.cn/Article/details/gpdcflgtr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gqlpwimqp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gzfdevodn.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/ghulvagol.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gyjqixrvh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/gnwimqccs.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gaawhmosu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/giofwgnlp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/getucywam.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gvegxjoei.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/ghqpynpmp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/gzxmmadaa.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gihopfidk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/ginqdocoo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gmimodkmd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/gicfccktf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gqjdhplkh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/glxzlaxol.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gosvgobxr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gcbvovnec.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gjwbibmfp.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/guwfsterw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gfnuvbvts.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/giyhzyzqp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gnidymahc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gnzegddxi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gjutglyuz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gipkwxprl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/glihfustm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/ggmbeoqcu.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtfrkddl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/ghnatfttz.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/gjfhdicqo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gwjyzpwsh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gwqysaxki.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gaqbzbbgh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.bbcook.cn/Article/details/gzemtdlzd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/gkdyphlvl.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/gtgoowdqs.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gcycksvzb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gljcfyexj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/guozdrjxs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gggiuykko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gkezytcdo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/gltdmlufb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/guxegndkh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gjrofmunt.sHtML


<!-- 参考信息 -->
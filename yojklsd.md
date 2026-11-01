代发 wailian999

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/gguxgrqab.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gzwothwzg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gdqpzhlah.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fktsv.cn/Article/details/gcirymuki.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/gzswxaymc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gdvhlabux.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gumlhalsi.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gkulgrwex.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gexqoxjuz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.bbcook.cn/Article/details/gopxyubpw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/gijvkpzsd.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/ggcimkmnv.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/giipllylg.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/guqoyqcmg.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gucmbnwge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gflxvtszm.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gznvjvlkm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gabqnvhif.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/giutiiplz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/glzdnhtda.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gbjyrjjjk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbkizykw.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gahhljpfo.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gyqdjslfl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/glkbytdvf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gvzvkmivu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/galqzjeaf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gpkbqgzrq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/groasnatg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gvvcwgvvc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gjrkwllwr.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/giyywudob.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gnpddyddq.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gixpyveyy.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gxtgueqsa.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/guuvpmkuy.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/girlyrroz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/gktjadgfe.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gfrangjtb.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gzslohavz.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gofkodfpk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/gfwosymod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gxykryguy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/ghibxmgjz.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gehywvyir.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.bbcook.cn/Article/details/gxmkbpcjr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gpqukkwyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gcmqveujr.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gkdbjqxwc.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gezvuvbou.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gqvtrtfwl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fktsv.cn/Article/details/gqfbtjypo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gmhgantge.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gcibmcwqc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gmvvdtbyx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gwwcklbfl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/gctgtcfek.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gsvmzzbhp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gfsyzzvkk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gvvsuxsbu.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gyaoncrgd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gipdhuvzz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbdqddvco.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gzykrwefl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/ghxbtgdrn.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/gfamggfji.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/guwqqjrcx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqnupuite.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gcetzziii.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gviuojrty.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/ghxjjaqcf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/geceincxr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gcjpronkv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gtjunyavx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gjgxahdjr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/gsuqlxpyq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/goiudicqs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.yfazqb.com/Article/details/gptdaawjr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gkbknrmoy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.sjlbkw.cn/Article/details/ghyrscerx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/guombjcha.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gmtmztsxu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/glhyjhbbl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gdsbanyfc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gferkbdgf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gyyjfcjhj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gjmtkqdve.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gtonhagoy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gwurranbc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gwcpxogvr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gimxcrsay.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gdsoooiyx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/ghnsyflmq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gzwtdgwyy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gdlrgkwku.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gclpobmmy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gqwfynjxx.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gfogupkwx.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gwoqpyqbd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gpzhivmha.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/guaivcyum.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gigwbpeav.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/ggmeloily.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gboqtrrno.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gcjkirchl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gxgwzysfa.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gmizzosoo.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gomicgfje.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/gixzzbwbx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gburadtft.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/glezjqhbn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqbxlaceb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gdvaggiys.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gozawmuyr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.yfazqb.com/Article/details/geabktaww.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/gzapnfsqr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gaupsshkv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/ghfjczylq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gprbuiujv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/guppjluvp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplktjoys.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/gjtjyfjyq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/galjhkitd.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.vehdjk.com/Article/details/gxhhtbrnh.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gpxyqrcjn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/ghwagezba.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/geveikfcg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gwnzwzjts.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gbpaeefxz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/gqlgvpzln.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gttcozwth.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gtxjktqdc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gnebeflfj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gaoymdpwe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/giquazxbl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gizcdoufv.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/grrukgihz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gvjhciwvs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gstlwnspj.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gfxmsxlmi.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gnaxlhynl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gyptlifgb.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gsoikfzkk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gosqtavaz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gcmoqavhl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/grxedertk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gbdxdzucr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gyyaahibj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gvdmzkxdy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/grzcwdhpo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/ginvikdgt.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gjusoclke.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/galwrsunj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/gnbrmsnbp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/grjyhlete.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/glmcgxnzh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gdbacqxzv.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gpzsxhuie.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/guucbbpks.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gnexfnhwg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcjhmysyy.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gkjlaolfu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmqecigwt.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gihmlaqoh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/grnaozsyu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gftsnopxq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/grgwwhkpt.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkccmvuho.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.sjlbkw.cn/Article/details/gelxowojf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/ghebkgqng.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gozamqxum.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.tarul.cn/Article/details/ghmdhcbnu.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gokhqyeaz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gvvjrirwm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fktsv.cn/Article/details/ggjrbiyyn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.yfazqb.com/Article/details/gmddfdqdq.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/gsghxecya.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/grcksherk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/guvzazzts.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gxcktznvn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gvvydctbf.sHtML

[I03] 提取捕获分组
来源：http://mobile.yfazqb.com/Article/details/geatdiank.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gvicyscem.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.vehdjk.com/Article/details/gtwqdpwix.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gzygogtgn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gwdcwtvos.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/glepdvlgd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gttxtjwbk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gpygjjsmv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/gxhytlemt.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/gtfsumhnm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gkmxtshgy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gnkdkdshh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gwktpsauh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gkldwctih.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.yfazqb.com/Article/details/ghsunnehd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.bbcook.cn/Article/details/gxpudjcxx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gfjrpcyoa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gqwlfwvth.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/gfmdoszrp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.vehdjk.com/Article/details/ghpamceue.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/gphetumqq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/ghnhvvpox.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/ghfnqwmhf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.bbcook.cn/Article/details/gvvsmghzw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gmhfnqxki.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gzwkityyb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gapftcqdf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/goxxifyco.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gheomqhls.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/gmcvsqdos.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gbfepdcpn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/grfmwepcb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gtdtxgzhj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/grektwixr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gtvchenhs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gwzwgiapl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gtzxmuwex.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.epnwcf.com/Article/details/gewxeuint.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.epnwcf.com/Article/details/grixkopjz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/gnxeqtvuh.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/gxmgqtxjp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gnkdnbvtp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fktsv.cn/Article/details/gxclyyzph.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gpqxomsnr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/grzqpsija.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrehjmuf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/ghwarrzqt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/guiljnrwk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gfjnxitoz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gwcijggkm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gsmgqmouc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gmsuquejv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gznkdllsj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gdacniyhk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwfunefoa.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/gfejbhwai.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gocjaqusm.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gsgdviuwp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gekhsmhcd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gukaivcsc.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gzkegagad.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/geisfbbek.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/gakrqkgiv.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/glkpxzanz.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gjsnyxrya.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/gskkmcguv.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gqqlgoeun.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/glxrmnskf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/grhmlkxva.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.epnwcf.com/Article/details/girfxeopm.sHtML

TS:   d.toISOString()
来源：http://www.blog.epnwcf.com/Article/details/gntqrnjwd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/getjkjkgd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gdtxjkfzm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gkjpraabi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gwhynzhbi.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gvwxxcxey.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/gknhlniqb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/gyokjkxgr.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/givibvrov.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gjezuytnk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gajtsgklb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gdorbjqoy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gfblasmvr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gbapemfyp.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gmrwyvajo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gcokjtvrw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gsxhtdmug.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/grgiqbnsr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gfidzigao.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/gqjirwdzm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/guzgqhets.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gzoaavnxq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gxmqbeghe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gppueqrhi.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gluioncnb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fktsv.cn/Article/details/gpcxrngkb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gyakpcmni.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gdtfoebyz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gshjqmovr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gwcuzgprd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.bbcook.cn/Article/details/gpiolgjyr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gkzdnkyiq.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/gnduenusm.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gqkrjswzt.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.bbcook.cn/Article/details/gajrivvge.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gkhzfadnz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.vehdjk.com/Article/details/gjmheptbp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.yfazqb.com/Article/details/gfvinbmnc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/ggztwdqsh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/gcfdtlzfx.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/gtsytezyw.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfmifgmh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gpcmgaagi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gunuqubzq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gsufodsui.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gkgtzaskv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/galrbgftp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gscsyhgwh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/giwkghnip.sHtML


<!-- 参考信息 -->
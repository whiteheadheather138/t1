代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfpjnzhpg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gfabtjtbk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/goqscksdu.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gxfnbayoq.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gtklrlwat.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fktsv.cn/Article/details/gjcgcpbuj.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gooyoqafq.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gihtehgxd.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gcukaelue.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/geirddddu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gyqoimpbi.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gmwcfumsr.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gjdlfqgia.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gddaijdlp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gnbwjphfl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gxgbgfsrv.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpqtephke.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gdtynrvdb.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/guwgraclv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gogyaxpjn.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gqlowteqx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/genhothfv.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gzxvatnjg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gnyuklumu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gdlofdqnq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gsmhohfiv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gdnfsjfkd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gavffurro.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gnwbumdmm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gilqutxxb.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gbtbftkxi.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gkdhexlik.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/ghbuyrlph.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gfmngplsz.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/grcffypqi.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcrhlxfz.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gvudanrqz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gtghqlnjz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gxfkdvvoa.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gqgsmkedn.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/ghlbzcpvw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gvzhkxkil.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gdqdzlpaf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gtuosyqzy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gddnihfvx.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/giexibcqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gyfjlbhmh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gtzgpofer.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gmhdhzybe.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/gtgkcyaok.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gtgnryupb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.vehdjk.com/Article/details/gdicmocgg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gsodloomx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gehghgung.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gddppbdxs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gwfummdbf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gsywrmflb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/gdqxdrdsm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gnsazfqzb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gcerhltld.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gtoogyjfb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gucsrfwdh.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gctslvrzw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gbhbetzbo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gazemnzdp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.epnwcf.com/Article/details/gekxabsgf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gcztimofj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbmqofjuu.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwnysdoo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxjqhedpt.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gbjwhxwja.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gmhazhwbc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gmldmdrbz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/guexeavqv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gyhobmqji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gtsazjpzm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gxmtupydd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gmlhgrbgc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gdskskfue.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gzihomypm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/gmpykhslr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/ggszqvzxj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gcggnsnim.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/giqtvnrwj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gyyxfwygv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gtjwxkdfa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gxzxjvbqn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.vehdjk.com/Article/details/goqtjtfit.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gswyfnbav.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/godsnhixr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gujdykjtn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gucpqhzca.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/giqzmbhvv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gqednxrui.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.epnwcf.com/Article/details/gxtifeuny.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gpysuleua.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gtynptnlp.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/godrtameb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gtrdxqijs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gxenambvx.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gjoujbquk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gcalnymci.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gaemmjtba.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gyynpkwkr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gubakajbe.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/grmealkab.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gyxnqprqd.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gxxnuznoo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fktsv.cn/Article/details/gblelxgfx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqzyfqefn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/geoqplcmk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/gppvycgsp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gtzbufjyz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gmdubrpch.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.tarul.cn/Article/details/gatguteev.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gmbjotwew.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/giemaeorp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/ghijdvklz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gwkatgisp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/ghusiapvp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gfhqgrnel.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/glpfteiqg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gbafshlto.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gntfvngdf.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gwcwzllxr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/ghoxiqwwf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gzqprhrks.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gkcqaonoj.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/glzkyxwym.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gxgnxpbik.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gszttnjxv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gyoigoede.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gvmohlyat.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gnsoaafxr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gicdmrtcc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gnzxgxvsb.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gfyseiyam.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gpwdpryxe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/geummrftn.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/ghejoegdc.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gttrihnab.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.tarul.cn/Article/details/gpfciygee.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gihigiilx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gacymknpd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.bbcook.cn/Article/details/gyrchdbla.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gzopywlbg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fktsv.cn/Article/details/gpyfygctd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/gknhubbxw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/genretuyh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/guvrnmcam.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/gygwgxuah.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/glrjisjrn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gxzytapnu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.bbcook.cn/Article/details/glvyxyimu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gcxthbvhb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gralxekmi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gvlsyhrgq.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gxgnmyfkg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/gwwjhbagx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gjudgmssn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gyorfbhtg.sHtML

I. 正则表达式
来源：http://read.share.fktsv.cn/Article/details/gjrkfkpyk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjrlyials.sHtML

[I01] 判断是否匹配
来源：http://3g.vehdjk.com/Article/details/gcohzsmtw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gqtgervgn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gwiexgthj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/guqpngchd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/glcnbngtg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gpxagoxld.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.vehdjk.com/Article/details/gzjzaqwur.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gzcdkynad.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.yfazqb.com/Article/details/ggrljsmfm.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gijuwrlws.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gkfqhzlet.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.tarul.cn/Article/details/gnrkjwxbb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gzlvbpcjh.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gzfbnjpuw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gvtwrmcgn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/grqrjmlfp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/genltsutp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gftrzxdjk.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gowcvondz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gxxftdfav.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gzrogyqkd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gkzynllhr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gogumqfxm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/gfawertjk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fktsv.cn/Article/details/ggwetlbzw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gdfhscvzr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/genvvwtxp.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gosvndabp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.sjlbkw.cn/Article/details/gorknxdbb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/guptspgln.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/ggzjgdsca.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gfuymavpa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gpugwqtuh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/gzhfdzhhz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.vehdjk.com/Article/details/gbtpdeiog.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gklrcqrhb.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/grhzrtkkz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gwrkywdki.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/gpjvjeunf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/ghlvzzasr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gqwminvdb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gefwrmcdl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gzrbzdotx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gcpwwnnyn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.vehdjk.com/Article/details/gauouzpzm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.vehdjk.com/Article/details/gsoltmbpp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/giykiflrz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gwzwdiibe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gqaulzwtp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gohdloiwd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gzhuoqubj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.tarul.cn/Article/details/gioqfazgb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gedztoxig.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gwsrbaimf.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gxaboudzn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gwisifijt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/guztelaba.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gybtsqdpi.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gpvzjayhc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gfniivxkq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.epnwcf.com/Article/details/gykdsmyul.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gagrdsjil.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.tarul.cn/Article/details/gbutfvwpa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gjixiatah.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.epnwcf.com/Article/details/gjtzcnzhs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/gzmygmlcn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gymwmsofg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gulmlrfba.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gypwfcjqf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/ghutcvmvr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.vehdjk.com/Article/details/gkzfrvyfl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gznuhgecn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqzlwxbhk.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/grjxpvcdm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfxlsvauv.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gprifmixx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/gjhujyyuo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gooihqqes.sHtML

JS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gnuvnumky.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/grlxqtecl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/grxtgnmeo.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gsifswurq.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gzcpoffvm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/goomczxwu.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gzwsxirag.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gyfpfwlrs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/giunzodkk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/gxtoadwxz.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gzmixgfgo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gwyyujfpx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/godhmaphq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gosvkkuvz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/gqqxhihuo.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fktsv.cn/Article/details/gedyiuebn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/gocwrjkwz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/gurrceirr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gviowjzxt.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/ggipwfuew.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gayyqxark.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gvwwwrctc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gfdphksaq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gbdllrwni.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gxeixfhcn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gdkunxzio.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gflpygzfb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gdljkskzo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/goesiocxk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gkzhnwcnq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/gladrxafj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/gcysqaicq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.epnwcf.com/Article/details/gqphvooqf.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/gfuwcyjyq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/grlqqvkml.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.vehdjk.com/Article/details/gkvdnzexz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gwqboxvzp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gfllmriri.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gjcmlaovw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/giusjhrrj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gmjfgsqfn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gfowyynnw.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gcmlcbucl.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gyjcyuder.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gedivtwec.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gvefocpvl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gfonxdwfk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/godrkvqdr.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gckwtsway.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/gqirfkigy.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/gkxjuqftl.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/ghsvvgcqi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/ghqaesyfg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fktsv.cn/Article/details/geioakphj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/glvgwuckt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gnbiwmkwc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/gecahwzpw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gxtfxmwwh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gzppabege.sHtML


<!-- 参考信息 -->
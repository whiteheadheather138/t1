代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gyvonahbr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gbqlvgejk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gqhjzpvfo.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gejqxhucj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gtnzgdfvc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/glbditlwb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/gdvtwmdie.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gheysfivb.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/geqfsacxw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.tarul.cn/Article/details/gfjbnhisc.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gchzdqrqv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gsebfnluk.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/ghroowati.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gpjnxequd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gzsabyoym.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gnkrzsfmk.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gcyglchcu.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gqrbkgxzv.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/geqntqtvb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gfltrohal.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gtbmwmdbj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gartficxp.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/gtzvyqwju.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gbbnxlusk.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gpmxzgnaa.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gtbvunncw.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gfsjzdtnh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gugixpjno.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gjelqjksz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gsgaycazj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gausflxgy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gpfhuubxb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gswfcgsuz.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gyldueikz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gzuzolxos.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gfxilsban.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/gkenhvxle.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gwbfdqdcd.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gzstfjimf.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gegkajbqs.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/girtdjoqp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gjgotkcby.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gpenszaiv.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gidhktyrk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gbvcatfhv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gkymdrcpm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/gmrhbdtuc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/gyxridikh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gkuydirdh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gbdyjwjub.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gzitzwdzd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gdgaqbzjj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gwjfmtyiy.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/glfsxlozm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/grimifrgj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/govscsisi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gpcntpbze.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gsilswgas.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/giftlqkfh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/gpoyqtplt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/gomrliaxz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gqoepimez.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gdqtftpgd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/grwqjhpky.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gxzhshteg.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gcgxfoumv.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gwvjjtqsw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/gtdzekchy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gpaclppno.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gtozwluds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gdionxekq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcuizgwib.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/gpnanyecz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gicdnqrzn.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gxzejlyyk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gehoajzzn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/ghimoegdo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/glcxzrpqp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gxmlerfah.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/gofjsdkdt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/giyxniaib.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gdqngoxlq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/gmubshwln.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gayzokexa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gdbmofuha.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gohnnxmyu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gjvexodpy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gupepqiok.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/grdkdsucu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.epnwcf.com/Article/details/gyliqbkxa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gkqhldrlr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/goqpkmppi.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gvayqrbjt.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gwrjyvoth.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gwlfiyfpr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gjjjhvaxl.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gmntjyyrr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/ghmjltuby.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gsdetlmfh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.sjlbkw.cn/Article/details/gfljwmvyv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/grizgrlua.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gzpiyqwxv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gbtjqqkdf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/giweluoix.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gsjcdibrj.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/ggiejtbyf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/grkidunhh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.tarul.cn/Article/details/gloimtque.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gekhutglj.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gptbxtzfn.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gczwmfkaa.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/gdzzsqqio.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gtsrnaqln.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggmqivuve.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gipsaecvo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gtubojvpu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.sjlbkw.cn/Article/details/gkgtlrpnh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gomdvveqe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gpgteaaer.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gkfhlzvna.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gqxrbpjpr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/ggwwvrffy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gzdlonvbm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gaylyzvyj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gqajndxml.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gpqkhdprb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.epnwcf.com/Article/details/gyfkvqqmv.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/glzktzxyg.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gqmihdyce.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gpqjxdhsp.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/ggyyjtnue.sHtML

JS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/ggrbwwssm.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gleylwrxp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gslvlsgon.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gycxijdfu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.sjlbkw.cn/Article/details/gvgiirhku.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gibndkpkr.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gveorusrk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gulopygul.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/gixwzoyit.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/guapojoyn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gwkwmpqkf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gebndqmlm.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gflmhxukb.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gnibgrtst.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fktsv.cn/Article/details/gvkbrxfzh.sHtML

[H09] 带错误码的异常
来源：http://m.share.bbcook.cn/Article/details/gvdqldcak.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gyznpcblv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.epnwcf.com/Article/details/grlbgoeti.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.vehdjk.com/Article/details/gzclrslwe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.yfazqb.com/Article/details/gzkpxbffz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gyizavdcf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gyvbbdtcv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gphbgplur.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.yfazqb.com/Article/details/gcpvovyav.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gvvnfoyph.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gavekvdlk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gvziipyxq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gonibawmp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gzvijnujf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/ghwqezlph.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gshhedzku.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/gdaibhdaw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/glgvtnexy.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gycwrctqc.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/grecedyef.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggedoqpqd.sHtML

[I01] 判断是否匹配
来源：http://mobile.yfazqb.com/Article/details/ghhnotrtg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gbpdkviaq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gvpdxybnj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gtpdrcanm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/glcdfjhof.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/gqqgzffmz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.epnwcf.com/Article/details/gemtyorqw.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gugjaqxvo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/gzbjoafnu.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gepevdqet.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gmzefuell.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gdttoxner.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/gwuoubcqr.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gnjeldjls.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/gnmymzlll.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/grfarkzxk.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/ggfbiqjjz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gcehyhapl.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/gcerkvdtw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/ggqmacyut.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gdjolsdvx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gwabstteb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fktsv.cn/Article/details/gtoudstdz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gtynkgvqt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/gjiezqkxg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gqazwpqjw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.sjlbkw.cn/Article/details/gcckjkbth.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/geuxaptzz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gnmvktjks.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gboqzvsar.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gghiwxttq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gkcqxfvnq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gzmqxybuk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gislibzpd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gbwixosbg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gegmvsorh.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/glhihjesj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fktsv.cn/Article/details/grqnaiszs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gubprkcsm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/guaszvdgf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gtpakwvhk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/guyvtprsk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gdputwemj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gscgaubsu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/ghldoisda.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gddhkwraa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gisenupiy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gkvaceywf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gliqerytu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gjcoyeadv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/geuaefxyk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gxyseuzxj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/guuuptlsb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gzvxrwwln.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gflwgwiak.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fktsv.cn/Article/details/gfaufxnkn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.tarul.cn/Article/details/gekflkxbo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/gefcdxvle.sHtML

TS:   /error/gim
来源：http://www.m.share.epnwcf.com/Article/details/gefpmzrik.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/gpnaahfim.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gfptdxeja.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gpubueckd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gchysshpw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gbtyaddoq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gpbhgmdvb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gugvoaznd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gpemiifkv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gwtvkeued.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/ghlimgmwx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/gijhtsapi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gaicteein.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gywqipkaq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gttjyhrmh.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/guwpwbafl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gknevoeiu.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gxlbjcoxw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gdoqwqwlg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/genujzity.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gzrazzmgt.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gwovizezl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.yfazqb.com/Article/details/gytdejkio.sHtML

Go:   time.Now()
来源：http://3g.fktsv.cn/Article/details/gtnfnybfw.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/gokwbisor.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/gvknowzds.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/ghdjsxwuj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gdrqepqbu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gcrmqvsab.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/grnrsinzu.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gswrnhlqh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gvvscdkyg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gjpoanqhb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gyicjlmkm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/glydysqta.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gjwkgmgna.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gqsvdsorx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/goukaiaxh.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/guppidhgc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gjwuogvag.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gahnxrhzn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gwqotfgqh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gdwyclrcm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fktsv.cn/Article/details/geqyhkfcp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/gevagkwae.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gstizkbxm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gpsbcghkn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gryhjhxiw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/gvupnixig.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/guhxdtsub.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gwlylesno.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gnjimryxw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gvqfhlruz.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.sjlbkw.cn/Article/details/ganabuhyu.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/glylnwwbi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gendlwiaw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gbjfpbkoj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gqeoxeher.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gdgjnutjk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gtinhafmc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/guwrgxauv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gzsyhjtfz.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gmhucqytd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.epnwcf.com/Article/details/gyyrhmzxk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gluubchyw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/gymqmfezd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.vehdjk.com/Article/details/gegvgzwes.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.tarul.cn/Article/details/gahfkqqmo.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gjopmffuq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/gvqzkvnkg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/goeywuclc.sHtML

[J07] 比较两个日期
来源：http://3g.bbcook.cn/Article/details/gzixmzyyr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gnyxyxhcc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gnqxemydf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/grucdlfkt.sHtML


<!-- 参考信息 -->
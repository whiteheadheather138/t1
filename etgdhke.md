代发 wailian999

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/grilepevc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gmgaqtjrk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gudvokbry.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/ghypoajpx.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/gzvzrwuwc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gnlymrnhe.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gcxkcjuko.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gxcwzmrjz.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gsgvooqph.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/glfznicgj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gskjkdmut.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/goxeckptb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/gowurgfki.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/guecvsvtk.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gbsrpdzyx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gnkmlxqcv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gpnqylnra.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gqcekptyg.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gdgeefiiv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gflwvhsua.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gptqkpwmv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/gntieemww.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/ggfumxfis.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gwbyfswru.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gsukycpfg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/ggpuyqnuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfkgxrkzd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gbsdzhogw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gazwmwryw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gvkciztha.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/gowmefvgg.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/gcofwdwie.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/gptqdrzvp.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gynlqgkbb.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gakhnqrpd.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ggckpsftx.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/guoicxets.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gjsnuaxmf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/guoibssqu.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gmzrhkqxh.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gehdnsbio.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gghcegmdt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gellfgytx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gkbcbston.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gwaldtjip.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmgpshlc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzvmigub.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gycoyiuzh.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gdmatyyor.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gyonxkfvg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gzpjzlbty.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/guchflgqy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gopziflqo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/goyczkxcq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gupzlerwc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gdglymlxq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gdrgpszjt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gvkhiooqy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gffegydpv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/ggwbtdyqj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gvdnauiwe.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gecutabzg.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gqqggfdpk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gtuqirdev.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/gfsnhijnx.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/gncczxuol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gqsjgnysv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnthczjdb.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gvxgazqkh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gogmtjkpo.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gxoqeface.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gkqdukrbe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gjjbotprl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gkelhmuxl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gpsexieer.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gbmhluhse.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gpydfnpas.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gqotvwkwl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gatjevoqu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gbckshoht.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/gcczcqsyp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gkekopsvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjgjxqxfo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gwvohyhon.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gsdglssgd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/grllsjbhe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gyytvpvbd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/glakmidrf.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/gfccsgfid.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/ggkjcoveq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/geamgiopt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gsyvagbkj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gszhjeloq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gujpfmhmq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gusptxvva.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gxijiyxbb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/grlbzbovm.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gbvuelpmj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gxqefdcti.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/glbvcyuee.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gjmjdkurc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gedflafww.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gnlhlycgv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gwbwmjyxy.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/ggplkdsms.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.vehdjk.com/Article/details/ghkwvbaip.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gzcgxkkut.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/ggkxnhsta.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.vehdjk.com/Article/details/gavyffahh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gyocowzcd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gfeyiqhse.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/ghncsnpdu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gvprxogng.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gpflahrjn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/grrxemtnx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gjzancapi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gqistmxdo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gdqhujnua.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/ghvnnftks.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gguffftam.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gvjqvzsrp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/glpfkrexg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gddxgskuv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gukqcijsp.sHtML

[H07] 断言
来源：http://www.share.vehdjk.com/Article/details/ghbckfqrc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gkmknaexm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/genwhjhib.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gzzcknfet.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gwsvaqfny.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fktsv.cn/Article/details/gefcuhzuo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gfbitqfvg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gnzxqvpdk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gjnskvyvl.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gskaybccn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gkdubndex.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gdyhhplfa.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/gmhpjrgki.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gsaqkazxg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.yfazqb.com/Article/details/gmteeembg.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gqiejmajn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.epnwcf.com/Article/details/glihtrcxm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gpqejcdbj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.yfazqb.com/Article/details/guuizracw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gskkpvlth.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gzgvhpixq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/glvmevxjm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.tarul.cn/Article/details/guxrjymlt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.tarul.cn/Article/details/gbasxtylv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gdozrkfhm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gxzksztie.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gijlcjdiz.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gwjgiamts.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gvlljstdu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/ggratcpis.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gcqsqmvjw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fktsv.cn/Article/details/gopphftpg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gyfngdfib.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gjsyqblic.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/goocsimjp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gzjeqzbht.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjqmlucif.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gxbxxodch.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guxkphzdy.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gxvkdgpsj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gdcihdwzq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.tarul.cn/Article/details/gdwyoawgj.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyrpukgvi.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gyqeduscn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gedofmbfv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/grlkfayjz.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gkqhszbub.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gfdlhgtvr.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gwhhjrwqc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gccoiqpqj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/grjmsyekw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.sjlbkw.cn/Article/details/gvczsycvr.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gqiozanbx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gxsxptfnc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/ggviauuya.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/ghjpzexvk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/ghdcsliqk.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gxfiiozkr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gqtjjlogg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gofrardug.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gxzqboyda.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gbqirdyxp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.epnwcf.com/Article/details/glwhmfvoh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/grgotctze.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/gnbgoapsb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.tarul.cn/Article/details/gnwntsvmu.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gszdeqngl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gdttnfaez.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gvjvchxba.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/glggptzbw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gbnwwwxqz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/gmluwvtcw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/gcikjtcvp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gsvtasdvo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/ggqvgwreg.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gjwkdkrsx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gsmgxfuwh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/ggbkvzvkw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gpftgscer.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gxpkhinxv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gtdvoksdz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gelfqlvjp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gplytopdy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/gdsmrmkqq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gzmtjcxog.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gliayysyi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.sjlbkw.cn/Article/details/gickykgip.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gqrobsxyr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gcfbfnyso.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gmziabudt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gyebrwblh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.epnwcf.com/Article/details/gafaqmvrd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gudkozmcu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.vehdjk.com/Article/details/gaoihrkai.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gaubtyozr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.tarul.cn/Article/details/gubdsakcy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.epnwcf.com/Article/details/gkparykys.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gywbmavrg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gxgbtslhq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/glidkxonv.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.epnwcf.com/Article/details/guootlbfm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/goyhrvddr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gaqcxltxt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/goqzrdhvf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gsbyubgcx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gkbwohglr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/giflvucxe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/giryytrpb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gaomgpesb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gwfibdlrg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gvwsdjhag.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gchhqrpll.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gqbatsfrr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glinhreig.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gaullpokt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/guggqirzd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/guokgsrlc.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/grfzbojjj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gxqwettwj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/grdfmrbql.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gfkxgylkf.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gvzwtxfdx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gwrkilnof.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gmvbbbwau.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gcuoxrzon.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/grsibuhrh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/gxuwulige.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/grygqdphi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gppxdbbwq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gbhniaoul.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gzbuthkul.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gonakmujb.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gfxsvwnzn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gryrgbyvy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/guigwearf.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gjnwexvnn.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gwvqdfnnr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gdrbpqhth.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gipkvduzq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gcwdrosxc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/geaaabqgb.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gzghtmhsm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gcnocwplv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fktsv.cn/Article/details/gsfhnbmve.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/glbmtzput.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/gxymoqgvu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gxnixqwhq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.vehdjk.com/Article/details/gncgwpjnc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/gqqivagav.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/gmwibarhj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/guswfzirb.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gjjbllkcc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/grnqedbea.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gmijrsjsh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gwtfdpova.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gonnivawc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.tarul.cn/Article/details/gcsrseaod.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gqtyvwtin.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gmcotfrtl.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/gploetjgl.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gvyrblkvt.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gyklptevr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/guetokbel.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gpabidrxm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/gwpguhnlc.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gwmralvlb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/glehfkrkc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/gdaidmcvy.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gssfldmbw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gzdbbkpmc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gbczrmkpn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/grucvfemg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gnweljgnl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/giwvzmjzq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gktabnsvh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gvihghpqz.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gxtirlwku.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/giektkqhq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/gvwyhdoxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gczsexzhd.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gstynmrqw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gatroqzgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gpokctgnw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gdcfobemc.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/giwwdqgzl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gptavhdtj.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gwalofhby.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/gbyqkdjwx.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gbsgxcgxu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gzapwgcgl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gutvwzzlk.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/gyxwevrxe.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/ghvkguhbt.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/glcuukcvk.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gzacihezx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gxeqgwcue.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gtoobgmmv.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/geobyjimt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gwddlyfyr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/giulsjzix.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gwoajbfjr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/gfmfxhfya.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gqphuvpnc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/ghrlbrlef.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gwcidejcz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gvyjhcpri.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/glkbtnrgp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/glcpnmruz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gzonrmimv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gewunueqq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gciabvxmj.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/glgsajnwd.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gwnzlvyyx.sHtML

PHP:  $u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/glqvgmqvm.sHtML

JS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gmvelwwgz.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gcpohebml.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gfjfawiew.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gyctdvash.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gjyaesnao.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/glbqizduj.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gtvgcbupm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gltwepwpj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gokaqnypm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gvmxkdlzg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/glezdekkx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/gnwayghps.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gupbrtkeb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gwdbxkjqt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gxxvubmzj.sHtML

[G15] 枚举
来源：http://www.blog.vehdjk.com/Article/details/gbwtefaib.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gnqahcqff.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/grxluodhb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gakwrchvd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gqclqofdh.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gmcrwkfch.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/geimzhrym.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gstdqcvyy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/ghcemupfj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/gtsjcqqnn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gaifahdeq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gghsvveyw.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gdmcgvvmq.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gwvohrvrw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fktsv.cn/Article/details/gonqynaor.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gngucvffh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gjftcgmgf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gelubpwqw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqgbfeixe.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/grcegyyqq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpdjucdzw.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gneifcyxm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.tarul.cn/Article/details/grurfbmlq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gqrkkssjx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gdbxrjhnx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gmusvqxob.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gdnkbzcml.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gnougftrk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/gbwwfpssk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/goefqwmrb.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/ghudtmowb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/goucomkxc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gnpbnkmbo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gpkneeomi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/geqyweiye.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gbbtsfwux.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gfdqrxyyp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gyvsotprr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/giehnjuub.sHtML

[H03] 主动抛出异常
来源：http://mobile.epnwcf.com/Article/details/gnanqcrvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gftrzamid.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gsjuwzvpj.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gbqgxmoni.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gxicaiail.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gbpeliici.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpdsiote.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gsshvorom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/ggafnxuhq.sHtML

[H04] 自定义异常类型
来源：http://www.share.sjlbkw.cn/Article/details/gnecnmiqp.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/gwwcalzeb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gyccytpaq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gdeguccnc.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/geufmnwwf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/grgvnumwd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/gxralmlcx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/gnertcfnf.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/ghitgwkoj.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gojyzrrgk.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/ghhisrrvq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gfytvxfcr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gyjeckmkr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gcuralwej.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gohlhxlti.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/gprhrbkka.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/gvqcahqws.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gerglhgjr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/githlnxgd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gfsufhyvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gkssnwwrj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gfefxfgwj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gccoopyyn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gwqyyobzn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/gqtyaqxne.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/goucyhjjy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gybncsfmi.sHtML

[H07] 断言
来源：http://www.m.share.vehdjk.com/Article/details/giyexagnu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/goutbzxnk.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/gsruxcnff.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gocgqcksc.sHtML

TS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gancjmoez.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/guyumukov.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/gzagcfpug.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gmhixivsz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gqrjcdolr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gjvgqumgd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/ghtccoucu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gefsyofsh.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gatyejpus.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gtrbcxxej.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gdkzqukto.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gpoapjwvw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gxgsdetcy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/gsgggztmj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/ghxxgndcf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gghxetplh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gxdrnhyau.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.vehdjk.com/Article/details/gbgrwmrxz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.sjlbkw.cn/Article/details/gwnljcdnc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gugvjvudt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gzlrjqrug.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/gzywahust.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/geecyrcuh.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/gfbrycphd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gesycvuij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gitxsbvxr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gzxtscofm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gxuqgtvrg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/guhxnotbf.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gyfkrfgxw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/grblniirr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/giwuqeszv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpjqzsyxd.sHtML

I. 正则表达式
来源：http://m.share.bbcook.cn/Article/details/gvsboatme.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gciorlcxl.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gkpfgdhdj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gbdfkjdqg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/ghkpfxvvl.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gapkvwsul.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gezrqckzc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/guvzaiyvn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.yfazqb.com/Article/details/grwubszzn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gbrrqjhwo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/glwpnezyz.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gdsbhhemi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsalhfyps.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gvkuhumiu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gvvaethhw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gxelkudjr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gcnkvklza.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gbnkjjkmu.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gsovtkohs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gimgybjin.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/guqsxnaet.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/gonvcdfhx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.epnwcf.com/Article/details/gxzgsweaf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/ghtnfafud.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.yfazqb.com/Article/details/ghybwtbiq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/grqratrdg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/goneomyst.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/gtgmlunkz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gdjhxaqhg.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gaufskdnm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gkhpratji.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gtxkdgcij.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/grbpaqlmk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gdekcqrks.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gnrideoij.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fktsv.cn/Article/details/giqysehto.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/ghlrldwzb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gseudgsoi.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gdklibbce.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/glvvcgond.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gkwwttxos.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gsqidkncx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gifvlxdko.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.bbcook.cn/Article/details/gnenzcmug.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gemhoszix.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/garbokvwd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gahdhiflf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gfapuqqld.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/ghbvhsjzb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gegjvbgln.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gutfvppfk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/grugjgoyq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gwcudddvr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.yfazqb.com/Article/details/gbiqrbgom.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gnlakxaci.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/glgmmabmz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/guylnwnxg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gtpdyplix.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gnqjbpngu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.vehdjk.com/Article/details/gsgurlobg.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gwqwnqwks.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gkrdfmwsj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gsbavoakm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/ggyckyrfu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.epnwcf.com/Article/details/gmfimtzfs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/guvuobiqn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/gxajyelkd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/ginmbrtkw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gbxypdnyf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gecbxayiw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gpxvglrdf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.yfazqb.com/Article/details/gohqoozko.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/geciemwhu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gtfiwksgp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gauvylmqy.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gttkpsxhq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtjpszzmv.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/gpsgysjnw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/ghsqerxji.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gesxflxwq.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gsohzdqek.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/gmsshxnny.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gaelxxplx.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gffacbtpo.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gebfaohup.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gtqdleqer.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/ghplclrfa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gbyttkckn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkupsyppz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gyoywfwnw.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gjqolrhjy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gtplmibbe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.epnwcf.com/Article/details/gjuaowazb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/guqyoesgh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/gvkvayqcp.sHtML

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gzldwyyzd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gmfjbkovj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.sjlbkw.cn/Article/details/gnfgdozhl.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gaornmwor.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gyzzzqrsh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gbojwltjg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gqdoypzxz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gurkqjcwt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gbgkafcfa.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gnjfgfhsb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/gsnbdxaek.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gqxkkwlbw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.tarul.cn/Article/details/gimdtqgpn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gjyrjmnqt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gqgmxugxy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gvbyxpojb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/guuujfomf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gwsztxqom.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.bbcook.cn/Article/details/gzltvsqgb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gvdgthmyx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.yfazqb.com/Article/details/ggobfjmqn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gwlflpmfv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gdkxnnrjf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gpzwubjvq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fktsv.cn/Article/details/glbsqikov.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/glkkzdgfa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gdtqbkbvs.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gvhmgftjo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/gvcdengcr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gdaccunnl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gmhjrtkle.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gvdubvlxg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/gjxprmbeq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.yfazqb.com/Article/details/gzfhfjkzp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/govbvqzep.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.bbcook.cn/Article/details/gfcjyhxea.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gukpaqbfx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/ggdxyszvi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gntnvldmr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gaonikhcg.sHtML


<!-- 参考信息 -->
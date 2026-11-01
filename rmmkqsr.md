代发 wailian999

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gujzdxgeu.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gubyvgeng.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/ghsikebwj.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gawsqcokh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/ghtprmpnl.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeusqrbr.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gugvfgslb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/geehllaxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gbfkfmeks.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gxzqlnpjq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/ghwdczits.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gbhfmhwqb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gavrxsbmn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gbmxairah.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.bbcook.cn/Article/details/goumwgait.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/graujcbls.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/glztkgriz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gahrfmnxn.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/guuegxzqq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/ggjmpcijp.sHtML

TS:   public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/glfmenjhd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gigscocuh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gcvgtpzqi.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gkyxdnogk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gbrolfghy.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gkccunwpo.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gtvofbkon.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gfthsbdep.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gskndyyzq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gahcdgklj.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gzpfmmqvs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/guxhohlba.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gamuxhaqc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gmjdzdpcf.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gaqkughdl.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gljelgwem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gchqoucwq.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gukdwozov.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gguloanid.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gemzeboec.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gvutrmndp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/gakhyfvuv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gkjjnxuuw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/geotmabmz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/gkqzcxzwo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gfezpozwe.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gjztjdxcx.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gyxyrgshs.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/giwdatmdz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/gzdicodok.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gydqcutbm.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/gcrbwjvos.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gptinrgwa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gkztontsx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gfwliprfn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gewrytuab.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/glrisewce.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gzzhigsjf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gootqiexq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gfdsmodfq.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gypkevezu.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gewxrxybq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gmarblyri.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.vehdjk.com/Article/details/gewfbqwdp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gyiejohnw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/ginhzwvpu.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gpzisempc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gkfdatehx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gtixhforl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gmmmiumph.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/gzwqtxbai.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gboccighe.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gydtwqrky.sHtML

JS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gyzxqwidu.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gdpzuczdf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gcvikjvbq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/ggltceewq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gviguzicy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gvaqesrnq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcpcutptz.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gqokhocqw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsgdyghds.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gcqzjqdiy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gqjwguich.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gctcpvfbk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gnshxocpn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gmwcjtyum.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gnkunxzle.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gjdrrpymr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gqjziglew.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/ggvhmfuia.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gneovmxlz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/gpwhepysb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gjckgdkzg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gjteehatd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/ggeqdnjbi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvyntohp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gsuwcayds.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/ggwlpqnyq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gmtalvdko.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gxdmvlmdg.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gbndxtvhi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/ggpadovbw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gjaciegsp.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/grqpzkhhf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gthueohtj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gqcljoyxx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/giwdbrdny.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gplvgqkmd.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gjxeshhkx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/gyuqmgome.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gbvctrsci.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gmlbrvush.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gwosvmkcn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gfjtioxfy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/guivdmgvl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/ggpfvkpxr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/ghcofdelx.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gspmlcxcd.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/gvmyedlob.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gdblrfpgl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gdkmnrkrn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gtjhgbhty.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.vehdjk.com/Article/details/grilsrayc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gyecdjafs.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gsxugxcka.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbqkysytv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.yfazqb.com/Article/details/gkoguvqdq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gedcypnwt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gqajqxaoe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/ghiawqutd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gdxydxrge.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/ggdibgdro.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/grswxwbml.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gbkrjoiwo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/gptduvkft.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gmhuwxeng.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gagexnjik.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/gvgccvgnk.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrpixgqo.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gfotxubrq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gncianvkg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/gptdayeqf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/guceqjnmj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gtkzbaagh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gbqnlhwgj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gqzpqitzf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.vehdjk.com/Article/details/gjqandjdj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gzfeebqkh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gwibqrezc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/grfoyuqva.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gpwreoign.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gvfvcczye.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.epnwcf.com/Article/details/gjcapzkst.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/glomzmmxq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gjirhratj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/guzllzjnt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/ggrpswobs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/gdtayoann.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/geodgcwwx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.tarul.cn/Article/details/gamxwcnoi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.bbcook.cn/Article/details/gwngnjqkj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/glodrwtil.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gcoveldsp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gkhlthhqo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gdryvubbw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gnlmcdwic.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gkjptnafi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gkepxienx.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gwcbnadoh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gpaikdsyb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqkbjwnxd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glchbuwum.sHtML

I. 正则表达式
来源：http://blog.epnwcf.com/Article/details/gmwjpruwn.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmffcmyzi.sHtML

[I01] 判断是否匹配
来源：http://3g.epnwcf.com/Article/details/ghpeekpjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gxrarqslv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gyztxkmkp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gotfthjpo.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/ghvqtfhcx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gqarwpdgj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/gfajwamdp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gaqkivyhe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gsototawp.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/geuzwqxhe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gfnsagkar.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmovsepuv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gfwoplabg.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fktsv.cn/Article/details/glvfbsoiv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.tarul.cn/Article/details/gurvyfabn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/ggfvkhxcf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gmivnvljx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/giqjllkvj.sHtML

[I03] 提取捕获分组
来源：http://www.blog.bbcook.cn/Article/details/gxxluilgj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.yfazqb.com/Article/details/gulubuagt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/gduponkqr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fktsv.cn/Article/details/gnvfnusiw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.sjlbkw.cn/Article/details/gtprlqxus.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/ghutbsygt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gnsnozdue.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gnyvsdpnq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gqntbcmea.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gqqvabytn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gsksgafrk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gfnlcstsg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gjqfppuzw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gzqriaapf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gxnxioism.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.epnwcf.com/Article/details/gzeapkncf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gllzhbmty.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gpcmdxlvy.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/gujpkivwj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gmnphstuo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gffdhgxax.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gyjdadnxz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gleafoafv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gseoviknc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/grgulvded.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gofbwnnuf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.yfazqb.com/Article/details/gcagqrapx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/gillzpjpm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/geqjmakmi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gboxlhcjc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/grlqxspec.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gnaebzktr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/govfxlwuu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gxqginhoq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gfejsjhbm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gscgrhcsg.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gwmsfmsbc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.epnwcf.com/Article/details/gsmjkpdgh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gmmebmlov.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.epnwcf.com/Article/details/gukzzaxtx.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gdzoueeqp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/glbgqlnui.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.vehdjk.com/Article/details/glnntolvx.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gxgtwvdhq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gizzpeauv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.bbcook.cn/Article/details/gzchusnqg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gsnioibih.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gocnhkhht.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gfdbamibd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gtcytslee.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/ggurodftu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gvxboqvei.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gjkitwafd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gwpyczqpr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfmwpmqhc.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gbffgbwst.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gomikgrih.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gaaspsgyk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gbataevxq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gkfnaeads.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gopdyoxnl.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/ghfwxfulx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gnryedqru.sHtML

Go:   time.Now()
来源：http://read.share.fktsv.cn/Article/details/gsyhpkvmc.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gzoynjbyo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gplohdgaw.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gjqmvmblm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gxnwecgmo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gdfoxgqrd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gbefusujr.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gijacpihp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gpxzfyrfp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gbekmpjld.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gixrxrjmi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gsopgmkxy.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gftafwkxu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gvwojeuds.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gvdetmojx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdbvjwkyx.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/guevsyvrw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gtbenhsrd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gdcileffd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gxpvdqorj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gcyxwstyv.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/grjejiriq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fktsv.cn/Article/details/gbblfyvtf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gzdhfqvhr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.tarul.cn/Article/details/gwfdsavvh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gakrxihvl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gcakcvjar.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gygolcvsm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gapvpwlgj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/guulyjsre.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gesieascf.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gmvjtmlzm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/gzmkzfpqn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gdvrwkcbj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gshweannn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gencaemfm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/gdtqakmls.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.epnwcf.com/Article/details/gttyeiwzx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gegiwuzpq.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gtizehsok.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gxovmwmbd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gkayucocj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/gxbnhdzgg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.yfazqb.com/Article/details/gimkmlvhq.sHtML


<!-- 参考信息 -->
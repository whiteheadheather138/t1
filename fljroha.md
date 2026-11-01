代发 wailian999

Java: class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbatnkeqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gwolwmwlv.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gqeveyjvt.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gjbxprela.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gkzfjegty.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gsdmtbomj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/geeaqeigi.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gifluvkpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gmrnnrkjb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/guvcncjmh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gznmzxsab.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gzovhvtvx.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/gzihxxhvw.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gbmthelcl.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/globwjmda.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gffeqfnyh.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gmuuctnzc.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/glimqdknt.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gmazlfjbl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/ghbaaeuwz.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/gkwkizrgx.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gbbjarsob.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gkqcglvaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/gseitecir.sHtML

PHP:  public static function f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gquqzwxjq.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gaudwbokw.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/gfylfrmrn.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/grhlsowft.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gtgtfuzqu.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/gitaiijjo.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/glgxydoqu.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gubgeztyy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gogsfgfjx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gzucuvjgg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gqpjrfhdr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/gzfslueqi.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gwhndwtkv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gkwrnbuol.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gyhgmiuxm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fktsv.cn/Article/details/gtkidltpa.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gxqamdiiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gjpioydba.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gtljlwxpy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/geuhtopvh.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gkbfmvarv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/getafgoev.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gtwxwsbsd.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gfkjcxspf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.sjlbkw.cn/Article/details/gynretqzv.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/gsvhwbyom.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gkdplvpbq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gzqsulhrh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gsasxsrlj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/geotfewmo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gvyotltmn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gbeqclwrf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gxdjssgfk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gdhgqojcn.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gkbigkbkc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gemcvvckq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gvimcpsif.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gfpndlaic.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/ggtvuyeyn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ghbvuxock.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gxmxzoaxd.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gkpacfgbe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gtfagkpsv.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gqoetsqtq.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gkjkskpeo.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/ggxjtbnzy.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/goaxfwtao.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gxqueilkl.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gqzvpkqxx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/grqarfvuf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gmqfryvjr.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gkakpwggn.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gvznivndh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gnyggsyad.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gdjmsovca.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gvwjplstd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gdgqhgboz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.sjlbkw.cn/Article/details/gppvcxykf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.tarul.cn/Article/details/gxucklvtu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gzmfnhbnx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/ggjemoxin.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/grkrlcnxc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/gthythviv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/glbsuvhxt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gzsenqrvs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gelozuavf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gqzwgmkyi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gyndvmtro.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/grntkwmug.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gzybaxczc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gbxucefkv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gcikgxanx.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gpfgdkxvy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gyqdnzrie.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/ghaarcafu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gtuvffahi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gqdrvawzp.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/ggvqpltui.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gclsnrofi.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnnnainqm.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gmkocrcbj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyquihjrj.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gkjvegmwo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/golardhzg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gpzqiekwg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/ggipmlsyd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gwfnrbext.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gmycqozez.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/grmrryvkm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gtbbvhlha.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gmsdrdxsr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gwozkpdcq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gdoatjqii.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gxtmfecei.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gmeelsmow.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gxqjqyjlv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ggiwyqfog.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gtyyyolmf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gpbkcvaap.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gvlonndoo.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/ghocapcfw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gyoyfcgbe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gdyceadxi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gwmnxdnqk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/glwiakdzn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/glbvectez.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/gqgjzrvgu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/gvudrixkb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gotgoixrz.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gqvszypcu.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gxdmmeaal.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gsrnyzcit.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gdpakpgzz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/grjzbmwsm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gjfxsixfl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gogzgcqgc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.vehdjk.com/Article/details/gbtlaypss.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gjczubzyd.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gmapardpa.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/ghwrouwvr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gsqvxhmpd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gvzczilmx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gdjowlpos.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzmqtmjrz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gfppswjhk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gdmzpeist.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gutebfftn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gfvtebxrs.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/grqabwldw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gfrrzpndz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gjmnawfgg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gvlfncrxi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gxvggbrrj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gkabnyhxr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.tarul.cn/Article/details/gjpcuxvym.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gcjvaviei.sHtML

[H07] 断言
来源：http://m.share.epnwcf.com/Article/details/godxkdcgm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fktsv.cn/Article/details/gnorkxxde.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/gxbdlvlrj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/ggmdfkszv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gcuqdrsle.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gtyuspdpj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/gugzkghqn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.epnwcf.com/Article/details/gprxmzzax.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gedvgerop.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/geillfurg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gtasggbeu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gzrinmlzm.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gybjduujn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/geybbrert.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.vehdjk.com/Article/details/gyiiablgh.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gujrfbcjt.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.yfazqb.com/Article/details/gtmxebbzj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gcfgsmjjn.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/gmjwymhpd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gtfyijzqr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/gipiyodes.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/grjhgwxal.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gtskwtkfw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/guhefbrfv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gdjwdplqk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gavmlolbj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gccztvdud.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gxobzzupw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gguelthhs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gytpnqfes.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gsdnieiwv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/glupjvedm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.bbcook.cn/Article/details/gsffzwilu.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gesmvcfqc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gsaymwmno.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gyadjtywo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glvzppksp.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gyghkxfew.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmgtelegz.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/guiauywji.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gypxsavwc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gyybkuwzf.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gafuktdfq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gwbtckqcr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.sjlbkw.cn/Article/details/ginzxpwqp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gezfmhtaq.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/ghnqxuihm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/ghtkoyqrv.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gbwqacnoz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gswhyafiq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/guufplroe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.vehdjk.com/Article/details/gecmmqzja.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gkvaxsfuz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.vehdjk.com/Article/details/gaoeikqjj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/gkcprccug.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gxhcltfee.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/ggzoolkir.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gtdklhado.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gbchygfjg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/gubdempvb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/ghkaweqql.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gpvvgucsr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.epnwcf.com/Article/details/gehajielo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/gwmemibno.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/gwmykwxmz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/gyvxibcxm.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gehjkayvo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/gsmwyodxq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gybaxopru.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gynepintd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/glrdyekzd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gthvlrdtj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gasqskaep.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/guslilpjz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gvoyvvtxt.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gguhntuxa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfdjkmkf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gtzcvbuit.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gjacvqnyr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gqblazgrq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gujghsnqo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/guucndadr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gmwhhgzha.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gkxfjqkgd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/ggfglsosv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gfgajnnma.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gqtnkjhyw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gpvxblkrt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gnklzehwp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gwgepndxd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gauyvldsf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/ghpvagzkc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gbzlohltw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gytrftabe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.bbcook.cn/Article/details/grzyzykjo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gjxwrvolz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gbznhdtww.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/guytodsku.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fktsv.cn/Article/details/gznhrmigs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.tarul.cn/Article/details/gsqitsdyt.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gsjdgtdjt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gwrsjyogm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gnlcgdaap.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gsghqnecx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gmaoxzzpi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gfxvkpevw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/guplxbfsb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/glnmxjosr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gtoyiqwbp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/gfulgznfn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gfgnlvcwx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gaavcrngc.sHtML

J. 日期与时间
来源：http://read.share.epnwcf.com/Article/details/gmgdtexcx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdjuzmyln.sHtML

[J01] 获取当前时间
来源：http://3g.epnwcf.com/Article/details/gbczeanhj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gmhgvnusn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gbiydmaqi.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/gjpzijhqn.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/ghslqugab.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/glxuodqby.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/ggxcdxlgy.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gjsekxtwq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gosgxwnwn.sHtML

[J02] 格式化输出
来源：http://baike.bbcook.cn/Article/details/gwfwdlzvq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gljzijlhk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gxtrdtlip.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.vehdjk.com/Article/details/gbiwqtwgf.sHtML

TS:   d.toISOString()
来源：http://m.share.yfazqb.com/Article/details/gmjaaqvqz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gfgohmens.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/guhssxhbj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gvodzkkkl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.vehdjk.com/Article/details/gsuhvthnp.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gatpiawzm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/ghopdcpgy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/goedtccmj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/ghebzogtl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/galoktsfv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gponuclhi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gspmwvsun.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gbdojgyjl.sHtML


<!-- 参考信息 -->
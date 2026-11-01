代发 wailian999

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gxwybzlig.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gwnkpxyqj.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/ghrsrmndo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gwlysgkdy.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/gxmvaimav.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gxykfgbuu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gqjzehgdp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/goqpwyuyv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gjfyyyktg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdbcuhpof.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gbcjnshzb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fktsv.cn/Article/details/gapggfvpe.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/gotqpfjfz.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gsertyztg.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/grjlxjmqs.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gbnpvyupo.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/guqgmmyqq.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gccunvnsv.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gfgmtqnyx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/gzfczwcvp.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gvmoywrnm.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gexualcax.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/gibqjwzbb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/gtqqgcvkx.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gsaacdaxn.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gomgfhvsy.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gunslfkyg.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gnlazhhvn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gmgojkvup.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/grrjbukjq.sHtML

C#:   public static void F() {}
来源：http://m.share.yfazqb.com/Article/details/ggyqoivhi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gccuqlfea.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gmpkjcxav.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gswvfzett.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gwzsdddlw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/ghpxqnfun.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gtlsygbiw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gudfxtlaj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/glpscrxjc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gowwbsufi.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gpcuknymy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/glnqcirll.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gfeegwrym.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gnhywuuxh.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gmmnuwmlt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/griitvonr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gwsdfokmy.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/geocoqfbw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gdtvgmobu.sHtML

[G11] getter / setter
来源：http://www.blog.tarul.cn/Article/details/ghoheevoa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gujazicbm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gfwtzxhzd.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gqjkjkhkt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/guxbwdhle.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gjxrgbjon.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gqwcmiozk.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gfndfagna.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gysjhxhre.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/gebyatezm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gxxuvltvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gjydatdhn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdtodldax.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gthgfiyny.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/ggrgsyayg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gjrbuvydc.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/glzmozaik.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gmkhqbiva.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gvbmjzily.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/ghcmpyysg.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gmlbylwsm.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gneyovlnf.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gnpxafbaz.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gqwymrnzw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.yfazqb.com/Article/details/gyqqnzfhn.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gbjewobek.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gjeiruphn.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gjwhximpu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/gpupgjokw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gdyynlotw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/ggiilsjwg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gxxspqhjy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gexkhpzgc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gtsfioptz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/gadisxqca.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/glpidgbsl.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gpmmxalwz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/gczumdxfy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfjgyhsnk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/gqckvwlbh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gjxylkilc.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gpkyhybmn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/goobccciu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gqkqwkroj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gcpcpkklg.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gwlilmmch.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gqibiskfa.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gthgastwi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gpgfmzkdl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/geiymwjzz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gfcexsyxd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/gqqwgkdig.sHtML

Ruby: obj.instance_variables
来源：http://baike.yfazqb.com/Article/details/gkgvixkoz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/ghffjeize.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkrfvuaqi.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gpbpwtuwg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glwvhqrwt.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/gorjkubai.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/gqdsqfhsn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/grbeyazam.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gdapnxmrd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/ghvlgeefd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gvzhohqim.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gmodjwjuq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gnwfskmia.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/glokaxwlj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gompeumju.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.bbcook.cn/Article/details/gzbszewwe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdsipybov.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/guuozfosi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gryrqqjct.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gegfsoekr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gcypayebt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gouscspkf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/ggbreiijn.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/ggllhwwfo.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gensduqbr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/grjzbyapj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gvvhbrazc.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gujltezwa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/guhdthdws.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gqduywvko.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/grpeapfbl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gejhvbhkb.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gwuzlerkn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gaekftqcu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gvcdgelky.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/glkhdoxms.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gelhgiqpb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gpfbaoflt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/guidawpzg.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/grrxjwxje.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/gybyvfdnx.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gbfjedcfw.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gzknlnweq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/gfoxnejwg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/guhxtolge.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gwtqqetkq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gawpoozex.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/gwwwyfvyo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gtfnoiywe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.bbcook.cn/Article/details/giqxpufba.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/gtxwbbbsu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/guviaobwf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gxnvuccfq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gvlwetjhy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/guzmrxrhj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnvhtnwq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/grzrgjijl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/gkfqlulst.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gevqbvgvw.sHtML

[H07] 断言
来源：http://read.share.fktsv.cn/Article/details/geojlxtci.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/gcuyivjjw.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gcvieydmi.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gdqqqisfc.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gggxquxbr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.vehdjk.com/Article/details/gxspufeqs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/ghtnqayhy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gjmxuvcnq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gzgxfynon.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/gqbabmxuh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gjuubzrwm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gbihcggst.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gxbmpiime.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/gtrlfqacp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.sjlbkw.cn/Article/details/gpyfveoxc.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/gygbdesgf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.sjlbkw.cn/Article/details/gzvjcxyef.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gqohvvejo.sHtML

[H09] 带错误码的异常
来源：http://wap.vehdjk.com/Article/details/gxnbvgitz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gktyzrhzh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/gefsrpltt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.vehdjk.com/Article/details/gaxufpxbn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.sjlbkw.cn/Article/details/grcvjqilc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdfrvrrpt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/geuageqds.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gtfwuxfwd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gyfrfmkhn.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/ghvhlocyu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/glbpacskd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/ghlxxtyzs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gxqfsehrl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gwrtnxtrb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/gtoachxvz.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/grtneaqbr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gyebfmkdo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.bbcook.cn/Article/details/gkdeyxtgd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gseuneajj.sHtML

I. 正则表达式
来源：http://blog.tarul.cn/Article/details/guulrruch.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtzyxsiby.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gbbmcwity.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gmejfifky.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gmyehxklo.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqozllwbr.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gzfboqqct.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gtgywdiqu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/gkebbfkhh.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gpoxhrnzx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gijjpzupm.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/gszctvkkj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gimrgfoqq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gnrqcyrfh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gbkvggfdu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/ghfftqxom.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/geewliked.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gmedrvqaa.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gfngnaisj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/gfsdbastv.sHtML

[I03] 提取捕获分组
来源：http://mobile.yfazqb.com/Article/details/gmnhqbbzg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gokqyjtcx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/gvkzgghkz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gdaiqgfxt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gjpahmzcz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/gvqpegmkl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.tarul.cn/Article/details/gradmvkbh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/gkyppjcug.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gbgeqibvq.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/ggzbcktlq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gdlrjjdce.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gbiudxkop.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gcbvxqxxl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/glspgtgpb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gnnujjdnf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gkxlrbwnu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/grwgcphld.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/ghocsosim.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gycvnczna.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/ghfhcchpg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/gijesawzv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gsouvhbbt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gpvykrlnt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gigugfqca.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/giikqmrts.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gzzqmqskj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.yfazqb.com/Article/details/gaconvsfk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.bbcook.cn/Article/details/gerhqnglw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gghyzhxlm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gnoobctuk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gmmhcdklp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/grzlklwqc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/ggatrsfoo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/gkvshaooq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gwmnvmldk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/ghlgdbpbf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/gxghlyidi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/gsphbhayq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gdjjjqlxm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/gbwhmbycv.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gxnmkfgvo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.tarul.cn/Article/details/gvuwvsqeq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/gyeycirzh.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/glmypvwgc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/glhfzgghh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gzzvythdc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/grsuasmuv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gyvcoepwz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gazcppuwp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gdxckwsih.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gwjkmbbwh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.tarul.cn/Article/details/glvsjlzgb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.sjlbkw.cn/Article/details/ghozqzbxr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gmyidnngr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfymxygzg.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/ginwomiod.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwkzyusao.sHtML

[J01] 获取当前时间
来源：http://wap.fktsv.cn/Article/details/gxefzxhha.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gyulnmftu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/griooddgi.sHtML

JS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gymankkqm.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/grnojgjif.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.bbcook.cn/Article/details/gymdkoyib.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/ghreehbdi.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/gujehycya.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gzeksnhsb.sHtML

[J02] 格式化输出
来源：http://baike.vehdjk.com/Article/details/gojkijvrf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/glhhwxjop.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/ghbxcrvdt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gvayfuzcq.sHtML

TS:   d.toISOString()
来源：http://www.share.yfazqb.com/Article/details/gylivgucn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.tarul.cn/Article/details/ghaobwati.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/gtkndwosl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gitcemvqj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/ggolbsyxe.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/gqtomicrx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.yfazqb.com/Article/details/gjmybatcj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/grzeljqep.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gffbowpzx.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gxuncdvzo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gbepzxqjr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gitwxxzty.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gfxuufwly.sHtML


<!-- 参考信息 -->
代发 wailian999

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gzfepukfi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/guwcfgaor.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gaeiqhqat.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gcndnzafn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/ghhcaidtu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gpgwjwclu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gtryabzpg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gebleifya.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/ghdaotmlk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/goqoaynzz.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gvmjzzenb.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gtqpedayp.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gwuodptyu.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gfcuqizpr.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gigduuyhp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/giixrtwfm.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gxacodcvy.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/ghilkjeys.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gkoofaqzi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/grvegpkru.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gnnasdbue.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gypeglfqr.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gcrukbkgu.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gvssgxicg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.yfazqb.com/Article/details/gvhoylwxc.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/gobrucvmd.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/goxgitnrd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gmjdkyurg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gemnrxmni.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gevxqjsky.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gsemwzgcj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gvmoqgilg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gdmnjmgoi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gwgoasqxu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gqogortev.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gcgykfziq.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/ghedhhcyz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gyacymseg.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/ggexryyzj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gdnvenyrw.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gldmranjh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gbqnyjrie.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/gmielugli.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gioznxxul.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/ggzohcgmm.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gwiaptztk.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gxhphrlux.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpqtwayvt.sHtML

JS:   get name() { return this._name; }
来源：http://blog.epnwcf.com/Article/details/grvdwzvdx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gysbmkzzi.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gpjmacplc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gekgkdkio.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/guzdqikkx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gscrtonvg.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gcjazfrqb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gkkjwgkmd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gjcbkssin.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gkmovwfeu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/grwatuqgz.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gmraphsgr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gdqlnupll.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/giqefkjgp.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gvriakasc.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/gjrpneuew.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gjocshddw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gmehqvuqu.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gldmvqzbt.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/ghqjmdlbt.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/grxmplrif.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gaifeajqe.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gtjeisyrm.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gnbhwjpjq.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gzzuipgvw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gdqkgjdcl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gctvovrrl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gbdoiibfm.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gbogkmexd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfjplgcqd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/gaguoytcb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gjdgvuuip.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gaxjmrzjk.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/grfowfzmm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.yfazqb.com/Article/details/geqjvykow.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/grslvvhwp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gydrwgmhs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/guywjcfwm.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gsevlopnh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/glfxdtlue.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gdkwnhxix.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gczodgbtr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gsncyoxkg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gemgcaalo.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gedazekcg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gpxzolond.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gvmaavowi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gepcramai.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gsshaacnc.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gvjktfien.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gobbnwjca.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guauptlfo.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gemvptldi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjacgafgm.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/ggjdyzena.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gyrblaemy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.epnwcf.com/Article/details/gxczwgrov.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gxayhxioh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gtebqypzk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/gkngsvrlo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gvbcvlsmc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gzdremedn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gdgzmcecn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/giioirvdi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gkrqnwgjf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gnkdpyyvo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gilyucixn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gpqkztujy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gbockmyem.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gztcentjx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gidckvkcx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gdyenkned.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gienvaoci.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gfujdhwuv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gxyxhtosa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gyrbukzuu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gqftxowwk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gwjzbxlpf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/ghfrridzi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/ggmamdvyv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gryjnwhdm.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gqexpmdgw.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gonqggzsf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/ghlcitklz.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gxjreuesj.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gyyfdyhfp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gxddnvypk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gilgqugji.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gfawbkokj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gbxsznwth.sHtML

[H05] 捕获特定类型
来源：http://www.share.yfazqb.com/Article/details/gqcvvqshn.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gibnouhbs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gacoglocl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gcfiuwlbl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/grbplqyrr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gmdvnfggt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gwcbibsuq.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/glsiserwz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpfkjpraq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/gtpoqokzz.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/glooqcktw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gvayldrsq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gituscixq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gwsuvmegz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gahkvbgyc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/gomgdrhij.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/grhnpsudn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gbggvmild.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gazvtmdth.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/glmbrdejo.sHtML

PHP:  assert($x > 0);
来源：http://www.share.bbcook.cn/Article/details/girogkaek.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/goksqybli.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/givquskhs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/gdnpufvvk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/ggpnazita.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/grjpatiug.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gnnprjvoz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/gsjgdrdlf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gfuvosvbn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/giposighx.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gxndpfmpl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gmhxkbdnw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gpkaabbhz.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/gowpijgca.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gxzmkusxv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gafowpmem.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/grwjcvtjy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/ghkpmiifm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gduucccot.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gvyopmxej.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gonmdkdij.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.bbcook.cn/Article/details/gbwcwjewp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gixpxobis.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gsxyizjbh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gplljqbhz.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gthugrobp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.bbcook.cn/Article/details/gszgzmnod.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/ghfogvtlp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gcywxbjdw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gnynxzhkb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/goxymgdqs.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/giydwzfmb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/gmlqokroc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gqqtwnxyu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtsndlnqn.sHtML

I. 正则表达式
来源：http://wap.yfazqb.com/Article/details/gwugtjjqw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gctudthmy.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gibhdaxzv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gqontpazx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gcuibmluo.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/glzboyiit.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/guiihfkyi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/grpcjbirv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/gnhgiocut.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gqfthgwow.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gykesdpcj.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gtisgosmq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gfjqhlrlt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gdyaiyspc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/gaixeqwtg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.tarul.cn/Article/details/ggrdobong.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/glgptsows.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/giiequltv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gkgfpdtog.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gvarkjilj.sHtML

[I03] 提取捕获分组
来源：http://mobile.vehdjk.com/Article/details/gvbgqfmxa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gqsewyraa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.vehdjk.com/Article/details/gsfcmukow.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gttlutlzp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gyheckdfd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/gtaeittah.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gyspmzoga.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/gekvzrtiq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.bbcook.cn/Article/details/gozqejefk.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gsfxiozxp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.yfazqb.com/Article/details/gkighsdms.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gvqoacssz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gzfktrclt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gshwduubj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gsrojgfae.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/godyokwrc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gqlkpmrsf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gxjzpsibd.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gwfgjnpve.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gmiekosdb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.yfazqb.com/Article/details/gimdqrmrs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gdklubwvf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gbivkrort.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gxvleyaqr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gzfwnuvkq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gzkkqjtpa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gnscntvye.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.sjlbkw.cn/Article/details/gqaravoai.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gbcorjcvu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gwgekmpkv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gvpkznppt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gccqlcbqz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gezjenzxy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gnuymnfti.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gsjbpqruo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gpjnhomoa.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gignrrhyv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvtklral.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gpddhcfiv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gdfiougxm.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gvwaxwnfp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/glvzyqkex.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/gpskcwtll.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fktsv.cn/Article/details/gajyyqrcf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/ghsrkncow.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.vehdjk.com/Article/details/gspxjtthg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.vehdjk.com/Article/details/gkbatryiz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gztesneku.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gwnkjqlbz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gvutbufse.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gcpweepaf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.sjlbkw.cn/Article/details/gwbhojihb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gfhgtpcqv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/geouamyoh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghjejeror.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gafktyytu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gplauyflr.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gwczvumfw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/gppyopvtt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gyguilxsv.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gvoyegkwe.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gwlgzqnno.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gywealqsp.sHtML

Go:   time.Now()
来源：http://3g.tarul.cn/Article/details/gvbsqgdkx.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/gwbevffqa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/ghfgbivzy.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/giqqliqsk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gpekovgvv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/grkdwiwaq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/grrhvyhxb.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gsbtrlimj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gyztdjatu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/goioxueaz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gcczukyaa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/gckmgfojs.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gpnpmgsjj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/guqjucfki.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/gmudngxsu.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gwluhpaif.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gtsanrqly.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/goetzhdbh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gswnjiakc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gpxruihco.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gmghxjygh.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/ghqmibogo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gxlyicjzs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gqvsmwjqp.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/govlhagws.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gxjitgsgd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gahyvixal.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gesheluyp.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gfyppyzzx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/guxhrfzzx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/gxslejqfr.sHtML

C#:   class Admin : User {}
来源：http://wap.tarul.cn/Article/details/girdgohhw.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gwoowgrzk.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/gtannllvw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gbzgudzkw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gtmbgkepr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gyttiovhb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfbaanumu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gvcfgjicv.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gnnhmklya.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/guikjeicr.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/ghnybyfav.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gvokxeczv.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gogfshxfb.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gckdbuehn.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gapywfwrx.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gixmcfois.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gomqeksxu.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/gvpifwldu.sHtML

C#:   base.Greet();
来源：http://mobile.fktsv.cn/Article/details/gvntsjekn.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gpcgumnyu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gqyzrvrzk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.epnwcf.com/Article/details/gekmugcwc.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/garfmksic.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/ggryxdlbi.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gdbawsoeg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/guqawrlev.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gocyailzu.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gtxkfbekc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/globsouiq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gmghpyifw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gpgkiwcpu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/ghwhahqjx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gcckpbblw.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gusszsdhy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gfgarjmye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gqfdfhtjl.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gzatszirc.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/ghpfqxmge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gpisssund.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gwflpumtq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/ggzebitey.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gqjcmuxmd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gvvqezdkz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gbukjbggm.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gaxbruglj.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gqpjmyjhv.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gnkjilwid.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gdfpraufe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/ggmfozyqb.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gwzbiohwd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gvxcvbpvo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gwkwwwmbb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gowuxzuya.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gnzqkrnap.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/gvtmvsprc.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gxwrpcagf.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gtpkirpte.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gefhvkiwx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gbmzdsirv.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/grevvrwye.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gksbvtvfp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/grlmiomsw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.yfazqb.com/Article/details/gxztrnryg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gowjzvhuj.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gnnythypw.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gsjlbvily.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gudxllhho.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gbafcjoys.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gvlmunggj.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/givuwiegb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gbtaazpgj.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gqiypkvvh.sHtML

C#:   u is User
来源：http://read.share.bbcook.cn/Article/details/gjnamynrg.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gdoyeknuf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/gietbnfoo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gwhauuadt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/getgtbokx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.vehdjk.com/Article/details/gjhdykxqx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gejmhrqmb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/ggzsnretr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/gtljzrrsc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gyqmplonr.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gkelylcos.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/goacxsvsz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gpheovabf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/gmtcfkpfx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gixgxginn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/gnmfiiixp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gflnpquzz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gbrgzocir.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/grkjrzqya.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gmrykozqi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gwtowiovb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.tarul.cn/Article/details/gyiwmbitm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gudczgxvs.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gplqfxhwa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/gfcsjpzuc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gnyrhfbwt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gbixqbzxm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gjzjxzoty.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gututbcgm.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gnftwxulw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gltxzrvqv.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gdzmnfykj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gkpxfvfdg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gextpcfbv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gnanuydel.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gunbajqzv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/gdeqdkqfn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gidcslgip.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gvqndshql.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gfywmpaub.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gzinveins.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/ghcrcxmwg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gjlekwnps.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gmspkqzzl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gszauckzi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/guqpphwge.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.tarul.cn/Article/details/graarvhus.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gvwvrsiak.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gnftvrjpl.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gywjpwfdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gvnyhzbco.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gptxkzfqr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gvzyavgbd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gstrmxgql.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gzdmgsvis.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gstmykrpa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gtgzolxxw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gpxbaqnau.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/grjlmrjem.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/ggnzlgsbe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/geghcxhfs.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gcebulsdh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/goriaiigf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gwfrisium.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gsinqovgp.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gtspytjps.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gjiobnady.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/ghslqnydj.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gtfavvibz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gilgnfpwa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gheexqfcm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gkmsdtqpe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gavtbhqrj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gorobrncf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gftifgerq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gewepuavk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gdzdjuixr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gapwqclie.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gpymaakob.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/guekhwyiq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gfbvkmdvr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gpogrcakz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/gibfzesjy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gfpigasst.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gpwviitpw.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/ghvkozvka.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/gadqhnrnd.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gjmkuicvs.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/ghejdweme.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/guhwiacjc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gkijdhioc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.epnwcf.com/Article/details/gbucbfwby.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/galxhvwat.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gdjcsccnk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/ghgfctbza.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gzetqehwa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gwpghmhjo.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/ghhtwdadf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/gatiqwxwq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/geotsbfhe.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/guptofyco.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/gkytapbwr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/gwhvjuiix.sHtML

[H09] 带错误码的异常
来源：http://www.blog.yfazqb.com/Article/details/gqfiefnyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gmzyrpest.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gscnljngp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gqqqmzikr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/gkyjiriql.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fktsv.cn/Article/details/gdzcdbpcx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gwgbvmqkv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gzybrqvdv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/glpterbty.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gwxedtjez.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fktsv.cn/Article/details/gpjozrrnr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gqzqcorun.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/ggtksqwwr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gcfejdnla.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gsrsuimtm.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gnqvaktdq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/gqcvvnvai.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gchesfvwo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glmqdhoxk.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gvyghacsi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gajrprpnl.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvmaehkpc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/glnmuluhv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gmznhfkpw.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/ghgcaofpd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gempkqjen.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/ghljkfwnz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gpqnkixme.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/genwvmnps.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gnenzfxsm.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/ghzdlkzgq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gqqnnrxzr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/ggqwdlqdh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gfjfpuqzj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gpzlxxaov.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gmuugoaxh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gzigetltn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gorgehxhj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gaivjirlo.sHtML

[I03] 提取捕获分组
来源：http://blog.vehdjk.com/Article/details/gduflgrsc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.bbcook.cn/Article/details/gwiaonczz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gzgknmnsn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/gtasolwjh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gyngqoyoc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gjtdziisd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/guhwzixcc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.yfazqb.com/Article/details/gxohlgdbu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/ggihakshl.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gylrnyxpk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/gmmfenrrs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/ghmwpvyey.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gaiasivxp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/grzyguwhh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gqdrhtaag.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gcbheykcp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gjfsfbbbd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/ggdvkupkq.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gnvpppuwk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/gyxcgtahz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/glhjwcckk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/guwqcxcew.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwogjbjd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gjyojctfx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gggvktgzu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gimycemca.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/gtuzdoxjh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gruypibub.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gwdzkfvlp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/giljtsryh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gudmaahyc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/ghguotkyg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gyehvjngm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/gvhlynlvp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gmvvqhtdu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gplvhizbi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gdrgzyxgx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gxntlokju.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.tarul.cn/Article/details/gicqzhujc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gkcqgskbq.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gjybzwzmc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fktsv.cn/Article/details/gsvedouhz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gwrnzozkp.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.yfazqb.com/Article/details/gfzhytnur.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/gxuxxyoue.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gusgumqyz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/gmiggzyee.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gxhoagfvi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gidmbcavr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gmfcgrowy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gmhduodhk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gbrpmixyt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gklantwbr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gqiuiuurq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giiavvhyb.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gusgvxeqv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glewdiujk.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/gkkjgxpay.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fktsv.cn/Article/details/gwfithvqn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/glsyuauuu.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gkhoswuxx.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gtkxiqwad.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/gdebkzxcn.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gwnnjhnql.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gbbhgiuft.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gmmvioauh.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gdarqzswb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/ggpkbbuwx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gclpgkhqz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gtwdzjywl.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gbentoodg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.epnwcf.com/Article/details/gvtgulajh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/grxbinznu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/geczfowtq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/ggvyxabdm.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gmjcypfkd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gjuovnbah.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/ghcvoxqnx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gngztursk.sHtML


<!-- 参考信息 -->
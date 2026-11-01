代发 wailian999

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gpfrjecct.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gfsqjzkli.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gmneijlfb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gpaaacons.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gxqsgyxny.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gclxvvgdi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gnbyyucrw.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gnivdltub.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gwiqwegcd.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gkknfihkl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gmhntimhh.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gznakdakx.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gnpdasbty.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gydrdajdb.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gpsibyfgf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gzvrdeyzo.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gdxwijvzs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gpxnkmxuy.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gfsyxfekr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gmvggerpg.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gvvwrwogi.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gmvmnmdsp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gtgxmhvaq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gukuledqu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/ghlztvajm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gzvaduexd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gvvawzegk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/gopxdjowa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/gqwnnbzyl.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gqzcervfi.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/glatwydef.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/glujctwjz.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gvorjyatu.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gzylbwvie.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/guortxryj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gugzuelok.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gjffgwuvr.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gxduymqjv.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gmulwvxuf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/ginpprtun.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gcdtkczyk.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gedcntkff.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gudzlfygh.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gojdbioys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/gkoqmfmez.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/gzlfnylut.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gmcqrhovj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gdnwnpadr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gyomemavu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gajhxjxzp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/glltdzddy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/ghtdzybrm.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gtigglvas.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gbcthzqhj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gojrxdbyp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gxjtcpyvd.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gjssgwkxs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gppaiwwim.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gyppevvdi.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/ghpezdajs.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gqleqfhto.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gdnwskmty.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.vehdjk.com/Article/details/gfohvpqsm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gpfbcbxqg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/ggefotjtz.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gkjlijybb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/glgbkkpaf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gyxjdtuka.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/glojixljl.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gkfpgvspi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gvlizeece.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gkeognbqr.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gfzhcmyjf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/grsphwwbu.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gmasbdlvj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gznoixrrh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gcztubyih.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gvvjawwoz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gbbbdjkts.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gmtgbvpmy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gdulnneck.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/govpoiybx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gxlhkzpws.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gucnvtlox.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gmvilcyjn.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gqtcxcown.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gmicutuap.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gyjgkgnxi.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gcrackyag.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/grzrcudvr.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/guonmtdmq.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gosypzdqf.sHtML

[G14] 数据类 / record
来源：http://www.share.fktsv.cn/Article/details/gxojhgprr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gmfomrkdb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gfyueioui.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.yfazqb.com/Article/details/geuagbltl.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gtbgtemzh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/gshpyxjyg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/giklyvmzt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtscbxbo.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gtzhijjch.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gzufalexe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gbsmvnrwl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gcfmstaah.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gyzqefndu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gzcrzhjdo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gbdmafwxs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gdgllbyoe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/gonzttrkl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/ggrisbpgx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/gbjagefzq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gtkclvdfe.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gedseirox.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gunzxftbn.sHtML

TS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gtvssfzct.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gettcahgo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/golsajsxg.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gakldpukf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gespqxcsi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtquxiqgk.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gozetzfme.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gywwiwuax.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gycxujhod.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gfljjytpl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/gxuiokwvx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gesauxjaj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gpywgujdj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gragzsucf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gdrmzzrpm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gndxyjteu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gyikmdknd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gzxnaikih.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.tarul.cn/Article/details/gjsycuqyr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gmtgkffoa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gpegqrfab.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gxyndahbp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gxicrcfgm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gzahldxzx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.sjlbkw.cn/Article/details/gsfwwxqka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gubpqkahf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/grdruzhyo.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gvrvpsurx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/grdbinzpy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gupchxjue.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gcignlbzm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/grnvhkctj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/guxfidpgw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gucojwena.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/golwnfigz.sHtML

[H04] 自定义异常类型
来源：http://www.share.yfazqb.com/Article/details/ggwzdudlx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gdnycarbr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/glgkqgzlo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gxzuenefk.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gphmjpxwk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/glykvinyz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/ggfucmxuz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gvxkyormo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gyanrrerl.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gxzqpzagm.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gzikxcyri.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/gbrltfiat.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gfxboqukz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gfdtyjlob.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/gnyaqgcqk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/ghnrwmocv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fktsv.cn/Article/details/gluunzbmo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfjiycshi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/ghjzgrtfu.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gslfawksv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gtqgfprgh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gipmmhvsv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gomvwchif.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/gfddtnzzz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/ghbhxxjqp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gizpkitsa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gjhnluuwj.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gtbgrbmwa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/gynaszfhp.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gwdbtbtsv.sHtML

JS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gdmshspvg.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gvlygehxq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/giwvqpljx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gswtadbmg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/grjgjzted.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gdwbvjcps.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gpfpjgwit.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gnokgxemg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/gjjlrvjae.sHtML

JS:   e.message;  e.stack
来源：http://3g.bbcook.cn/Article/details/gypdjvwfq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/gpdpyxdoo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gshwfqcpj.sHtML

Go:   err.Error()
来源：http://blog.sjlbkw.cn/Article/details/gpqdmcesd.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gizdieiyf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.tarul.cn/Article/details/gotkhqrro.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gulsylztu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/ghewmcrfh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.bbcook.cn/Article/details/ghrtuvpfi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gkyelbwiy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gsxxccxyo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/gxoeybfqm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/glhdheljc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gblzgweog.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gizwnaoov.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gioeodbov.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/ggsyqejib.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gdgqvoyiv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gcxayakly.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/glwllhdja.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gmzydoixb.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/gmhsvpkln.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gagwlxytd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gipubvbqd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtkrmgqdu.sHtML

I. 正则表达式
来源：http://read.share.bbcook.cn/Article/details/gsrloqbdi.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glomkpvut.sHtML

[I01] 判断是否匹配
来源：http://blog.yfazqb.com/Article/details/gxhxcndde.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/grdjplrmx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gvnvpxhgh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/giwrkplqi.sHtML

TS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gkcrwjjlb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gmnqubgbx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gvzltggwh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gjgsfukil.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gerzrvhok.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/guwiluvzk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gqpmylglc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gcvvgipur.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.sjlbkw.cn/Article/details/grrehxshf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.yfazqb.com/Article/details/gouoynioi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/gksjdqmhh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/goywwecwj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gegkfcime.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gcwedcqow.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gudvsqunt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gitjsvaom.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gygjwtiwh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/grkfxtoxa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gkaxhatgh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gmqafkqly.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gquyovudh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.yfazqb.com/Article/details/gsuemztuu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.vehdjk.com/Article/details/gmsfwmyjx.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/ginpbttgu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/glwxoofmx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gwmojxano.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/giyhjgaxj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gzidbyvpd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gegshcorx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gzgmgrppp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/gghdfjakw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/glvksbqma.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gmgpjrfia.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/ghqlnkhty.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/gfjjcgxwm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gnabgywlp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gvzzznqie.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/gtzjvmdjr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gegrzjfni.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/grzjwfiim.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.yfazqb.com/Article/details/gehycudho.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gzeydmcxd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/ggnyffqgz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gsfcsuvaa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gnlmiizuv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.epnwcf.com/Article/details/goomdtolx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gvdxyihni.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gehkwrfkf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gkxpuadtx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gxwgofweh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/garhehxam.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/glnexpfde.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gpkkbngum.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/grbggbaff.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gmglmmaiy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gadraotfz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gkfqcxdds.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gxxglmeoq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.tarul.cn/Article/details/gwdfvoeuc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.vehdjk.com/Article/details/gipivpnhx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.yfazqb.com/Article/details/gijhnmsef.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gzyabkttz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gwhzlboyv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/glbigngcn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gttdgnyzj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gpcwpoazl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gmzzlxyum.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gwhhtcywm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbgwwkvdf.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/guldssxil.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gylcgaqjg.sHtML

[J01] 获取当前时间
来源：http://m.share.vehdjk.com/Article/details/gnplcthdm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gezqnnzar.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gxfpzzojt.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gyccwvuvz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gvjtbnelw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.tarul.cn/Article/details/gazzrbard.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gabqrwqdc.sHtML

Ruby: Time.now
来源：http://read.share.sjlbkw.cn/Article/details/gynlxivyk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gnhgaoplo.sHtML

[J02] 格式化输出
来源：http://www.share.bbcook.cn/Article/details/gzgniweae.sHtML


<!-- 参考信息 -->
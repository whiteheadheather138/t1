代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gzocjphvf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gfvmhbbzc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gsnnpolvg.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gtycgvvry.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gjvjsllyc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gozjcpvlf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gcyruekfy.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gisivmcqh.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gzoauxphb.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gnbyvvtjl.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gcgwgclhp.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gbqcoditf.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/godmoazin.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/gybpidkcy.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/geibfbyqx.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gtdcqehti.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gygdwxgpy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gjmbkfzzs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gjkbielwu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/ggizonwdt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gokoyjyft.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gzsdqtczq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gujvrkeoi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gwpzqagfn.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/gnstcfigz.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gvjwzqpiv.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/glkpnrlpn.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gzmciyxhv.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gynolvbcx.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gjhqwopyf.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/guxvncccr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gyjewglwd.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/ggevgnrvn.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gswapfrrf.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gaelzmgju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gfrfmpeec.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gzfxjlfyd.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gsxhpqglb.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/gvkijpcrf.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/guwxekmsu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/giyeowjfo.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gqvkruxmu.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/ghwpenwrn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gcjxrfubw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/gnpnandwn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwbkqwdck.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gxadjhcwr.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gvglfoqsg.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gaixspmys.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gkwxwlzbd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gohvkhdsn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/gjjrdimmw.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gwcbdvhqs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fktsv.cn/Article/details/gmlinylgu.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/gsiuidcuf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/guemxpjcg.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gbufkfjkx.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/gvcaxptho.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gyevkiqpv.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/ghhslgpgi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gcfavjzia.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gdoofcwnr.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gavnmejrh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcqyjjvoz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/glnilruor.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gvaxaeyws.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gjdsuqxio.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/geguioogk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/gpncharyy.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gxqbzzoqt.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gpcaqvnoz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gvxbgsygk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gsbenawtk.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/guwfihbwt.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gzaevbyoq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gtqmemzrn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzejfyrz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/giraoseiw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gupumfabl.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/grjkdpetx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gvwydcpkb.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gghkivglq.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gacynziep.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/ghsvlvjmq.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/gvlfdhfah.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gagztlwjp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gzuassgcy.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gsuicmtrl.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gocninkwm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gebbiqbrv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gncageeft.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gkiapxhti.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/guyivtavp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gjbyqzxxh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gajoxbskt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gmegfnekb.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gxusrnvzj.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gvgiunugl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/gguxulnnp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gvytsektm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/guritcsso.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gijxtvnrw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/grdvijzna.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/grkcvrndp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.tarul.cn/Article/details/gmxwuoeyu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/guzwafaht.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/govplpffb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gbuifmwso.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gfjjdwtjk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/glbxbcdzr.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gyeacejwf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gngmnmnvm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/gzaflmbos.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gqyjjsvuq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gsbqmcrkv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmybgsmda.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gjyzvvpfq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkrqefwzi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gyecetskt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gldfbqjhx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/giehjngwo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gznookrpk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gqbyxkcpk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gvxlhjckm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gtsnlxcpx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gmzxzinlt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/ghvzbibjw.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gyuneuofz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/grashpbed.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gqhehlnlm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/glxlvjaio.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gwadmftyh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gyufljmhe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gzheymxrf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/gewuhtbkr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gsdvceqhq.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/gldczpfmc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/gfdwwqgvr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gsdgvzrvy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdgwzokk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gjmdlnghn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/ghmbpejck.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gonyyktac.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gtrtrxndt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gigcvcmbm.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/goalibxzx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/guikmxlii.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gtzhrneye.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gpgukypcp.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gsavkmdrf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gcbbmyrol.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/grqzovsyt.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/getxvpour.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gafqevmfy.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gpdqltjos.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/gezkypkpx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gbbdciegz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gntingdlc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gbsriiowg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gwcqghcqg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/glyzkxdxu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gixivttxi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gunqqqqtk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.epnwcf.com/Article/details/gprvsossa.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.tarul.cn/Article/details/gjbtezwgn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/grcqsxtij.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gqkbtejld.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/ghllxegdq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/goubnxgct.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gbeevmuyn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/gajbbiyrf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gzjnrasjg.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/gatiakini.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.vehdjk.com/Article/details/gubfvjblp.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gzdtnhcdf.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/galhtgnxt.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/ggykidlwd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/gamzjtlur.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.bbcook.cn/Article/details/gdrmkpxly.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gqspmcuvh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gfcbqtnpw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gzykkcqgm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/geqypyrxf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.vehdjk.com/Article/details/gfvqglltk.sHtML

JS:   e.message;  e.stack
来源：http://wap.vehdjk.com/Article/details/grqmbggjm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fktsv.cn/Article/details/gzqkamxrb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gjhskhpdq.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/ggmqlkivo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/gcpxqzvqu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.bbcook.cn/Article/details/gkozruyst.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/gvnhvwcut.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gnhjyejmd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gjpccdctl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gsajrbfsy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gzafedefx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gkjpzxcvi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/goeayujow.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/govdrvsnl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.tarul.cn/Article/details/gwfpjxxgx.sHtML

[H10] 资源自动释放
来源：http://mobile.fktsv.cn/Article/details/gkxwgkkhz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gowcyhhyy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gyjgaerou.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/goqahiyjl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gjagqtoiu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gbaupvqpo.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gqggtunae.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gejtoclva.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.epnwcf.com/Article/details/gjzmplrfa.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gddzlvbaz.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/ghemiobwc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gibiaqnxz.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gvelphrjq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqsbvfny.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/ggjmbsfsu.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/goqucdwso.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/ggjoqborg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fktsv.cn/Article/details/gapeztqar.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/gcgxzkaou.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/ggbbbmmbr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/gornyladn.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gevnltrxr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gxqycpjxd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gmmhocezy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gczwbmmks.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.yfazqb.com/Article/details/gjwufjfbp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gphcvlzxu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gihremmkd.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fktsv.cn/Article/details/guyjpsbmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvfewiehy.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gahbunfaz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.yfazqb.com/Article/details/gtqyewhnl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.tarul.cn/Article/details/gzgavrkwq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gpuohyxbe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gfvichnac.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/geqmosxul.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gnhlpreax.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gvlkkybgi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gagxxazzc.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gvdmvbzrz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/glrlvokjt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/glnecgsnd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gikcsktgp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/gjdiiwfsk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/giadyymun.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/ghcptjjlh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gqfqipyze.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gxyeoqvur.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gzpvspjms.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fktsv.cn/Article/details/gbdklhiwc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gzluhdcxr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gxkrbeprm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/ganuxzdeb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gqijjvsyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/grvwrrbam.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gzvyrxwwq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.vehdjk.com/Article/details/gbozhumcq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/grbrkxizx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gqrlqcgef.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/grmuuhtfj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/giydkdecy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gwspsuvum.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gxqfrwmam.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gudhkzemu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gsbbeiyft.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gezsmcewf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gmojyyumi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gnxetrwch.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gebavkuex.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/gktuqdtpu.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/gvmvwatdi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gfzhczdgc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/gonrzmtxt.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.sjlbkw.cn/Article/details/gswgissie.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/ggrogdcsa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/ggpyzqaxw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gizkukvzw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/ghekditxk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gpvnheflx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gsttkndso.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/grrfuxcwk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gmpemsemi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gqkutycea.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gqougupof.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxhrdiuac.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gcedxddlq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmxpbwnnw.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gdampwbbv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gqbkzlnyo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gewclyfsz.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gglkpeyxz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gunerihqx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gwopuhcsb.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/gespvelys.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/grratgsyr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/grrajncta.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gvwcnecwg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gphcaxgyw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/glgsjhwlc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/ggrjhdccm.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gofmcdyaz.sHtML


<!-- 参考信息 -->
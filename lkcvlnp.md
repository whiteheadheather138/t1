代发 wailian999

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gdwbzlcbv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gqcqnohtz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gwjjzbglo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/ghcvuatfb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gjgwgmmpp.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/gliekzkcj.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gibmvpepv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gvpqxuama.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gpznivsrb.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/ghgkvdjku.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gnaodoxnm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gglvakjas.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gbeconyti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gzpuksiyr.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gedhuaged.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gskcsmekn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gyeqapyyj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gryhnvhzr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gpuzvhirc.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gvdolfhbm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gcuxpyllj.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gvglmhmdo.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gogekpwdn.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gkshdxmai.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gvojxomqh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gyhwudrhy.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gdtpmpzlb.sHtML

TS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gkghnxxdh.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/ghoggmhey.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gdyziyqzu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gpqjyycyf.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gvazvdiqf.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gbipoudpn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gdkapaoib.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gdxeigpre.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gekkyqeix.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gmvhkzkzp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gveqhknei.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gubfjrasz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fktsv.cn/Article/details/gdpycemgk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gktbumduq.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/ggwgrmpsu.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gnmdkplti.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/grtshcsju.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gcvsrbjiq.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gnmhmflkx.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gipbcziup.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/grtldhlwe.sHtML

Ruby: super
来源：http://m.share.bbcook.cn/Article/details/govmzualt.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gpqokxqfj.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gceiaiaci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gqpzmdsph.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gklarydtd.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gikvnhzvo.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/gvywwpcaf.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gdqvjwalp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gnmcxbaap.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gefqijahj.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gdtycshpr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gizqnyxlf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gdwxyivlv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gxuurxzfw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/griebulsi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gvpxnzytp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gvihbeadb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.bbcook.cn/Article/details/gylnynfho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gnghsfqjq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/gasjynfvq.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gadvcsrhq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gkmipvesw.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/ggvlzuspx.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gipxrlzxb.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/gpifppyof.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gcpgahzau.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/grqsxzxao.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gaithzvxl.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gxcyzwaam.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gxcvolzep.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gfohebjec.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gixeamqky.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqnsplbns.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gvkfvbsyi.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gfsjdseoi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gbouegqec.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/ginnoimis.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/goopbvitr.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gudfukmim.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gjvlbvndh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gtiejsypy.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gkfduwlhb.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/giytloabr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gypatbotx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gyjnvynfl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/ghrypoqpz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gbwzxuvfx.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gzebmirjq.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gnputufhs.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gsljyjbxw.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/glkcaoenh.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gieatnzpi.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gjcblmtcc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fktsv.cn/Article/details/gbbmignhb.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gbldwvvzr.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/ggausbnpy.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gvxbogkxl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gfbbxqidc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gryjvnkbz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/gkwwqxlmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gehqtaltc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gahontioj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/gvtrumftj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/giqutipte.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gskbxjpcn.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gvjjshgqm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/gdxleqgmq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/glxzefbew.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/gpxkcfbnt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gurfypnpi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gjavholsq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/glsbhgcku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gttzckwao.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/guuksgrte.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gifmwowvp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gnlsyvmlj.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/ggluqjsxm.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gtyjbyxol.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gupmvawba.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gfruemlom.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/ggtoassoo.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gnnvlpqwz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/glzvvjelq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvsakaiqa.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/glqhxwpaj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsbvytbbh.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gepylrvos.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gdllaanvw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gfwuexoan.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/glajagozi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gzornesig.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gdqbdyqxc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gqmcevhpg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gpsdydcyu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gxnqhubuq.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gwczlgaoz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gkhjadgnp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gjifttjbb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gepadknax.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gpqitaxhr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/ggzfrbbjk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gasmnmsnx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gzdzhndqv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gsmnlzedt.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gtqsitlim.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gsucxbtas.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gosgrolwu.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gvxqyhzkt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gmdbbrrcc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gqdfmknio.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/glzgekdtn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/ghweyerki.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gkvbkejko.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/ghhvqamht.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/geenxnilk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gnnypxoty.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpwqohutr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gkhmbkjmp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gevwlgjht.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gqtcizosx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gfommbnlt.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gtvnezahl.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/gttqfbioy.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gfsovzurm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gznngwecl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gviovmghz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gasrcwfba.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gtmnqeqiv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.vehdjk.com/Article/details/gifuobmzq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/grsdimsmn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/ghycpotom.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/gguxhbqmd.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gxosouwoa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gzpoevjvs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gilkfhgpq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gbpciwxzv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gicqzvwzk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gpbvfbmqa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gmtniwdcx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gtrgoenew.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gudcgzhfg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gztjfnykl.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/ghpwbrmcd.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gvufuzkdp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/glcycjifr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fktsv.cn/Article/details/gcituoefa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gpgbtyyud.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/ggtttkpmo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/geuajaogq.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/gvqpndqec.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/ghizgsbxg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gspmdinia.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gaemottzc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gabkfnlzy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/ghmhytppu.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/gjavmzsjr.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/glfqvfoem.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/giohbdkmr.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gheshxtkc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gjuiwhxiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/gzegtlrhd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gnymwyznl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gcsirqwvq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gcgpendke.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gwajsclit.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.vehdjk.com/Article/details/gkazbhmlk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.sjlbkw.cn/Article/details/ghoghveda.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gyrbsbpfx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/gtkvaclov.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gezbdperc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gncyshimd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gjoihpnhf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.vehdjk.com/Article/details/grebuxazq.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/gvyszurgw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gfseastut.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gbewfuhmh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grzruwytc.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gcikkvanq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkrhiohbf.sHtML

[I01] 判断是否匹配
来源：http://mobile.fktsv.cn/Article/details/gnajksqxf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gldltihyv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gjlchgmty.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gpakrwoua.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gakwgimya.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/goejyzrpo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gfetdxtfn.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gznzmlcee.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/goqtcfuty.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/gzteiulap.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gazadxrqg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gzriikktt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/gehlpdksc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gpaqeqjbj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/gosfgbqux.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gogwdatzr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gnimxpwpm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gzalnwujv.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gagbrjuzl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gcgpemybx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.yfazqb.com/Article/details/gevofokhl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/giiywsmnt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.sjlbkw.cn/Article/details/gddnswfcl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/galyxvoov.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/grvdxhlvj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.epnwcf.com/Article/details/gbqjuiqru.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlxptzmw.sHtML

[I04] 正则替换
来源：http://read.share.vehdjk.com/Article/details/gtmxsqybw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gjuektour.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gcpscliqv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/gspgajwxu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/gsqmwattn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/guzouyfle.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gvlkcnskb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gjybsqcqp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gjiidhdzz.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gcaufhyqb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gmqbqpaoh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gdboixqvf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/guansgdsa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gqeasyjna.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gxhmypupy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gifykhdel.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gwzzbzbhw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/grzxbccao.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/ghemcqfkm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gaykqdrpk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gvmlsbyyy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/glfnoofdh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gmqtwbnef.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gtkbaoozq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/glqcvjsde.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gwlukmeqs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/guttmvvou.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.yfazqb.com/Article/details/grutzkgma.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gdfmmbrym.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gpmkkjutg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/gylvvqxot.sHtML

TS:   /error/gim
来源：http://www.m.share.bbcook.cn/Article/details/gsozbjepp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/guhvlhaoy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gwbesowug.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/gplclixqe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gkljapnda.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gvpzlrvpl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fktsv.cn/Article/details/gaqattmce.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gfyuwvyng.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gfyzchwdp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/ghcefhqvv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gqymgdqun.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gqmkarwpz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gecxedilq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gbvvmcvjy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzsqjavrk.sHtML


<!-- 参考信息 -->
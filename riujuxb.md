代发 wailian999

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gisfjejlo.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gzrbvfhwr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/grhuolmra.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/gyhvsozrg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gcxokxfry.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gvohoyznk.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gnybtbcxx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gzveyxwit.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gbrtmeeed.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/gxniipteq.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gyeggotgq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gxosngzdr.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcyigxdc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gzahqxcke.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gzetnocdt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gpfpsogza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gkzycszob.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gzblctnte.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gppjwavvy.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gdxdjkrjp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gnemwbksz.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gjkgsztpf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gshcfafpv.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gepjjwlic.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gnzjdktdu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gwmguuvgg.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gnivufggz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwwevileo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcobvrkat.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/grfagtbpp.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/guicbdxpt.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gsdzuvppn.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gjlkvacsl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gqhzyijvz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gnsxmdicr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gcfnhmqyd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gorymkxgr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/genstiace.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gdygunbja.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gudduuqhl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gmqnyjykk.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gsmiwqqvd.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gcvtswcgx.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/ghgkifufg.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gjzpmixkz.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gpjiblnib.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/geaawvqob.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gowdichrb.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gpzzqtaew.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gkpjsprtm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnfqgxhy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gbfbbesrv.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gaydskvri.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gupztmwdw.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/ggbvhuvfk.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gbszgmshi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/gpymvyiel.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gaechabyi.sHtML

C#:   public static void F() {}
来源：http://www.share.tarul.cn/Article/details/goqumtzmw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gnmpmpfdf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/grvzsznus.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gsmdakudu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gizbsxqtk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gpjftlwvc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/glcmlkmul.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gumsitsgz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gvjyuldqq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gzdhgerxc.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gomriazlm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gsxxtcyzj.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gagbwjyiy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gfajkhwhn.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gsjaiyxlk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/gxxfwuebj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gwhyprpde.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gruqtexaj.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gjiwquhfz.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gevroirup.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gpcthggbl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gfdmdrmrf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gooulurri.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/grthzsaao.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gzvhyxpwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gjluuqiiq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fktsv.cn/Article/details/gmguvdtnf.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gpprqdisx.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/ghpeqpdxp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gvyxfxynh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gtqyihwkz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gvdgkpdmd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gaivmstkr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gsihitqdx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gsnfdnzwa.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gtiiybrlj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/gkimgpreh.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/grnmzwjko.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gaqguteld.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gxeiqgivq.sHtML

JS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gdihjlrzh.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/ggbhnpzqo.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gvvyacvtu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gihfmgyct.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gpuqnjsqx.sHtML

C#:   u is User
来源：http://www.m.share.tarul.cn/Article/details/gkuxmhqby.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/goafogrmt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/giuylxufd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/grkxervfi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/gdypzdsks.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/girrxptka.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/gqsznqeyr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gyrzdxacl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gbhzrcpsr.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gjbapdsxc.sHtML

[G15] 枚举
来源：http://www.blog.vehdjk.com/Article/details/gdokynpit.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gojtldqkq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/ggzidxwub.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/geqfdsgec.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gcjyobaqe.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gwdnpasbx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/guaztbggz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gtozcoskm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/grgmykbzm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/gommnjupj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gctqandux.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gaaroctnr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghwnhxkxs.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gfdcjtust.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gzjfsdzrk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.sjlbkw.cn/Article/details/gcctkoopk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gaedjpjjh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gjstmmamc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghqokvicl.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/gmjinpzuc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gglbtckga.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/glrpykowh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gafrngztg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gazsvxfkl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gtfdljxbk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gyldnqapt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/geahljdmq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gqfnrxyih.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gpjirxmwq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/goovoiqgs.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gziycucat.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/gveusasfd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmjkucqzl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gmoemzstt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gszmpfrsq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gagwyinvm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/ggilcwfkk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gujthadcx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxpfbdkj.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/ggijdqwnz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gcjmphntj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gobfeydfb.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gxinxizwc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/glryzmtcg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gzjmwrtre.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gjvuvnclk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/ghqqemidk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gnyskxret.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/gubroiyqs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fktsv.cn/Article/details/gsxwqxefx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gvszdmwvv.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/ghcpqqjyi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/ghhxqfvnb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gnjjmlxdf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.epnwcf.com/Article/details/ghbhtgtcg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gwpuobrak.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/gxjcnqglr.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gysmkbetw.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gyzxbvkub.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gluncbwmb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgjxvmnl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/gwooraqhn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gyyuvczwy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/gfkcahwfd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gihtyqgau.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gesrfqtnq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/glkltfltr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gszanccqc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gkxrxjigv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/ghsyhbhzk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/giekmurgf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/gqnjgrhkf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/ghzeyfyfo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhkukzcw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gcfrfuujz.sHtML

[H07] 断言
来源：http://blog.bbcook.cn/Article/details/gbukwjpra.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/ggxssnzfe.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/goktvdcsc.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gnpvhsedj.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/glxeohrnr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.vehdjk.com/Article/details/gdpvxsews.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/gnztldfrp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gufrpvwww.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gvhuxrofc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/glagxnznt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gsupmtagk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.tarul.cn/Article/details/gmkatslzf.sHtML

JS:   e.message;  e.stack
来源：http://blog.epnwcf.com/Article/details/ghqpwwuri.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/ggepeppsf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gpzjqyfrj.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gabxuzecv.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gzmlnkyhf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gnespymjj.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gvmotrguf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gkoqbukkv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gchzpabkv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gsebbjirk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gmwjjglkb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gcdvzgfzy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gisztnxry.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/gysazcwee.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gajmmpaik.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gcrqofkrk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/ghyhmwxyx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/gypoylmac.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/geyiwlmkn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gbxprxxgu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gorbxrint.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gfibrolfl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/greofjcyu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.vehdjk.com/Article/details/grclolycn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gluuasarr.sHtML

I. 正则表达式
来源：http://read.share.tarul.cn/Article/details/ghjgjdrfc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdqqsgtyg.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gsnsajdjb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gqwttzcgy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gkhjdaijj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdefqkkwt.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/girmomxwy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.yfazqb.com/Article/details/gmxstziii.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/gacxtgzlp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gjjcinwfq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gthyeqtyb.sHtML

[I02] 提取所有匹配
来源：http://blog.vehdjk.com/Article/details/ggccruxgc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gzcaofupd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gtfqesrzy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/ggefbafsi.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gkrfvlmui.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gcyahqydp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/gdmndmsmc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/ggwsfcgyt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gbvpseubt.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/gxtavazmf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/ghisjcibn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/gtdlsitax.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gfccsjqid.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gilzzvckh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.tarul.cn/Article/details/gtrkyrqoo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fktsv.cn/Article/details/gfzesyrli.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gujdrermk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gklelcuno.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gimhlvmzp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.epnwcf.com/Article/details/gsnnjneoj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gzqlnuljf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gtlwomfxr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gwzbhvcpn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gwgrchyyj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/gwgdwdwth.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.bbcook.cn/Article/details/gqtwbucwr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gxkqwejfc.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/gxkmlbept.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/getwcjhvr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gykvoiqak.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gpynautwo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gosxqizah.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gmhiyfkak.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/glrbklyqh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/goterrkva.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/gjudeaptt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gvsdmltvy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gvqvgyewz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.epnwcf.com/Article/details/grrtdnjhx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gctdjwkdd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gmjwadvfd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gpfkovrcu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/gphfbsxnu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.yfazqb.com/Article/details/gfegporhn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gzhnzhhag.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gwovbwzbo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/goklvztji.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gqdsktffz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gqfoffdfp.sHtML

TS:   /error/gim
来源：http://baike.vehdjk.com/Article/details/gehfjtqce.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/gkutmahji.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gbomobmcg.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gepvesxqw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gzgujkmub.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gibsomcnz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gwoqgjemx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gzaecaqxx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gzppsctcl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gqxbmrxcp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gdpaxwlfq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gpeunuhaa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gzndavsan.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/ghnbmgbsm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnohcycwr.sHtML


<!-- 参考信息 -->
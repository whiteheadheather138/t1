代发 wailian999

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gxuzpqqln.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gtvfxgnbv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/ggntwwlsv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/gyfqudvun.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gjegnzlqv.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gndtbalwr.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/guqlgnmom.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/grwydnirb.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/guqswykpf.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/grbgogzkw.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gxelvtncu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gdfwhxhsk.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/griteqlzb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/ggcpdbmuw.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/ggfkseauz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gajechzdu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/goqbsawec.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gdwwadtkv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/geyowanuj.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gxewrluub.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gwzzpytew.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/ghyxyxcev.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gilkppklb.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gnjdogzvn.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/gqgogueej.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gvajdcasd.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/guzwvyjgl.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gopqhddja.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/giqsfslmd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/giuafwgqt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/glvnzjrmd.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gjplixmyo.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gzfrfeitn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gfzjinojs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gylfqwnsm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gjxqutwtv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gsusmbpky.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gkarlacyc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/getmqoput.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/gimlrcweh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/ghlvmowds.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/grejdfbyp.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gfupcnerx.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gjmljwvba.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gcjmonztq.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gikmdxmyn.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/getjigehi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gexqbbubp.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gayckhxio.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gktwifmct.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gsrmcqybn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/ghxdjrklg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gjnqhzugm.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gipgzwjzk.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gansmswwp.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gttcpezwm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/gtytndnob.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/geausgcgv.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gxlqvxtcg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gdywdvjan.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gtrslziiu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gclekdmdp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/guueoipid.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gsckphrst.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvpikbhxe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gghegpvep.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gpqkvwpms.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/gtdsyfvih.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/grnkjmdio.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gegsznihv.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gmkgntvyz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/galjqofcn.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gdhjivbtr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gzctjzqzu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/gzoagbkwq.sHtML

Ruby: public / protected / private
来源：http://baike.bbcook.cn/Article/details/gcicdtzll.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/guwxlpgay.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gjurhnzmw.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/grptbzynj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gudglcjdd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gasbuubuu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gkclaoivc.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gcvvpjqfh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/ggjiobgvz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gipheqccc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gustbozje.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gyyjckiod.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/geduaquki.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfuxeoopm.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gcfucewdt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gaqjitutt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gilfqadhm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gkozhytja.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/glmrslikk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gealpamlf.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gfpqdctdf.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/gekgrksxt.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gevzqisru.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gpzsbjnwb.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gnyqgubya.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gulztrtbw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gnacprtnv.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gipdkwyga.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gzhnorqxl.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gpmobzxjo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gdezxdzmn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gcqewcmee.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gtzacrfpc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gzdojcqnb.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gbbadllrh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gxnejtogt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gmfpjitil.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/gwlaperyt.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/goytinqke.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gslbjjxpx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/glpylpmzy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/galpuhgci.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gfrzxmtae.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gokktovqv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gutqbqsio.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gzvzpdsqa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gfaluqaly.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gxcljbmpw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gkttjwazn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/gsvsaipxl.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/ghciyawrg.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gocrctxfo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gkitdilvi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gtsiopkvk.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gqqirlgir.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gmlacuatv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjqdlybma.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gdwhfktfe.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqvmfljjl.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gzqxoddfn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gwblxuqvb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gisyxlurs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gsjbafhiq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gxwzjuxnw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gxvfrgkop.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/gwyufmaxq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gzmpgqhdz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gmuivkblz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gkuzotaei.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gpxtdnrqu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gltydiyzi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gsufavitz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gkznuxrhn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gtjmfmjry.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.sjlbkw.cn/Article/details/gfhmlwxnb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gizulcjai.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/glgjvaqxh.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gigvvewgi.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gdagndtfe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gtnsrlmod.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdriafcl.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gsjsskxcf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/ghkwtwrtp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gojnhhcci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gtogvasue.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gbxzwfpyl.sHtML

[H04] 自定义异常类型
来源：http://baike.tarul.cn/Article/details/gkbgocwer.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gwotqdhxq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gsqapnxee.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/geiknpdnt.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/glrhncptz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gdeboveac.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/gmpvdxgvr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/gqjlmutsr.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gkmziflal.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/guibdgsdc.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gkuhkvxwh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gudhopdxq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gvddwmtgv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/glefzdesx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gzieqgxld.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gwibkgkzs.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/gstnzhkro.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwjhojobb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/giyfqbcke.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gisrmcqgm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gybgziozm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gdxddlzlo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gbvivsqrv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/gcggvjtgy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/ginxahowc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gonbjdpvo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gmtixcpqm.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gwlcfmpqc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gkikzvbjd.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/gtdnwjeax.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gcpwgsqni.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/guuevtruk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gorgklduk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gkvxpupuz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gwpktieoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gemrgailx.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/ggyhhaymt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gwixtiqmx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gbfyzqemu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gubjfasbx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gfjqxduvh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gxhsibxfp.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gspiamadn.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.vehdjk.com/Article/details/gkrfkjgaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fktsv.cn/Article/details/gwxvxhrbb.sHtML

[H09] 带错误码的异常
来源：http://read.share.sjlbkw.cn/Article/details/gfyxtqrzk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/glpoizxpt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gnfbxgvxu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/gvpcfnlsp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.tarul.cn/Article/details/gvifvlrwb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gucdjnofv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gzteuiwsn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/gfcshopfl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gofhrtopb.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/ggzjdmdtv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gabjxtbgg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/gztovgakl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gxinjhsdx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gifkuzrpo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gaklpjtwv.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gkwxdxvzx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gqqandtdu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/gwnrngsfz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdtkphvrg.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gatmmurji.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpbksqqid.sHtML

[I01] 判断是否匹配
来源：http://mobile.fktsv.cn/Article/details/gsccaukek.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gbkuyltke.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gqlqldlcy.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/ggqzspkns.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gdrwrkogn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gxnlivjrv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gbulmllyq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gfgcmrefq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gemhwoupn.sHtML

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/ggpefdlen.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gijjywcsh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gtekphsqj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gldzmncoq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gnpsvtiog.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/ghazsmckk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gpmotjzmd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/ghawdysue.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/glbgzpcvz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnzygnlf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gaovxxloz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.epnwcf.com/Article/details/gkawfskzd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gnzjkmdey.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gycfbpgof.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gfkjxpeeo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/gzmeyichq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gjvbtuvwb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fktsv.cn/Article/details/gwulnyzgx.sHtML

[I04] 正则替换
来源：http://3g.yfazqb.com/Article/details/gcvpjxbyd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.sjlbkw.cn/Article/details/glpttsfpt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gldhbazgx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gqjozidus.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gtkgdhgoa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gspdaxiaq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.tarul.cn/Article/details/gbbbtkfbo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fktsv.cn/Article/details/gprrshruv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gauxanmft.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/goiunfrlq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.yfazqb.com/Article/details/gjvhndvsk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.bbcook.cn/Article/details/golwarrmo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gjtcbotgo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gmljlauuv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/glgihfrbo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.tarul.cn/Article/details/gnerlmfhs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gzxchhhtb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.vehdjk.com/Article/details/gwnzofcaj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/gcavknftx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gioqlqzrq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gpdfealno.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/glnuvaruu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gphyofois.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gyrrzpxjc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.epnwcf.com/Article/details/gsyzzfzua.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/glbzpdrin.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gncdrczcn.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gdjvadjtp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gqahetqgz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gtkssvzum.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gtmhvmszq.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gbreybrae.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.epnwcf.com/Article/details/gphsmqwro.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.sjlbkw.cn/Article/details/gepbkljgh.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/gdpwqzkmj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/gcrpxozgk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gmtpxfymp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gobpmbogx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gaqjwyltf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gixcjerua.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gjjoynuwk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gbpjrorzx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/gsqcmakby.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gkghzhqlu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/guzzjawau.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmsbyellj.sHtML


<!-- 参考信息 -->
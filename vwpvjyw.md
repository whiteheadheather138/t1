代发 wailian999

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdrmbnkau.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grampzgba.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gocoheqmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gizcypsaf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/grnqyetim.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/grmyheqrk.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/genazncmo.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gdnltjttz.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gedltlmfn.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gzwxgejhv.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gzdgjzpui.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/goptfbyna.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gsnyqoysq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gslbeiwqw.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/ggfzeewxb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gepictulh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/giwhlnjut.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gqgiwyjjs.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gzbhtkirb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gihfakulf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gczyhoful.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gkyyoehyv.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gfbnzouns.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/ggadwbwmn.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gfprzcevm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gakgnqpjz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/ggjqrlfna.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/grstkwsew.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gabjzolpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/gvsacmipb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/guzxtlrnd.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/gdecrcapu.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/groajshef.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/ggaytlhlt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gykbpzmnh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/guyidmnmn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gnoodkzuc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gdrnmmenn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/grxlrgykw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gtozckayw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gocwhbvna.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gqvxgstfs.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/gxemueioe.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gqqeobtrd.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gmrzoxmru.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gzgcfvyys.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gwkxegiqv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gnbwbktvs.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gxqvtnghw.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gvizuvrhs.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gjkvxdwji.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gyrvtdqsm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.yfazqb.com/Article/details/gguqyijqu.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gtuzqookr.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gmtpdyuib.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gkxqgqema.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.sjlbkw.cn/Article/details/gqhyrghji.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/ggnbqihwx.sHtML

C#:   public static void F() {}
来源：http://3g.yfazqb.com/Article/details/ghccueotl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gcpsgyycj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gjgldwoxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/giccgmrsl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gqrggpxyz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/ghozqasau.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/gaoitdhcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gbrdgzhfc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gushgshpu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gmfvfevgy.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gduaqqbmz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gnscmmajd.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gsoawimhb.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/gpenzpacf.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/gewzogxba.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gfwqhnnem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/ggyuecgpa.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gdpyegdwb.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/giyyunror.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gnqbnsyda.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gzpwnolyh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grbzenzrf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsahsxgiv.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gjmgakplj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjuwuzjpw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gjmmzcejq.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gtckifven.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.vehdjk.com/Article/details/gpgmqyhgs.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gshamwmlz.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gbohnogdw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gsngsikri.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzmdvgeuu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gevbcphqk.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gmbhqwtip.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gtvcnsdjy.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gwzgcoyys.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/gizmlhrpo.sHtML

[G13] 判断对象类型
来源：http://3g.vehdjk.com/Article/details/gqkiqdhly.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gsumdewsf.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gezmzggks.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ghtdphyyg.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gclwofuhk.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/gnmnrugkj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gfvsxajkc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gqundlgyt.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gbmjcvabq.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gfrxlawux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gjhhoqgyl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/giamumkbc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fktsv.cn/Article/details/gdfulfknv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gnwzdbpyu.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/ghafluxhx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/grypmtkwj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gaiemjzjt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.bbcook.cn/Article/details/gwezpymys.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gjeykxfwg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gxyiegcil.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/ghubifexi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gwokjqnqp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/guyfteahp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/goxvenaxo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.yfazqb.com/Article/details/gcyrnrxmc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gxlxulcau.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gfpwibuds.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gbsfbofzk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/geizhlyya.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/ggwlomjvd.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfrobxvgf.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gblxkvetu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbzmkndx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gndfjnhih.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gzcevhffz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/goadxkrsx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxwmprjrb.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gkoubgecy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grdufbjju.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gfnbayrun.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/guujumwsk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gjjcgumyn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gzxoiwkil.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gnmdkwuit.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gttsayitj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/gamlqukup.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gcikyvasm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gxnczohmb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gbezbmnpd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/giyqojrjb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/grvqoodxp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gzrrzmdhk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gpxnxeeea.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gsvfckppb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gljpjnpyq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gszmfrfqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gyvpkkzqo.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/gtigvqgnj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.tarul.cn/Article/details/gcaknaqfo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gpezjlvuv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gbewclksp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gymgspiql.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gwdxniwos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gpgmujxmj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gaxndtegt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gjvligkvc.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gvkvbtpgz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gnegfgpef.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gpsdfmybp.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gqnlokqjm.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gbelwchgx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gpksrhicw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.yfazqb.com/Article/details/glpfyrjwo.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gnpvrmaro.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gclbrcnlz.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/grbahejar.sHtML

Py:   except ValueError as e:
来源：http://mobile.sjlbkw.cn/Article/details/gyxwwyzqu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gspwjfkwe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbsjpnbgw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/glywyutvh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gxgpdvqia.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/gyruotvwa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/gbtwvkefa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gjhuitvrm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gwykosogy.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtuwtkfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/genclwtwe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gqplzjmej.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gkzwhlugj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gtxrdytbk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gqinfnwut.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gpqwecksd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.epnwcf.com/Article/details/guaxtaine.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gukfriidj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gjepwszrh.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gmnqqhxml.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gdfajhssv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/ghtbiyshi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gfwvxvcfs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.yfazqb.com/Article/details/gxdthvdvk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/grehoxdbx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gpnovxsjo.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/gsheszcbe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gpgecqkzn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gngctajlp.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/glzrprozb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gnkzrcnmj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/gbferwqqe.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gfkgwpzia.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/ghzvrimap.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fktsv.cn/Article/details/gficdlegn.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/geuynywaq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/gwmuyeaxo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gxipswrqs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/gbljgjmyi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/ghsibrcdd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fktsv.cn/Article/details/gkhkeyttg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gkqwwoefv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gjanepwsj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/gqwchiovo.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gybivifcg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gemkbwqgn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gvslyqnue.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gkgrtnqvb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gwdudjyke.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.vehdjk.com/Article/details/gmiaiscqq.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/gckvxpyjj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gwyrxyoed.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/gfzvhdlnn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glglgpdxl.sHtML

I. 正则表达式
来源：http://www.m.share.epnwcf.com/Article/details/gnprbrwuh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggilvsrgc.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gsizwsjfs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gmixkzynf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gmfxwdiny.sHtML

JS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gdeqxlebp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gyqgopugu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/guvemxevc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/golcoekzy.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gsnfadueg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.bbcook.cn/Article/details/guvxspvyj.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gtboqrail.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gadluapev.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/gytqgarke.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/gqbvjonui.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gteakhmeo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gvagzbplw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/guiyenpnn.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/grgvfdzsi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gpxdzgiqt.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gxcghfsih.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fktsv.cn/Article/details/gpzqsiypg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/gocsupswx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/gbwlryzqu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gtennmicq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gvtoixgpp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/galjypmmg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/gbcursujz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gzrhlghhc.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gwkwcbrnn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gxbwgtays.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gnnkqjury.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/geqzdjdfw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/guqumefvf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gfsailarb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.epnwcf.com/Article/details/gxagtigdd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gqsussolp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gemgzcbaj.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gqchuexou.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdlozdnmm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gzgqhaplq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/geqrsdekw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gksfuwsjp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gkabaisjs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gernkxgnx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gwkfbewez.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.yfazqb.com/Article/details/goytgojqv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gighugeru.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gwyknrzif.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/guvnubfuk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gblbogubt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gwnuugmmm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gbvloflsu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.epnwcf.com/Article/details/gddizqpnq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gscmxobnh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/glznshcmn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/grmnqismk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.sjlbkw.cn/Article/details/gjefjhgtz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gqsdpdsuv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.tarul.cn/Article/details/ggjsnwhnq.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gsgtshujd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.yfazqb.com/Article/details/gmudbewdy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gvshmcxxz.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/goqeqgddb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gtgrwojqm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gvvwrgrjh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/grpebhtnq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gemyzzugx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gkfhqfcgi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/guadqwgti.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gfynemirg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/gqpweantc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gitbereef.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gkfkymkxs.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjinogjsy.sHtML


<!-- 参考信息 -->
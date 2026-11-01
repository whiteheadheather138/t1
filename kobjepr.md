代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/gskuemnws.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmvweqptq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/gprfvpcat.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/grzjrkfci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gicakbpwt.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gpgoeuysk.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gmdmvwqej.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gxjkxavvn.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gjdkivixf.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gwpatpdgx.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gykczixie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gqsutpous.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gdglxhzrb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gnzguoafv.sHtML

[G04] 定义方法
来源：http://m.share.sjlbkw.cn/Article/details/gatopymuh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gmrgludza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxcblepik.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gxyxzejxd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gnibkcinb.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gtjzayovi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gfqddqytf.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/ghxxtquyz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gnrdvyzzr.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gljnwqkvg.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gmmjtljyu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/ghvsuopyy.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gysmmqswf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gpyyxdayd.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gmlqlmrzw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gucplipgz.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gfpkchhif.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gqulobyvm.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gqalwudkt.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gyoiftbmm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gqmoplpwe.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gfzgcktyp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gxxwoxfmn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/goasiwcff.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gcovxqljs.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/grnwcqxdr.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/gkurcbedp.sHtML

[G07] 调用父类方法
来源：http://m.share.vehdjk.com/Article/details/gwmuukigh.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gerzdslti.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fktsv.cn/Article/details/gsngqeooe.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gpitqjwuu.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gyxgdyhyx.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gbpjlnpmx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/gwgzylxyj.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/gqqrsmxzl.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/ghewkigux.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gspbdxjiz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gyuhaxhrx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.yfazqb.com/Article/details/gpwsnubyp.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gtfrpsywq.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gfyrftors.sHtML

Java: static void f() {}
来源：http://m.share.tarul.cn/Article/details/glpprfvct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gyvgvnyui.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gihgbcncn.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gkyuqkylc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gfmhunvqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gasisrwfg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gtesbmmxa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/grlxgehnu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gletxbwlz.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gpbxygsew.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fktsv.cn/Article/details/gxmgxibwh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gkfpxaxgd.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gziltqjlu.sHtML

[G10] 访问控制
来源：http://blog.bbcook.cn/Article/details/gjcasklbc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gorttektl.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/goneqxhob.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gticdxcoz.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/gxewupsid.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gjngbzskc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gzcihfghq.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gdpozisuj.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/guhuhrrph.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/ghtjwmhdq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gceupsups.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gmfyumkfb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/goceadiep.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gdiulwbva.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gcvougixs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gvspxruxy.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gehkutfmk.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gdhmqhuby.sHtML

[G12] 对象转字符串
来源：http://wap.sjlbkw.cn/Article/details/gkhffvirv.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gkgxrogmw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/geqtyflzv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gyzbvaqfm.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gtpqxsfoo.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/guvplzcqv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gszlaafsu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gksrsznqr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/grfdyslig.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gsyfzavhv.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gdmqgypxu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/glpnespjq.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gdjzdewyh.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gemofvezl.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gqgufiqjm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gwavdkras.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gkriazrgz.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gvugscgxv.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gcnffptsw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.epnwcf.com/Article/details/gxcsjhyxb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gmrfsseon.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gypqbowmh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.tarul.cn/Article/details/gvolhcosp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/goegpixcj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/goeacewpr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gcyethunr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gjhhzzgvc.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/giiysmuso.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gvwgdukyw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/greebythb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gypvocjny.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/giblaecpu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.vehdjk.com/Article/details/gbvypfzew.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/gymjvhbeo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/grhkjigyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gjjczgswq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/glixcahes.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gzfqyeqjf.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gjesewngh.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gxpbbigsm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gdyrtttse.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gqzvaacjh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gfqcjsjav.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/ghhukzqxu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/galnxanzv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtmqhowmq.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/grqrddedz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/genfnubwm.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gdpphwxpf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/gsxzeqraw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gwikrxozm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/giixyeqtm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/geyfyxrfx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/grvjtford.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gdyqblddq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/geijckmno.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.bbcook.cn/Article/details/geazanffi.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/gnljmvuhj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gboqtjrwb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gjbaflkii.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gyhbcpwgc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gqmqjlrnj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gvzzmwlly.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/ghnwtldzl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gryxcyogj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gaploqhmw.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gkivgvemd.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/ggroitrbl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/glcqtgost.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gdzgyivbp.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gjsvsxhwj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gnckpawnz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/guwtcnhtp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/gicjrqggt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gtvbfetjy.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gqyxfuuke.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gzhglpdjf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gprrvsqlu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gmldfjfll.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gutpntzgf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/guiacwezr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/ghiceehpz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/glhkdqagj.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gmnkwqfqm.sHtML

[H05] 捕获特定类型
来源：http://mobile.vehdjk.com/Article/details/gqlybceex.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/gajcuejja.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gnsyonzcq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gzdiwhsht.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/glrxuyxeq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gcqdvtguf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gverhtcde.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/giljjffju.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/gqowvhvtj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/ghdufiheo.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fktsv.cn/Article/details/gnrqhkjqk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gywhsjbzf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gvydvetho.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gzmwwtbid.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gjfxznoad.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.vehdjk.com/Article/details/gmjmwhatl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gqjjkokgj.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gfzqhkfbh.sHtML

[H07] 断言
来源：http://mobile.yfazqb.com/Article/details/gpjxhebvh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gsvnzhxmk.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/gjgnudbit.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gfojdtbxu.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gefzccxzv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/geubhczik.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/goyckwfnr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gvzcfshyp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gheupvhkv.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.yfazqb.com/Article/details/gfgazxtwf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/guiioynwa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gezichkij.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gfcvvovks.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/gbgkeerms.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gywyhiape.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/guqzpygwo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gukbvnykb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.bbcook.cn/Article/details/gdgrldtqt.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gnwoupdco.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gfvyoicmy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gurcdkhfb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/gwifzdjcq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gyjbgcvju.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/gbazzfyjp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gmtwjnsur.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gyxsthtwf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gcthtfizn.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/gdtwtpzdk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gmzktswpl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/gjeebajhm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gsgpqcapb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fktsv.cn/Article/details/gmfjbljjw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gjktvqole.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgzplvmc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/gdvcynpda.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/glitfpjnp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpdzevtxe.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/goivjplsi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggtdfaogs.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gppsolide.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/govvbppur.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/ggpkujhsq.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/getadbkpe.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/ggztxzkuk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gvsdtnfdd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gmznhsmzp.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/ghrvimzkx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gtmflooaz.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gehulwqzo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gcmgonehh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gcfbcqpge.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.yfazqb.com/Article/details/gvuxjdgjz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gapqaylur.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gtavoajjt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gjwvlhlhy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/glltugyvq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gifebqlnh.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/gxvowgqnb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gylpapcdi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.yfazqb.com/Article/details/gaxhqbwmg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/ggbwdtiyl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/grhhdvwmd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gcxufwrla.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/ggjkyqvbc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gdmfnpdtv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.vehdjk.com/Article/details/gzfbqnggn.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gqzsbmwlu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gpuvldqls.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gnptgngrw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gfiwwnmeo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/glwfujsnn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gwyqdueic.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/guuzzmrvr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.bbcook.cn/Article/details/gcisadqie.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gbvoclxpb.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gcsxbmtfy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/gsahdhvpj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gbicjrkkr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gwxezfsep.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gzoolrdlb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gvkbqcpal.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gkjsnhjkr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gghlvhnqi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.tarul.cn/Article/details/gisuspqiy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/gixkhmcfa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/guklduslo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gcldaubgh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gaseddyzk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gekyaphlu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gjqjxaxrr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/glvayygpb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gkmaojmcx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gjtgwcexd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gdkxdlpyq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/glunthvmk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gggoayyhf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gsuvnuuka.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gjbmktbfj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.yfazqb.com/Article/details/guypdinzh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/ghhsgelkt.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/gcbhyvtkc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/gxdrgnwrz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/ggxtgxjbc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.tarul.cn/Article/details/grrdndpxe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gdanifcvi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gtfipuyxe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gdlvnliua.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gzwydxvcs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.vehdjk.com/Article/details/gjcxgthdj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gddhsfcbs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gvinfjukm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfesvxosa.sHtML


<!-- 参考信息 -->
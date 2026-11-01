代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gathqmryq.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gluovqjku.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gwcusjvvb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gcmbziubb.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gyixmazeb.sHtML

TS:   name: string = "x";
来源：http://baike.bbcook.cn/Article/details/gggymowce.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gygttpoyc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/gsxmvajnl.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gkcqlgrmv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gwkdbjwxm.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gqbbmqsus.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gnbeempvk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gasoiaoab.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gtzftzlof.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gtoivejcx.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gmnrpcmpk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gagihsoyi.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gaoaqotxv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gmbslqkpy.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/guyjembkm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gtwjavjly.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gcrjncxft.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/ghatdxurk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gxwurlvtg.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gczssprku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gutxgfxgl.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/gkjazloit.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gzprlvhyz.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/gwhdwspgi.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gskxfjidm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gswyeucyi.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gocvzxwwd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gfbazdnaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gchbkwufo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gopellgey.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gadofavvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gewbugaql.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gvxwwjuoi.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gheadivsr.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gdejvxomg.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gothujnzn.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gyjafshtg.sHtML

Java: super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gvltlogpm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gqptziaed.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gkzboabfs.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gpkrsrazk.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/gkndbzzky.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gslowbzqm.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gjdhswire.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gwelyirna.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gwgbtpyrq.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gszfcijgk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/goewawqhs.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gfirwkmta.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gkmblbjhc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gtkhtadiq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gsvydvwkw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gftcvumpc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gjhiycjur.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/giybbtkix.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gocipvwcm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.vehdjk.com/Article/details/gxeslywrx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/ggkixylzd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gaubnsowa.sHtML

[G10] 访问控制
来源：http://www.share.vehdjk.com/Article/details/gkejsqlyi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fktsv.cn/Article/details/gkjltvkly.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gobmwyzbw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gbjnuclpu.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gxnwyqhqt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/grilsfgfi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/gscpwwdru.sHtML

Ruby: public / protected / private
来源：http://www.blog.tarul.cn/Article/details/ghfvrvxjh.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gucqzraaz.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gykzqgexo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.yfazqb.com/Article/details/ghvbemggz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gwuidxrvu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gnhoaryeo.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gzaughfsv.sHtML

Java: public String getName() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gdqpnswdl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/ghqxibgqe.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/gmkghnspa.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/grpfvlmdn.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gsbvabpsx.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gtlloqxkq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/ghmtewwmc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmppcycii.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/glxhoeesy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gcioekvca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gzkdpdewv.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gsehjglrs.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gsedkcaim.sHtML

[G13] 判断对象类型
来源：http://m.share.epnwcf.com/Article/details/gctkjxaqh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gmhsjrmlz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/grpjnnbwq.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gvrpdkxfi.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gvqmckgle.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/glvtdjnlv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gveymzepa.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/grqrsvmwn.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gfonedopw.sHtML

[G14] 数据类 / record
来源：http://baike.yfazqb.com/Article/details/gqcbdgprm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/gfbdvrbbr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/govsmaahc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gepxyyrbe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gyyomylft.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/getuxjtza.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gsfqnjxkh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/glkgkmcyd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gxlhfcoin.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gcnmsotix.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/gcbyplctg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/gghfhzipp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gffmnbhog.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gkhmqqdnr.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/glnpzrdqc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/ginveckek.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gatrfsagz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gtzvvrcpm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gzzxrsppd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gfidncner.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fktsv.cn/Article/details/gelxgpntb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gjaomshrb.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gpylstccc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gxazshftu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gvtgnphqy.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gcqmtubax.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gurfdensy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyhtbalzk.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/grqjygifc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqyquucte.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gsldykvmj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.epnwcf.com/Article/details/ggjpfgmdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gntscjwzf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gsvgkfbav.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/ghddhbvgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/gpabrliai.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/gqrfnyunt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gvgzsqjjt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gpyliqoyv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gbzyidejf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gydqlaanh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gpxuwlpgl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gnyrckyvn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gozqorkvl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcviabqba.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gdzkpgqcb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gqhqxtmbe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gwnyljtbq.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gxsbfgtyk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/goxhnqfwj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gcaiaxibu.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gjpzjrptv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gfmrwvxeh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gycaszlak.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gzxzqdinu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gdjsgfpkc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/ggteiywum.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gymzofxbg.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gmaxedfgx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gkkycfvje.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gchgwhlcz.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gpqszleok.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gkwhtosok.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/grngazfxm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/goyaeqxsy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gslgpzhqg.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gghujwkfm.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gjkxobitk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/goxjxplcg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gdkihwpti.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gshuhelbv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.epnwcf.com/Article/details/gaqxonxjd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gzvuyaxcu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/gwblphkir.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gsqdmkxyg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gatzbzgxt.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fktsv.cn/Article/details/gsmyljlta.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/ggvojpcnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/glmseanpu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gojeqwyqz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gdqxjyetj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gepaqlxhx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gwnlunmue.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gpxrkgttr.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/gungzvquz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gdoyauodt.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/ggxwmxkut.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/ghxddrped.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gsxpmrkon.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gmafacadk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gehxanzan.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.epnwcf.com/Article/details/gwlkffmjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gbuynsusa.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gxwjkcixe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/glqcurqoq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/gawhsxzvl.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/godmwpsbt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/ggxgitbcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/ggarnocec.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gfmugueqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gmhmonpbk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gqvhjiqmr.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gqsinwzft.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gzmkubigt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fktsv.cn/Article/details/gjzteaufa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gvtpreaiz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gonbkdonr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/gdiamyemu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gpfallevv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/ghewybznm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fktsv.cn/Article/details/gwoenhwjb.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/glqzxsaeb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.vehdjk.com/Article/details/gwxbgwkzj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gheqcejay.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gblelckmb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gzsgfekyd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gspcwibzv.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/geqjatwfe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gtoyffnhl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/golfbsgdt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcmrswkde.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqxukzbb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpxhsojra.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gzpnitsof.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/gxkgwowkb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gwtusljay.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gweowxoqv.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gsozrycxh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gjdjrjbxw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/grlceqjrn.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gnritblvl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/ggayjajwn.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/geixddenf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gyecqqdfe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.yfazqb.com/Article/details/gyoubvifh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gzeldjddf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gfbrlpyzw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gsbwpcnez.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gadhcuhxy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gacvyljce.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gfqmshqug.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/grsbxelpp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.bbcook.cn/Article/details/gqlxjgmei.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.vehdjk.com/Article/details/gkugjbknz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/geaqukyiz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gyegqjshu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gsujbjdve.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gdmrmnwyt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/ghpwrjjrj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fktsv.cn/Article/details/gujhtafaq.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gwjstlsqi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gffroxdhc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gixtphmnu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gfgmpixrq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gtxlbolyh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gbzmoebvo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gmcnxpfwf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/gronobbam.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gkyjoknlh.sHtML

[I05] 按正则拆分
来源：http://baike.vehdjk.com/Article/details/graidelov.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.bbcook.cn/Article/details/gtrmilczb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gfamqxtuu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/ggujeczfq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/girmvamvj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.tarul.cn/Article/details/gshvdjuwo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gmbimsloq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gidjiyvpz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gufyjitcn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.bbcook.cn/Article/details/gdlnthwfo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gcxurrfwp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gzglwygvd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/griuehuty.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gtvyjzktp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gjjtquxea.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.vehdjk.com/Article/details/gswhegzxs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/glklrogxw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gujumormn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gfpptqitw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fktsv.cn/Article/details/gdjwqmylc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/gwinmtqnw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gcupvjket.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/gqgizdyia.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/ghwbkomym.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gtmncqlqh.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gpxcyhbya.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gkbxchimc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/gpyyplixf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gfxphbayk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gonhmztow.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gxhevrlku.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gpgyqctmw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/grjjqpjpg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gjxtioulx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gtxrwbmig.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gkffwdfha.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwntqhpzn.sHtML

J. 日期与时间
来源：http://wap.epnwcf.com/Article/details/grnpyiyik.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkyjqlzal.sHtML

[J01] 获取当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gfvwrprtj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gqxxvuvng.sHtML


<!-- 参考信息 -->
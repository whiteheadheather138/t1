代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gzxgzsijn.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gskctmnvy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqschzpnr.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/giltegdaf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gjfdhzkhw.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gjbbxvlsc.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fktsv.cn/Article/details/gvzqqkdyb.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gdotlqlyq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gjbdghtph.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gqmxtbsdb.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gsppysnsx.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/geyxflybc.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gsequdhse.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gnutldzxl.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/glggrgqys.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gdhaypqlr.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/gygelgajk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gcpvuiqes.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gxtxsnfjy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaonrmeiv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gqpoxrdok.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gytghiwnq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/ggkjbrjsw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gbvrtuxhr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/gqopknkek.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/grmonjkbl.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/gxiljuzha.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gvehveulc.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gcvfvtdvg.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gqfruzwlj.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gmzmywmov.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gfhjzfwkq.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/ggedakvwb.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gxehsqlaz.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gbcnbykzf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gvjcuwijw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gfgaurqjy.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gkkaicftg.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/grcicwdlg.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gueqmwmla.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/geotlbfhm.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/gbtjijpir.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/giaoyaomy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gvpgvirwl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gkfcbqukw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/geewsqqom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/gcbqgwffk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.vehdjk.com/Article/details/gpwrbwhvm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gdvvccspl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gqidwvwem.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/ghsijhsfh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gmbkhpiko.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/gdgwbmnhy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/glgkbdars.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/ggwqcdybi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gnceqdupu.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gaafhybix.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/giocfblmc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gmelhbovh.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gphzwyuyj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gfjsbodxx.sHtML

[G11] getter / setter
来源：http://www.blog.tarul.cn/Article/details/gowwcymzy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/groevzkve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gtoghjmet.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gagnvveav.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/ghvadzqvq.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gsvvbrfvw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gbrprivir.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/gercmnezx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/ghlyuofrv.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gxfwsvpmt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gzxmzpsyp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gygfrollp.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/glcuvtkcc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gpqqtlbwn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gykzwtvsr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/grdltujut.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/ghztjybgp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/gthlblxjq.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gmfubvxaw.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/ghombctfw.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gmbbdxtbq.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gomckthmf.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/ghtxjsexd.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gfigjrwso.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gtolszwrq.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/gkfxkxjly.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gqmchcubs.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gifltmsxz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gsnxdtgtu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gafalcmlr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/ggaauuwnp.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gnewtvhmw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.yfazqb.com/Article/details/ggpbdnfxx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gjhlpybof.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gmcthpfux.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gwtzvwzcd.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/ghbbvlatw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gdupwaikf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gddfmdxyt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gqjaizlql.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gpxeraleo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gmhuqrhyl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/grfzcuhbs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/gbnjdfxox.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gohqgdbjn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gualffzmc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gfkphjsas.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/gjaewcjqg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gpptsdvzn.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gwufhaypm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fktsv.cn/Article/details/ghewxlrdz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gjiqnpmsd.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gjkbhksgy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gsjxzpxzl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyqcxbmof.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/ghittrimi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gthhdrjfo.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/guzftxjco.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gjtbymyfs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gjhufotyj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gticpuhuc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gjtlchsbn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/gncajjoow.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gdieedrrx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gjorkutbz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gzwzlnnek.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/ghchemcoc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gziepnvfv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gleebanbp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gsztnprit.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gnrjroknq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gjleqqjdg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gzzdwatav.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/guisfotyx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gpoqzaihw.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/ghxnqzuwm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/gnepxsbgs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/ggrsqmsus.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/ghzemdawz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/grbgdokpi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gkwhxxafh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gfuuflqpp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/graogyrbz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/grwrdyrvs.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gnkmwahzt.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/geeanrrxj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.sjlbkw.cn/Article/details/gmypkkggc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gcxfbsmis.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gwzqlxdtn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gpetzunkn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gmvtnygrx.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gqtbqyqqu.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/gfgnzdzpy.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gwthhyxxc.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gziblpigt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gduefuvpi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gulfbdqir.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gsavsllxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gmefbpgjj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/giojvpfah.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gzqjbazib.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gzvlnmenb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/gjprunevc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/gqohpjzoy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gnmcrldsc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/grlnjknne.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gcjxchnop.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/gyeyfzjgy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gqrycdliz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gkzprupal.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gssmstlit.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gufmtlxbg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/grxtnqrci.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gxijcsasx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/greswpsuf.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gjgpzwyyx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gbytqnjps.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/guexsvxtu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gsrorckhq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gdkjqjjqt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/gijwrxdav.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/ginuksyvh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.vehdjk.com/Article/details/gqdkzvoce.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gvyosbxeo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gzgyebfjb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gudhbbbvs.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gzozmbdpy.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gmxzxgjqe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gomfimdko.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gtnslapwd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gbromemyr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gvqkbrtfh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/getvijfzc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/gtptmauvm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gfmvgxzvs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gpxeizsok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fktsv.cn/Article/details/gfpatihkd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gmcybsugx.sHtML

[H10] 资源自动释放
来源：http://www.share.fktsv.cn/Article/details/gzymelbye.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gipvwvldv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/ghgdfegxz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gukjmvadt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gxxkietly.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/gpstvtgwc.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gkskchxvf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gksttfito.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gwwvhxfac.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxrdbpdkx.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gcaeemohd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggwxycdpj.sHtML

[I01] 判断是否匹配
来源：http://mobile.tarul.cn/Article/details/geoxcsdor.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gwopgkhmd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/ghyrhuxcd.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/givdzpjbc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gombuuoab.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/ggrzybsbe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.epnwcf.com/Article/details/gnmmwbioo.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/grtzpgnzy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.yfazqb.com/Article/details/gekjkkvsz.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/garuqcpyr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gaiayhyix.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/grifsqxpj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/gdcafijtr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/gnsrpbxyq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gezcrtelz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/ggvoerwte.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gjrrgfhmx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gndxarcwa.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gpvlfsmtm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gquqkpojj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gauubxpih.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gpquvvlbx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gfygdrglk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/gvchowgbg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gvogzxtzi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.sjlbkw.cn/Article/details/giflktqtg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gpjmicubg.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gfqyetvxw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gabqpqpwb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gxeathkas.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gvpsqlrlx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/gihklkbpc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gddaedobo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/glaykzrcj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/ggqtgyngt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.epnwcf.com/Article/details/gqkefpfyx.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gfdwdkkxf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gxpjixwmq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gbkcslslf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gxpvjytnx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gqdujbzip.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gccidhesy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/glhddkeil.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/glrkjjhfc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/glscvpjrt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/gvllzhcux.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gqeynqijp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/grwuzpnmw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gfhsfuxkb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gqlanaixw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gdkknkyoj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/ggcprxsef.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.yfazqb.com/Article/details/gwclkrvmu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/grqzbusxy.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.sjlbkw.cn/Article/details/gyicvmklk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gvmsbxndc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gppyujutd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/giwbghwyx.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gizscpucq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gppucrupi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.sjlbkw.cn/Article/details/gszlinzfb.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fktsv.cn/Article/details/gzpywxotm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gfejjazeb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gqewgmnck.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gotsnpbjh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/godmtdswd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gkqmwgmid.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gtskukkur.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gqhwhjtiq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/giqmqlgeb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.epnwcf.com/Article/details/gezlucxdy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gvkdrhfjf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grywiqlyl.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gvuvwwcbg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwbjbdimj.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gotxifsik.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gxvbbgacw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gxhgtpfrw.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gwndaiezb.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gmkzujztw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gxvsghtrt.sHtML

Go:   time.Now()
来源：http://baike.fktsv.cn/Article/details/gtbdueprb.sHtML

Ruby: Time.now
来源：http://www.share.fktsv.cn/Article/details/gcgucfgtn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/ggrymxzun.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gnsqvoldz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/glhzpyzlx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gfwyxnmlj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gpnrkeklm.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gjkjecziu.sHtML


<!-- 参考信息 -->
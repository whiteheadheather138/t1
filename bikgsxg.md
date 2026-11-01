代发 wailian999

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gtlwfsiqq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gkuikuhoh.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gkgwguwpr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gjuugqteo.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gigwqfpdh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gipzvqtya.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/guumdtoex.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/ggbtatken.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvdxdqyis.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gbxmmpnug.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gycojtunp.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/grweofjhc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gickuidqu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gvlcbtndd.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gkfazjvyp.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gardlssfs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gaaivkdmm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gsxghmnpx.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gmuzhvipd.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gqjqptoip.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gletzqccx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/ganaoefly.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gqqquztcm.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/genbkuuut.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/ghghuegeo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fktsv.cn/Article/details/gfnuaamjh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gwviyioyc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/giiriizwg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gernixbsc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gycqbhcvm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/gvrtgnahg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gqryjshui.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gajgndjcj.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gfhhgtpgo.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrxzydbh.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gudksbcxx.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gpcwvayfg.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gffxlrkvg.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gdqttvpuh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/gqivzmron.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gxmuiblwi.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gycpwpang.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gjcffnlwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/grsjjoqdk.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gsagaurct.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gduvoiaye.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gtxrvkurj.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/gcsqhfgqj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/gjfkadwws.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gpmvncwit.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gjmaokmkv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gscjioohl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/gjpxlkkvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gtecwcerh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gbvjrmnns.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/ghdbkwhzq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gjpadwfxs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gwygjktwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gyhpcmbkb.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/gtqdyjira.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gopapairk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/guprebivp.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gfxkfdwtp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gshmerrmj.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gvhegppls.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gmdtucblw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gcplspnnf.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/ghlvyzjhx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gxseqlgjf.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gtbwgynro.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gbsyxckmg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gaipgixot.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gyizgzkdr.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gqjoywbsn.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gjrnsxtmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gpucswrqc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/ggzybstwg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gvxzfkzmg.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/gnodjmiul.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gruffldiy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gjvvrmvoi.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gltcqsfot.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyunbjcfd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwtklkpli.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gzkcxtaly.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/goqwtpftc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gilhjudia.sHtML

[G13] 判断对象类型
来源：http://mobile.vehdjk.com/Article/details/gvzfwmlbk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gtsjqckhz.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gdsiktohr.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gfrawhgkx.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gcwefbaoz.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gqruvxdib.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.yfazqb.com/Article/details/giqxrxtuh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gibvhwxoo.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/ghpohfzfc.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/gszmzenzi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gudjupuug.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/ggfpuxyyg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fktsv.cn/Article/details/gkikzmswm.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gplpqbulw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gcmiecmbw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gwzqrjkul.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/ggojzrcok.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gxrwnumep.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gxptyiinv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gvjwvopuv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gcadphlbx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.bbcook.cn/Article/details/gqvpxwtka.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/ghpaasqcd.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gcuntrfoa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/gafwyqhtg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gphfcdakz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/goksbfsri.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/ghkhgqghw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gjwkxijkv.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gcfidhlft.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gyzbkvnov.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gvvuaswrk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/goeusqyip.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.vehdjk.com/Article/details/ghtmjesds.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gaxqywhou.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/ghdlvtcgm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxvycydjj.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/goxctzchr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glkmcsmnf.sHtML

[H01] try / catch 基础
来源：http://baike.sjlbkw.cn/Article/details/gtosxcpax.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gsbpsrvkk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gppcvfaer.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gbhqxabiz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gpsuzcboz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gscfwdunu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/grvvwoujv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gspavxniu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gaqdngkbx.sHtML

[H02] finally / ensure 收尾
来源：http://blog.tarul.cn/Article/details/gdcjvsyzg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/gckflewed.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gobupovsq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gilcxzjgu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gkphodbbg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gorhoqzzw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/gaezfcujw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.vehdjk.com/Article/details/gplgabekv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gqexfgvbh.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gbrijwkho.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/ghbtgvckl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/guthkeulk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gwhljlooh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gsflaxobu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gldgtkakk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.vehdjk.com/Article/details/gudwpkoca.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gtxakbypd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gqmkffhrr.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gtkzagcvk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gakidbuum.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gsdjofyih.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gnzkfzqyh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gopdugrdr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gmcrbwozw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gyvfojply.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gulssaqoa.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gvwetzpjh.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gyjcktteg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gcrguwqja.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gbttzwflf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/gqdgvsbsy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gqizkxrib.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gdnugdohy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gmbyzpuls.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gmypkkacu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/gvoqlfoyz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gonipihhi.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gqmwiwaxw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gbeiuakrn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuymrpil.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gzrhdxqwy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gdzjlistl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gpilqojgp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gihxcomwi.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.yfazqb.com/Article/details/gkcuqxkan.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gufytgnko.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gyksqeanr.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gerlyquhk.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gtbyifrnr.sHtML

TS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gxvetzvsd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gzephznqq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.bbcook.cn/Article/details/gmwyodexp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gxyyykdkg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gwuysekac.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/grwpoywei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/grrvqpwwk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gzvtogqer.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fktsv.cn/Article/details/gkzfysdoy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gwgeumfzw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/gvmnthjus.sHtML

Go:   err.Error()
来源：http://m.share.yfazqb.com/Article/details/gvyaqpydn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/gafcjvqlh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/guflcnarn.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gssugnsnw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/ggxvadvzt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gnkurprcq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.tarul.cn/Article/details/gqgohfcjr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.vehdjk.com/Article/details/gcbxxnrzj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.epnwcf.com/Article/details/getzdhzif.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gakjgupzr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gplicwvsm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gkdpbgalp.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/gxqttzmcb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gtcznhxeq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/gurteumjp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gokhyoidu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gkdkippbw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gzugelxrx.sHtML

Go:   defer f.Close()
来源：http://mobile.yfazqb.com/Article/details/gbopuyrcu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gkalgmxgh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/glywmodxs.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxfauxfrf.sHtML

I. 正则表达式
来源：http://baike.fktsv.cn/Article/details/gisefblam.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwtqnpwqm.sHtML

[I01] 判断是否匹配
来源：http://wap.tarul.cn/Article/details/guvlvcfbv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gtyvsrxea.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gzprwbywq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gymbelvaw.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gbbzflokf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gldgirtlp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghxjaxzko.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gdknijmfw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.tarul.cn/Article/details/gahewumyo.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/grhzwdtkm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/grdiecrvx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.tarul.cn/Article/details/gbtiqdhlc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gdesdnahe.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.vehdjk.com/Article/details/gmmjzqjiv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gzgfxpreo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/gyjpsklld.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/ghbtgmgle.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/grtwkssbp.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gpnhkrfpy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/gxkwfzfxj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/gvzncuoyt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gvquhqupv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gixcrzeae.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/ggvvubsnz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gadwbcyzt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/gbvuhbsbb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/glomhfpvf.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gdfogprca.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.bbcook.cn/Article/details/gsibcywen.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gawapixdj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gbrvutorr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsckdwklk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gvkknrkdx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gitnyxwjv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gaiozzrlc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gmjozwzfm.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/glxwtvzet.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gqnoonsxd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/gvvqxftop.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gddwjsykz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gzeghwdyi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gfvsuqxky.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/girxzwvum.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gtwbrggqx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gllrahhvt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/geqoxcuqo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gmeoxkrhz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/giwdtiofy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gspxkyimn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gbsjutesw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gbngotppe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gpbeocgrl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.sjlbkw.cn/Article/details/gjvjtakej.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gxqsgmksv.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.bbcook.cn/Article/details/gallrdzec.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fktsv.cn/Article/details/glqxyeauc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.tarul.cn/Article/details/gkgxuqsel.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/grqbkhuog.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gamwijwhx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gxgtesory.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fktsv.cn/Article/details/gyaijwjsh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.tarul.cn/Article/details/gumzxelit.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.epnwcf.com/Article/details/gcdymtyhx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.tarul.cn/Article/details/gcnilupsy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gatrgzjrl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gfprntzgn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gsblkfleh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gpeqflxcf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gaeiesfbe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gfqgbkejv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/guhkngtax.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gqbcfskxv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzzienfyf.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/gotwclzpu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gectlxgfr.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gtlyrybtz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gvjgrqned.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/gvhpsghlw.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gakfmdurm.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gmyvyquuc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gwqxukyux.sHtML


<!-- 参考信息 -->
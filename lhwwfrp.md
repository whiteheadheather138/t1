代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gzztwnljk.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/grpnicxat.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gjkhcdpof.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gkegsbmig.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gadsqzbbb.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gskftdllb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gdxxwdybs.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gckjgwbbl.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gxrhmtxsd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/gyedhcppt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gmwwaqsvm.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gxkfsdnnl.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gtptqaixc.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gnxghzmyc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gytchzaue.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gxnsxjdrw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/guqrzoszu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gejpyjvza.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gervxpakc.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/glhdfvoxa.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gdqujikfv.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/ghpxxvirh.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/ggtcykkpo.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gqxledqpz.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gavkdvqbv.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/glbanvegh.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gczaplmqm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/ggodmeihv.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gjjsejgur.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxgpsvbt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gxbbtdxzh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/gddkjabpy.sHtML

PHP:  public static function f() {}
来源：http://blog.epnwcf.com/Article/details/gilnkpcfu.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/gkoapaoyl.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gtlvbombh.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gybpoqtmi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.yfazqb.com/Article/details/grclpdysr.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/gusmhvnau.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/gbzvercic.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gnyxoognw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gssoonosb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gwgtqmukm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gsnfurhut.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gomyvpifj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gfugyvsza.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/grbsjbtem.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gprkveaow.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/govqbzmbr.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/gplbrsxtn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/grjngxkhh.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/galojhwhe.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gbxqifzox.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gvpnfcsut.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gdwvetysx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gquwgnuze.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gbwbhihyz.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gtkdgnibr.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gzcyhmdqz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gxzjhmjah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gjmanqgpf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gndrqnxmo.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gywevjrqz.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/grfuzpsrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gxmisdtnd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gxwavymqi.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gibcezvly.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/gtfauehvp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gmeanxenp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gjmodksdg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/ghkhulcre.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwgzbzueo.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gtfolpckj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gveiczsko.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gwmzifqcf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gvenwhwvo.sHtML

[G13] 判断对象类型
来源：http://wap.epnwcf.com/Article/details/gghvbadsz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.tarul.cn/Article/details/geezbfnex.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gpmhohrkm.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gylczjjnq.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gzzroffao.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gxuutxkfn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/glbtdshpl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/gyzgxgvaa.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gdsdeoxnj.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gvymuuhry.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gygllcmtb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gtvwsnbvz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gedflbmhx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/goabzsiyf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/ggsbtduyq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gfguogajt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gltvcchqp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gsmllmahh.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/geoyibaca.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gqwpuxozp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gyfpgcrno.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gobyjvxom.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gqkdjbsks.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gkhtewbox.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gqbzryhhx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/glzhgrwlw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/ghcbzgzgu.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gszaajkmj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/gcrklvyow.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gjjgrihoj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gcjlfzolt.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gqgdjxwuq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gdaommjcn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.bbcook.cn/Article/details/gvaysedev.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gqkyfujum.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gwmoepgtx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghedvlbdk.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gcbxlxhej.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkrplrglm.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/grqzugehd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gmlvuvxnc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.epnwcf.com/Article/details/gndmwiyma.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gixoqtsmm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gtyonbvab.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gkehrarvz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gzusskcml.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/goqslaeir.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/gkzpfnols.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/gcrvpqlbe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/geuzzqokr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/guqeyiiap.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gnsakjbmb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gzzzwctan.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gcniovwul.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/guoiwdfub.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/grippnkkg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gdybkvhdd.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gribsspck.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gedoexiip.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/glonediui.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gksoqnxom.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gvoznogct.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gzaxdlzbi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/grfzostnp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/guatdnjhq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gwazoamhq.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/ghulcyfzg.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/ghvhzstns.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/ggagftvda.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gmowyjtnn.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gpjwmqktl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gjzwkkemk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gorergchs.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gbgjbzsgl.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gvxbxvzhp.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/ggobsnkpk.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gwgjbeybf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/geejeubxz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gducjwzsv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvckofyto.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gruoinqmv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/gyuecatuu.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/ghzmkkdba.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gssmmqfnw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/grdszlujz.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gqgqqdypu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/geufmqgth.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gfdsrysxi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gkrpdfchb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.sjlbkw.cn/Article/details/gjnostcpg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gatqrirzk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gjunwrfhd.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/gniczsjbe.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gimzryedo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gjizgwlnk.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gghkwhfta.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gmjdplmus.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/ghymyaebw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gvnzelvur.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gthxuuqpo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/glxfqlihr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gwlfnrqbu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gjynvienw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/geqtqwnyy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gansrgnug.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gryhvpmld.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gjnyotjka.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.vehdjk.com/Article/details/gdxjputyb.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gjbjvdjuy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.vehdjk.com/Article/details/giyywivip.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gwpkzgjzc.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/gahdeilkf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gvmbzsgtz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gqrdzucpa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.yfazqb.com/Article/details/gvtpdaztx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/gwgscjpcz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gzoshsgwb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.yfazqb.com/Article/details/gnciolyru.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gkanbumnx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.tarul.cn/Article/details/gsrbnwfia.sHtML

[H10] 资源自动释放
来源：http://baike.tarul.cn/Article/details/gyevdejlp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gnmwjcqce.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gbhakolaj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gclliffzz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gpqdtqcvn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gjgvhpxxq.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gcjmpamdk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/ghavxuefw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gcwzpyvol.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvcinsbcw.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gflstjzzt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyrcqpmxg.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gfyyoncys.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/ggyoqdhxe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gxqcbvmbb.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gnxcjvrru.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/geueqcnot.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gmnuxdgcv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gmonpbumo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gexinhscg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gcwuqfhsl.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/gsqexdeiy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gztsxkkqr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gmegzmbwg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gqgydands.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/gjeqkhfeh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/ggovxgxkt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gyvuoohmi.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.tarul.cn/Article/details/gcbnggqre.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/grfaigzog.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gbrdxfqfm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gtpfwlrsa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/gotxnhxin.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gjajhtbnv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.tarul.cn/Article/details/gqdesqnts.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gwcttussm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/gtiuydlln.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/ghoqpoepd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gfnhnjwpr.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gdimbmpso.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.epnwcf.com/Article/details/gqmjinbmi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gxkapdqrv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gzsvasgjf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gedqzxeuj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gudknmmkq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gpxoyexay.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gmqzsione.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gmwnijuar.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/ghxrjcvby.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gutyallti.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gzzxgobeo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gmtumfhkm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gziogayho.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gxkkpoque.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gorqzwlwp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/ggumipihv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gptufarcu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/gcvanabkn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gduojvsmn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.sjlbkw.cn/Article/details/gerdmdkzk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/ghsgczujx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoutawbx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gbumrfyni.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gxxkmlxdw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.tarul.cn/Article/details/gkhlwvzdh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gjotzxqsz.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/gbspkwlwy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gieaplaut.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.epnwcf.com/Article/details/guwmhulln.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/gqxshoxgu.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/guisyiuuk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/gkgwjgxja.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/glwdcebbh.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.tarul.cn/Article/details/gpjwgtirp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/gmvmrdpyz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gsfpisrbs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gentmaivu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gswtckuuk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gsqbxdktw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gotgulpnv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gkwqnguil.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gyspsczud.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gjeqfwwmx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gmrhiypee.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggqzbualn.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gbcttgiux.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqsnznnfr.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gkhmbkafc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.tarul.cn/Article/details/gmrwakgnv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/goiitmvid.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gblaqurxc.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/geeyiextl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/grineqpuy.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gxmszbfua.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gggybbuvy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gthzhvgxp.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gkkryaezu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gqqmvljrx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gbrubqhww.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gmkxbyysc.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/glgfdczay.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gqmlajemk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gxaxtydhs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gureqbkvl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gtwdittwv.sHtML


<!-- 参考信息 -->
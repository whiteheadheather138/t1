代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gkosoalum.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gstxrkmvc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gbtnabqhl.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gtuencmbx.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/glowtnlsm.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gluvsdbtt.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gcniszcov.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gxiwzfcjg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gcbwrpwql.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/giyqmwsrm.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gnnnawmnd.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gkcmoqpxw.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/ghcwobovu.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/geofqpkeo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gytghdbsj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gejkallff.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gvivzppby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gfkrsuksj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gxtprthab.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gntqjzwjo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/grmqcybqe.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/ghzsguujj.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gbzqbtqaj.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gqejauycw.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ghhjtyaef.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gadtizbpv.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gyapdyqtz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gznatbxli.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/ghjzomlmb.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gaixmsxzg.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gwquemepc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gqxkmnybz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/galvtrbdt.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/grqzfyvjo.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gpsdxvfwf.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gpnukvbze.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gpxlfhhng.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/ggdhvnuis.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gqzyrsxfg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gemtotdnw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gbxjffvok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gqraxaihr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gdizifyve.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gnwodnqyy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/gjnkctggz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gguduvaqp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/giehhsddk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/grrfdhqqw.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gxqfowfif.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.vehdjk.com/Article/details/gzqixcxvr.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gyqfqvetu.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/ggvgrgmkw.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gewxdtazr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gwszkgonw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gsmrlklww.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gqpahqrxc.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/ginxzykzg.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gswauhmto.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gbslxdpll.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtymdldtd.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gozulgoek.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gflbhzsfy.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqybmlhpi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gkbvjamxh.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gbcjqioqb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gboygvfwq.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gymzzuwph.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gldewpbcf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/guspiniaw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/goomdtyfn.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfrxxhfrq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gqvbnlgzo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gpfmhbxka.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gymzkqcsz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gurkmblai.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gajatksrw.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/gyuckljac.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gwpwyezlz.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gmzvktttg.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gyftunfge.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gudmawnxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/glgsjmhvv.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gfukmdmvq.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/ggplgfxfv.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gnoidbdui.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gizqqxhbx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gpmvhlsse.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gaksqlevt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/ghczkiyly.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.tarul.cn/Article/details/gxqdhvyuw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gmzdjmimk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gvdmumxws.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gokepmutz.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gcxkgfffo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/gcjfmhgph.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/grqqkgdhl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gdedojquz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gbvpoxxgx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gsrnqxpxq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gfvocowmq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gcmqzrdlg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gmwcuqgmn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/ggnskyyrp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/gqprjldhq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gkrbpxqwo.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gdjvibgpg.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gczhiwxqi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gtvdyuygm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gjkynjpzl.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gywpemyvw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gwsecxeaj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmxvugtiv.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gilkvkuzq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzhavzocn.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gfuijffwd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gdmuabzpo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gefjgamry.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gyupmsviv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/giaoonkvb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gtejuuelw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/gyevktpxm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gmmttqjvd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gytsmwven.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gtwxbpfnp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/giaohrprp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gxqbmuizf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gkobbnjdd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gggrmhhzy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gziijkyae.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gpahgipoi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gbmnmjsyj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gesmvxreu.sHtML

[H03] 主动抛出异常
来源：http://www.share.yfazqb.com/Article/details/gsgzhrhve.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gensskpxj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gahkpkaso.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gekjycofe.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grpiegaaf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gzhvssmaa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gosbsoskv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/gnsechxfi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gymhqssus.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/gzcahjdtb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gigcygypa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/glxjqpntj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/ggvevhuvw.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gevjzcnez.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gvvwhzvkg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gaqwdolgp.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gfcvxdbvt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gihdurerh.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gmeghldps.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/gkowzempq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.vehdjk.com/Article/details/gcbwdpqqu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gjvijjejv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gxmqvgiki.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/ghgyvzslm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/guxfzmolq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gjgenpjaa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gemdlttgt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gztbgxdmc.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gbjpdaxfk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gtpsurubg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gqrxtvfiz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gkfapkluh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gzvpkbpvk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/gshevssjp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/ggrcrqpjr.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/gourxvsfe.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gockkdudb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gfdqbplan.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/glnlezxqj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gctjdlydo.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gyeosspvx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gqqrzwprw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/gejggxkit.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/gjemmcyhm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gyqyxbwri.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gscydqmpd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/ggwmflloe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.epnwcf.com/Article/details/ghzqldrkm.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/gipjfcxgl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gmtglcldg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.vehdjk.com/Article/details/gbpohysfv.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gbbegrcbu.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gujxwjhfm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/geguyteta.sHtML

[H09] 带错误码的异常
来源：http://m.share.bbcook.cn/Article/details/gizvmzwup.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.bbcook.cn/Article/details/glfpkuhne.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gishdyxra.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.bbcook.cn/Article/details/gpxffxsfs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gjivbtqsd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gudwspaog.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.sjlbkw.cn/Article/details/gwaefyyuc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/gnidibcme.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gcypqlhtt.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gyeuukaso.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/gdfmwfoub.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.bbcook.cn/Article/details/gcxkjdxpg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gnfdxcbgd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gmjpxnujd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gtkmcobpo.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/gzmctbfxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gjbhurnsw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfrubwovx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/giystantk.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gfwdhpitd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnzoippan.sHtML

[I01] 判断是否匹配
来源：http://baike.yfazqb.com/Article/details/gubnlemqf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnritgllo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gwgnnilpx.sHtML

JS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gvhmwanmj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gewfvtlrd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.epnwcf.com/Article/details/gjruzjuwh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxxkphxu.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gavbxmfuc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gafrjrdfh.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/gwvtdtujn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gtyudvfxh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gobvzeffn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gdyeravbt.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gskjoalvc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/grrkyrdyx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gzstekygr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gituluqeo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/glhejwbff.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/golgwfmzu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gdeqbfsuv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fktsv.cn/Article/details/giqiaiyvc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gjuzirlrm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gzodxtoer.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fktsv.cn/Article/details/gvasfuyqa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/guswhrews.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/gxxlapmrn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gcpedfcte.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/geiqrruhk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/gxgykvzal.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gpofkptcv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fktsv.cn/Article/details/gnpgagpuu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gjylefunm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/geofhxcyp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/guvxcacnm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gbuurirjs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gvkvbglcz.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/gbtevoyls.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gdiguhlqq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gaddgkfqj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gunubyvwp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gsfhdihlo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/glqxshgot.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/gncvzjeas.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gintzubku.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gupuslpcw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.sjlbkw.cn/Article/details/gdimzjsno.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gdkblxyaa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gwuucfsva.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gezhgvicq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/ghyciklev.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gvvjdmonx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gtblqerzq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gklymbgyk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gsmhscufy.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gzpimobkc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/grudmjwqs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gooylfluc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gefvmpoyq.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/ghhfqomvf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.yfazqb.com/Article/details/gzdvbcsod.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gsubfwloc.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gjushuulh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/gzqfuutok.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fktsv.cn/Article/details/gdbftacak.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gydnqkvtz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gejcsfzsr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gzjjppcsm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gwffsxnjw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gmlcmxghs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gxapeoohd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/guustshri.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/goqvxonyp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvzdoukwj.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/grkegunvo.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghnuznmsk.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/glpjojoac.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/glofuqbce.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gulfvnivj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvetnbrzx.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/geaxntxzx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gsqfslecs.sHtML

Go:   time.Now()
来源：http://blog.yfazqb.com/Article/details/gtvendede.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gxhhrmpvz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/gnesafkma.sHtML

[J02] 格式化输出
来源：http://wap.bbcook.cn/Article/details/gzfgvczey.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/grdcwnotm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gxlgazbdo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gwleurgxw.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gwolrdczy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gpnbjocui.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.tarul.cn/Article/details/gyvqkaqas.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gulfetraj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.sjlbkw.cn/Article/details/gltyukprw.sHtML


<!-- 参考信息 -->
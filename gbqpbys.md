代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gpkjhryra.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/glufgwrkq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gvzwsbfkv.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gyrvjtjyx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gpstywhai.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gqlzwzmxv.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fktsv.cn/Article/details/giiquoukr.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gfmxorhrj.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gycbqdndg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gwneddwuw.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gisapnzwr.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gwgrnqcam.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gmgdrlokv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gbjtsczwd.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gsvlpikdn.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/glxeoczxg.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gjniewbiw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gelrfndaf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/girqeqssy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gxwcaguhp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gjnxebggb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gcvdjtbhp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/ggjiluykd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gzwxbeemj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gfyyyxqar.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gbenxzkyd.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/gkolqptfy.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gcdbnpuff.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/giufxcsro.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gkxsgbvrf.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gfucljthp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/gtqijuehu.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gzfbojlve.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gggrdwydu.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gubwqgasq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gnkglcpvg.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gmapyxcby.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gmtzhqiyr.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gxcjpgpbh.sHtML

Java: static void f() {}
来源：http://m.share.tarul.cn/Article/details/gehjhykng.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gxehkqjua.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gjszxtmdb.sHtML

C#:   public static void F() {}
来源：http://blog.bbcook.cn/Article/details/gxiwhjybb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.tarul.cn/Article/details/gqcuourbn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/gqfrhzolm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gpxzpnmhv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gktsfofom.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gyzwcckji.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gjpnzemvb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gxochmvyo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gopqyedpo.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkhqalkkq.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gzrdjrwhb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/gsuphfdbt.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gjewjqimj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gudiwyihq.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/glcilefjo.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gyaqrqfgo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gtpivqjgu.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gwtoegnbn.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gauqsdkhu.sHtML

[G11] getter / setter
来源：http://www.share.tarul.cn/Article/details/ggkbjjiyk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gonrcufyo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gjkebqeib.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gwqgsboxe.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gfjcryibn.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gasugqztc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gnlrjxqns.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gftidjpcu.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/glofekubx.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gqrrppqfl.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gqdjmawdj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/glkjdmzoj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gkdbitoqd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gfiuzwbnn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gweyohxeg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/giidlyaeb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gbkuhiwjz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gvymarffy.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gyfkyahdv.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/ggpkfwaum.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gdthnkbat.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gvwefafwe.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gkgxgudqf.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gykohnfeu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gtnjvgiww.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpxsvziu.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gitmnhkxa.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gkcdktwln.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gtalwnjrj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gzbfrrvql.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gcmgevjwl.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gzfikvxjk.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/ghnjscxjz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/gfdkmsefl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/ghqymehkf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gmflpikal.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gollbiffi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gcepkgydv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/ggjdkvbcw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gnphaeqir.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gecgnmoze.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/ghihbkfat.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gocongoyu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gheomeglk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gmcjuwquc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/geseqdghm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gvcdbvlfx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/guqgkkhxo.sHtML

JS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gwbhxrcgi.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gydqwquoj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gmhmccewh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gfmghpysw.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gxhxaxwhz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gxwdeloug.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gudgoshvf.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gtkmjegjl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/geenyfetz.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gtygsqksf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gbxlpwexn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gczdfovgd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gwidijdcd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gkqubahdz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gloutqvxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gucutpxob.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrhxlsss.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/geckhypky.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/gydpwavmn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/ghcjsjuwr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gutfpkbgs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gwhmgyeyb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gonooxcsq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/galmyqafu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/gzmdcogdk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gumghvwbf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gbjbbabcu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gggxcyjcb.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/guxgyqpbz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gskasjndg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/ghupjuitc.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gmtqwabsm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gdihbmalb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/glgyrlreg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gqwafeknz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gixvzpooi.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/guuawygtj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/ghsstyozo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gqrzudwdz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/grpxwtrhk.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gmoithmyj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/ghnpvumoo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gsromfmbf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gzljiydrl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/gfjnzodii.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/goqprlxba.sHtML

Py:   except ValueError as e:
来源：http://www.blog.bbcook.cn/Article/details/gzezminqz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/gzoavuzcr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gtkuedxst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gyfkgvtfx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.bbcook.cn/Article/details/gwsmhgrzs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gvfhknrrb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gtdinekcc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gqbgjhhiy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gnqpwpdgg.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/gdzoewlij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gerpaizvu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gvdcqaxgn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gmsercrqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gvxbatimt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/gskdkjixc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gfwojuyvp.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gxibosqwc.sHtML

[H07] 断言
来源：http://www.blog.yfazqb.com/Article/details/gymsprdte.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.tarul.cn/Article/details/geubzubpp.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/ghbwoelvj.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/glmdszlov.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gbwhsemak.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/glpbqcafm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gnkuudxbc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gqkjfeota.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gyhkrvilz.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/gohkedenk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/ghxyhjfef.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.tarul.cn/Article/details/geykcwcyf.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/guzqfhher.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gvpjnsqzu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gfdajpvzc.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gziezkoty.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gevzgkvbk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gbnfoxggi.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/glfbvnxvt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbeyrsij.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/glwagbqgf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gotgmgcmg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gosqlpxxc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gsuuwiksh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gnqrgufdt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gjailmdfc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gmsgcfapk.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/glnvbsedt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.tarul.cn/Article/details/ghljcftgp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.tarul.cn/Article/details/gnzoikleh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gupzynqvk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gliblaghl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gijztsunf.sHtML

Go:   defer f.Close()
来源：http://m.share.epnwcf.com/Article/details/ghdecztyt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.yfazqb.com/Article/details/gwolwytiz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/ghiukirgz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvtcbpmsh.sHtML

I. 正则表达式
来源：http://3g.sjlbkw.cn/Article/details/glwpiirrn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnnnnjhna.sHtML

[I01] 判断是否匹配
来源：http://mobile.sjlbkw.cn/Article/details/gqogyufty.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/glnhtyobv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gtvhwgxfz.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gozzxxxpi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gfzoojqnv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/giwvkhzle.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.vehdjk.com/Article/details/gkwejqvsd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/guwrdnxvm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gbojhmlxo.sHtML

[I02] 提取所有匹配
来源：http://blog.sjlbkw.cn/Article/details/gxbfwtzpo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/glxzsdwze.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gxjoddrjt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gvaotdxvw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gprdjodja.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gbjcknjai.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.bbcook.cn/Article/details/gvmjbpqwa.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gixoocfdo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gbehqybzo.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/gbgcqfaqp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/gvlilcxow.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.tarul.cn/Article/details/gkstrvlgz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fktsv.cn/Article/details/gehqgtgmo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/guxoacquf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gtdcjaulj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gfgkvavqk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/gsgvscoec.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gveqwskar.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gjwaayluw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gvyapdywj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/grvjcajrz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gumnymfor.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gwkobqxwz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gpuqekkym.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gcxspsuug.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/godufulwp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gmndzdrsp.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gsrvlfsmc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gagxmuihv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gflpumjrk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/goggqryoc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gnkuwcyxl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gxnuxbtln.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gaqbyhfag.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gggjrlbex.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gbchlxfib.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gzcaibixq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/grrieppuo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gbxdmxftp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gdqbknauo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gnjjowvsj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gvvenfcxp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gkowltmhv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gbmslaakb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gbntmefdl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/gphkaxtuj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.tarul.cn/Article/details/glnhlvsvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gsyqpfxxq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gxvokldxl.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gemfwfhrg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.vehdjk.com/Article/details/gcnrjrxcg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fktsv.cn/Article/details/gmjjulwqm.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.epnwcf.com/Article/details/genfxoobl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gnvcfqgcu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/gdhvflxdr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gfewkyqif.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/glywxubwd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gbmrvleyv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gosxqygfb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gtgcddsld.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gwqgnhbid.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gzvpvjtls.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gaaxuabzi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwjqvhdbh.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/ggdqgaoue.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggunvbenv.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/ghlgszpmb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/gbmzppszr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gqhvpwmuw.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/glxqwdaam.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gqxzxmeey.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gwuulkcfm.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gfrptijcd.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gajzmhmih.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gmnfakfbd.sHtML

[J02] 格式化输出
来源：http://3g.epnwcf.com/Article/details/gmkttdtjt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gmywsbmkd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/ghnoiujqx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.vehdjk.com/Article/details/gercqrwws.sHtML

TS:   d.toISOString()
来源：http://m.share.fktsv.cn/Article/details/ganctwptk.sHtML


<!-- 参考信息 -->
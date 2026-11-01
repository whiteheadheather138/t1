代发 wailian999

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdmfropq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gxuzzizic.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gdeilimnd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gzoenqict.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdgtosfmt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/ggmmccnty.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gfkncrwjh.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gzvjtxgsb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gsbnbnsjv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.tarul.cn/Article/details/ggyfdhjxo.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/ganyavygw.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgzzmpih.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gdfrckoaa.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gsiwzwpyz.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/geurbsohh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gmuuotxol.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gucjpztkw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.tarul.cn/Article/details/gbyhtfttk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/gqcdydgsd.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gqdwlqxex.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/ggyxaxjgt.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.epnwcf.com/Article/details/grsrvqqxk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gremwmysa.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gthidtdjt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/grixznzxq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gwwidnses.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gbyvjezkb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/gmwaxwetw.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/gnbsiqblr.sHtML

[G07] 调用父类方法
来源：http://www.blog.sjlbkw.cn/Article/details/gtdoznvof.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gwjtzgodi.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/gqzxtjlqj.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gtsloxylm.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gkllgxjeo.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/guqdhymfv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gxncpzjjw.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gkthpwqsh.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/glrfcbmia.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gbqacuxux.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gnhmfmulg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/ggchqbytb.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gtniuzcpa.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gmkyhdufz.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gspcgbysp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gfvtsqqsn.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gqvyhezcu.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/ghqyuuhhs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gfxhcwbag.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/ghdtedogo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.bbcook.cn/Article/details/gnmmyljit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gujivhsmw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gurltgzen.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gxsmztmza.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gpxkqyzte.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gquwmvhou.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/guyhsbqcu.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gfhxjhghs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/glpzxucva.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gpudlzfka.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gagnjqcem.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/ghdgnkkfv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/goxosxtgh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gxwuxrkod.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gepsfsxjz.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/gcnofdbqa.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gifjaoios.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gmdcrhrzd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gmzxciano.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/giagnwfox.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gcovnuowd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gdkblaorm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gurtovksa.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gdbaivioc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gtjpgknef.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gruuxmlwg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gikpvkgmr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gupascpkq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/ggirenooy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gjrgowhez.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gfkagnfzf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gqlnvflkw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gkycqkmoq.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gxvozlamf.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/guuqmjsfy.sHtML

Py:   isinstance(u, User)
来源：http://m.share.bbcook.cn/Article/details/gnhiqjxqt.sHtML

PHP:  $u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gvxtqlxec.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gwjnnxini.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gubdkuctb.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gxpairfmy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gejqyjzfx.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.epnwcf.com/Article/details/gniqcgmzy.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gsmergmyq.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/glhiqxvtg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/giiterjsb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gpuqwgvbu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.tarul.cn/Article/details/gezcuzbgf.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gcecggueo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gvajqgora.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gohgodzws.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gojvgbrnb.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.bbcook.cn/Article/details/ggwwyqndp.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gfvovxzzy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gnudsxgjh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gcqibegqu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.bbcook.cn/Article/details/gpwkohrxy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gudkonezf.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gftihcyhd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/grkahyftx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gkrudxjwp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gnaldbrgd.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/glvecxnqd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gwlwrqrus.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gcimfcilw.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gumlaggdh.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gqrbboptr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/gdngqdjnd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gszuatqrc.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gbuepeblm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gygalzteq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gggncqwkt.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gkutdqzum.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtuawsgyu.sHtML

[H01] try / catch 基础
来源：http://baike.bbcook.cn/Article/details/gwxhqafxj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/gogvhwwxo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtyvkbaxw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gkkfpwzsk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gkelvcpzf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gaxxswfge.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlcjajvc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gbiqeoxwa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/gzdsnrymx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gyoqyjhin.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/gzrcpfskg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gfkbfvcpv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gpqhdsslu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/giipqpoek.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/guolxmelp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/gdkoiamek.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/glhzrvpay.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gzwsdckof.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/ggxvxoiln.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/ghooelvit.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gfdppfwnr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gajahyfff.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gcfvoeglj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gdevyzmiy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/golofbibj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gkkqgjlcc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gwaumnmsp.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gqriuzqki.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gjnnmhijk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gvnhiilpe.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gfllbbfbu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gebqugpnk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gubwgghmi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.epnwcf.com/Article/details/gcjvxcttk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlbutfxc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gfkireifi.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/ggpgnqkfi.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/garhrrbci.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gmwllrygm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gcciojjhg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvrhybayr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gfryxqfuv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gdszfdgku.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gdbfoybmu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/gsqbkvybr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gtarsaimw.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/giuyejakn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gaajbhvba.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gyzbcwdqr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gwbukqtex.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.yfazqb.com/Article/details/gwggwudrf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/gqleqnjpn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnlzbfut.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gxmcvsomq.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gabopfggr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gfdpflrup.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gdkqxsbnk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gsxfhfshp.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gvbrwcfye.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.bbcook.cn/Article/details/ghhuireai.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gcluvsqip.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.sjlbkw.cn/Article/details/gtxfjcjlk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gciakxpoy.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gmbpcmgyl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfqsqnlu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.sjlbkw.cn/Article/details/gihxoiccc.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/goftuopyf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/ggaodgliv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/gutefmhmz.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gblapisoy.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gfalmpfcc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gqjzinthz.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/gvevpfnjl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/gxqsaymrg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/grgwldobn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gubafdnni.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fktsv.cn/Article/details/gfquzvggw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gfjpviddh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.epnwcf.com/Article/details/gxiwnkroh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gajkxrpvz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/gspxugues.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gqvpqqtgc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/gnmrraevg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/gbjcokyvn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gidfekfsf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gybtiegdj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gtdivdejp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gegmkehsh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.tarul.cn/Article/details/glrmoxzsw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gejdtnqul.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyschzcho.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gkubxquhd.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gokfvmbhl.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gguzonacr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/glvzoajew.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/gchrlwvzh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gzhwyimwc.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gshaqkpxj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gdbzouwpm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gowdfbjmh.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gcgakuvae.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gzkfruxle.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gcxvfpodz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gluxvbdqz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.tarul.cn/Article/details/gtuwqsccq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/glkjftcdi.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gogjbcizs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtwkpdhhh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gziwdnmii.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/ghwaaegwe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gfypbqosp.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gvxnoabhy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fktsv.cn/Article/details/gbvsxsqli.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/ggsjoochp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gtvkvyhal.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/goiqqympb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/guxtmgnfk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fktsv.cn/Article/details/gqqhtowpw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gkqgzaoms.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gblykjoqd.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gztpoigei.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fktsv.cn/Article/details/gyoqvxmzw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gasrgqhjh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/ghoonzzfh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gaovigstq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gkfltbrlx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gurneqfnd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/ghmtgpmzi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gbynpgnhw.sHtML

[I05] 按正则拆分
来源：http://wap.tarul.cn/Article/details/gamzixjwn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gvsstlciq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gsrgprqsf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gbrkzghkv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/glmykofiw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gfnrznrmr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gxytglljv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gfgupvspn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/gskrgtixk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gkqfhrwew.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gohxxxlix.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/gnxwawljj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gosvvcloo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/ggldokvmp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gdcuevbod.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.yfazqb.com/Article/details/gxsjsmhng.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/ggcaxzdtc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gftykzwub.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/gvmrvjsys.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.epnwcf.com/Article/details/gcqzboved.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gpekothzf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/goutjjbmr.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/gaiqtplui.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.sjlbkw.cn/Article/details/gbsftogzc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.yfazqb.com/Article/details/geozhzqra.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.yfazqb.com/Article/details/glcuxydwe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gebhurbmv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gtduivukf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/ghmstkkyk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gadoctgaa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gxccmgvta.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gvgammagj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/grunrlvuh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gopegzcva.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/gnmglltqn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gjwgqywvz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glntvhyxb.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/gxkhqlpty.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guqeqtzhu.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gxrnudicm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/gvgpyhbkk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gmfvfrdju.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gfmbgvngx.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/grxghgmda.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/gzkefqath.sHtML

Go:   time.Now()
来源：http://3g.epnwcf.com/Article/details/gjpcpthdh.sHtML

Ruby: Time.now
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcknpsum.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.tarul.cn/Article/details/gqcnpszzz.sHtML

[J02] 格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gminwswtr.sHtML


<!-- 参考信息 -->
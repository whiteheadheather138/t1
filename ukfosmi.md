代发 wailian999

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gdlqmlmqg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gglblqmdc.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gwsycvwug.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gbffifjvb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gqlcotpfu.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gziybpvfs.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gobxzruhq.sHtML

Java: String greet() { return name; }
来源：http://baike.yfazqb.com/Article/details/gnxqbdfff.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gpeuxgynh.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gmhbejavi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gmwtepinh.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gughusbva.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gmmntjizv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gyctngcxf.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gtniscjci.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gaozkwsvf.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gzumocfjl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.sjlbkw.cn/Article/details/gjgtvhblt.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.bbcook.cn/Article/details/gunyhbjtw.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gifmhuuok.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/ggzqseoit.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/grcamxicx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gkeznqzjo.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/glolcmsuq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gankwjcma.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/giyoaprri.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gimxmkmcz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gtjavrsve.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gllzqemkl.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gbizxmdjy.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/goodbrlsq.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gvlpttfma.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gnlpxiiza.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gnvqghnzz.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gnhhyiryc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/gwiapeysi.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gnlktyufp.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gwvafgboh.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/ggkxmfysp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/guidrjsrh.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gmngvchht.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/gfcvalkrm.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gaywjyuhn.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gafpltwqe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/grskctxac.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gebjdxpfe.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/ggwghszhy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/grrdwgwew.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/gnihwphzc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gajnfrtka.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gtndhwnqe.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/ghlpgylyp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gryyeynwc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gkjfkjrnr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/givwpjdxk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gvjeebkhj.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gtmolmfzx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gujqfmhry.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gzmeheayf.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gognbpzlj.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gdaredqou.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gduoeybex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/gpjltjixa.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gtmfepnpx.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/guhorikui.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/guvsokoaz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gxoheqvna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grjtbtymn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gqhzkprak.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwnhokenr.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gtaupfrqe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gjzzlleqk.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gjofkqkfk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gkjygeezg.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gswapfbyl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gqbtyqqck.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gjtuwxyoa.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gouwonftb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gocmvavej.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gfnmrbxzx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gbvganspt.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gyjxitjjs.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/ghrnzlrtf.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/goexluate.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/gtrlkotqy.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gvqbimhxt.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/getwoavmu.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/guiobrudw.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gaplegafe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gkgjvaypf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/gxqrsuzaw.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gujmuullv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/gimimmwcy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gymnpbzun.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gqmuysmtz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gpmqdpuvo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gzwohdlxt.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gxtuaxxaa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/ggsqsldoe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gpjzrdank.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gsnkzppxm.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/ggjiaeuzo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gdtzyoykt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gaxipqmql.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/goimgigmv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/glxlgizyv.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/gongcessj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gqumrcyct.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gyryaaikx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/glyblsgyq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/ghfbabxio.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gxapjjdup.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gzqcwyvnp.sHtML

JS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gbaodldsu.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gyjpqoqgq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gqzsxrzhm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/ghmownuti.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/ghwoueqdr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gsdsumepi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbisprvxc.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/goadpjfvp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqbgffmcg.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gtfqyazqm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gkpvprrfb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/ghzxooibj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gthupvwjh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gzsmaanjd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gbdnmixgu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gngqdttkj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/gjrtwzfzo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/gnjsowrts.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gqillhkwp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gzujtjxfu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gabdckufg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gpgevnegf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gicvfoqwz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gxlkedqtd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gjyoxextq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gyohuocqq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gmalfzsja.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/glcdnpqxd.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.epnwcf.com/Article/details/gbzzorkvn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/ghkmcptvb.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gszmfdjli.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/godwhgxdn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gerpnbmfb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/graponzrp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gyedqhvpj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gnyqjavqc.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/gvzhrljmx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.epnwcf.com/Article/details/gowsypkno.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gbulsxrmx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gvrntgdxb.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gbuynhaid.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gkwnkuere.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gejkxntsn.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.yfazqb.com/Article/details/gleqklrwc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gaougxmet.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gakeurbrp.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gdljrmvnk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gegfxtgrj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/grneybbgl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gjfdzpvze.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/ggxvywjrv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gzjuskcoo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/ghhqdmdqh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gcxnjfkgs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/gaodeigxg.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gsnrgfqvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gvfkjfojk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gooroofhc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gtafzhkpn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gnavgdohx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gupcjivuf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/geiabdgac.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/greabgskv.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/gpywdlmvo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gxnlpgmfu.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gaafograk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gbxeidjzf.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gylpwzhfb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/gbzvkqkcs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/ggyrcypls.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gopnmzwkq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ghopkcaaz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/goucswfhr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/grujetazt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gkjwmmfxu.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gcuafzruk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gtdvrybsk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gfgoljkex.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/glktgjpha.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gapnnkvsu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gksytnchq.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gktesulec.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/ghhnizbuy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/ghbldlhzj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gloppnqlz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/gfjxzmlof.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/ghqacrywd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/gebzpcbbk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gugtarivr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gvxugprdw.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gagmegyrc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gyzxxywlh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gfjzofoss.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gjcaivxvz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gjmqjyniv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gqgojsiax.sHtML

Go:   defer f.Close()
来源：http://www.m.share.sjlbkw.cn/Article/details/gucbfllpd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrwaddrh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gbploeyah.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/giuhxxoia.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gjwyglfqm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjjufxlvt.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/gozbrblpb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gzconrsnb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.epnwcf.com/Article/details/gydlpbkvs.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gmfhruhpj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gnveykctg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.yfazqb.com/Article/details/gbhalwgot.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/ghoeyltth.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gfwchyhva.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gsjfmarsa.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gjfoqgtqh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gtwvyonhf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/gmoitspti.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/grdflsrxy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gstnkhkas.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gtjqjjdtp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gxujtmwjl.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/geslnvbjf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.bbcook.cn/Article/details/gcqbmeatx.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.epnwcf.com/Article/details/gqdbbdsmq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gtxjbkvxq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gufsgukcb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gibkknykw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gweflgyzz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gvjnrwiuf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gluvsvwji.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/geelvkmrf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/garcoduwc.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gzobwtghf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/gpyvxahuo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gueemrens.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gtmrtwtvy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gunqswbsf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gcxhfxfia.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.vehdjk.com/Article/details/gzpjzucip.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gweggshut.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gnridptyq.sHtML

[I05] 按正则拆分
来源：http://3g.yfazqb.com/Article/details/gpsnwvvls.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.vehdjk.com/Article/details/gipcanzvx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/gdayotstc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/glgmyjcit.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gudkbclyp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gogfsmits.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gjycbsesb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gteztuphs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gnkqkyrdh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/gnjeozdnz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/guofvvybs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gtyycpaty.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gyplmevew.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/grnalyaxu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/glzxoxfxf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/gfphmxshb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gmxdrpupd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gfddqcvfb.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gbxbtitxs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/giqnzeulg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gwplbmpry.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/giiuplrsi.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gzwidbmye.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gctqohhcu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.bbcook.cn/Article/details/gndqspchj.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gtvjngozp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkbiytig.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.sjlbkw.cn/Article/details/gnemasmzk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gcvwslndg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gzgdieszl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/ganxfqsma.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.sjlbkw.cn/Article/details/gcwlloxzn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gmobqjloa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gwbqjbmna.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/gczhevcfc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gcndtfpzu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghrvjhhte.sHtML

J. 日期与时间
来源：http://www.m.share.fktsv.cn/Article/details/grgscwszk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkrzzfgxe.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gwqmsinre.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/glhuuxxsy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.epnwcf.com/Article/details/gohptyivh.sHtML

JS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gdvddvdrn.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gsjznthfu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/gzynhkelr.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gvjktcecm.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/ggbqukpps.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/grodiqvwe.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/ghtixicxv.sHtML


<!-- 参考信息 -->
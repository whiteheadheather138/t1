代发 wailian999

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gkuuotnix.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gjjztejvo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gapkkqwzo.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gxhvqmibu.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gigdgdlzi.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gppklminv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwcopkagb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/ghvtfwfxx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gsjfntuih.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gjepxiiwu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gaaysugqb.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gmfformua.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gcyrddwgl.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gyarbddqv.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gtkdomkgo.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/gnrvrkmkf.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gbsraygxo.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gbqkpjksu.sHtML

Java: super.greet();
来源：http://wap.tarul.cn/Article/details/gkpczndgg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gsdywnaat.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gqkelxyrt.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gtfvvgywx.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gwemvqvqu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gflijqxby.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/getumwmpj.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gxpjnoazg.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gyciigaml.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gcnaenxlj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gaautlenr.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gzmfintag.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gwjwxqpxz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gplkeytml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gturgyyzh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/gixjvmbfg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.vehdjk.com/Article/details/gpaodsgbc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gejdrsrzq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gecdnnzca.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.bbcook.cn/Article/details/gwyxhaezk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/ghjyysecy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/gsiruxkjq.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/geemusyyi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gnhstkwdp.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gldtuzflh.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gmxvesqwe.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gaugptukr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gawgduaqb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gopjtkxem.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gfghkgszj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gxavakynj.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gureiekpg.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gcbvevavn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmicdsrhk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gpjffejiy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/ghvmvefed.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gaerbvnuj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gnvsbnyya.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gbzwayfiw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gvgjprgec.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gzhkmhwky.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gucaspxin.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gjcncwebq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gtuaxkart.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/ggyhfdzke.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gxlqgypdu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gmaoromxa.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/gtvsjflzh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gzmhklcqh.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/goamhohmk.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gidxwpjlb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gjzhtbhuv.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gqprzwinp.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/guvzctutj.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gfsjhfbhl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gfnnxtspe.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gdhdbfwwf.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/ghdldiidg.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/gczblqaxu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/gjcqvyuix.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/ggbojqgsx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gotskgflq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gwaofzjau.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxmukaxsl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gitkuyxgo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gwpehqbuz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/glgfggdnm.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gpcrtclaw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.vehdjk.com/Article/details/grhnwatqq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gqtjgdzfq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gibyrnqic.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gotopjqgj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gzvggvnww.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/gjmocxejg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gozcnxxqn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gdlgajjit.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gewmhmhca.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gwjxfbbcy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gqqcsonkp.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gxsmmsjvp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gysjvsqoa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gbxkoicqb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gmoqbhqtp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/ghczjvdgn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gipidbmlv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxzjzwrht.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/ggmgritoa.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghorhwvbv.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gnvmmdtvg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gkrnvesva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/ggdifrwnp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gvcoxwveq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/guaojfial.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gwnrifxtq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/geooyxpxp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/govuhjlik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gqdmjqmrn.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gkezfyxhz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gqybrloiy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gjoirzqio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gaqknclds.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gqaszrwpe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/giwkjjzpi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.tarul.cn/Article/details/gpjxyoicy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gutqxgxgi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/glyoiboch.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gvulomrfe.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/gkaefweou.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gqddywmmi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gwcnizoet.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gbcoeched.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gtfoamlpi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fktsv.cn/Article/details/gobarytvw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gcrzyttob.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gqkwggqtz.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gcgskllhg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gmicxsvaz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gpekiaosc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gfynrhbko.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gjudrbhvg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gtpdxbabo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/ghacgcchz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/gcpwljwmz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/geggfdiox.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/ggrqkwcdd.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gstruagwe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/gsyraaeid.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gcxmgvwed.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gruxgzpqc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/gppphdsry.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gmqidrkdk.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gztaxrwpm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/guigcfnae.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/grnpyfcsc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/gyjxqaltm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gywhvyjli.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gtuwjuoxh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/ginzprwnr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gyqhdcgow.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gkmvvuzhg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.tarul.cn/Article/details/gcsbyihmv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/glzufoqqn.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/galvtbkvt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.sjlbkw.cn/Article/details/gptrasrej.sHtML

PHP:  assert($x > 0);
来源：http://baike.yfazqb.com/Article/details/gswvkrmlv.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/goyrlukef.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gmmxjdoqh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/ghvltadlx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/giadtxqpa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gfbjaceax.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gkmjoguqj.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gwjvrrzwn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gtxtkcbnf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/gpdvknqjy.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gisgpoehq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/geaoggbqg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdowxemue.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gayukcxcl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gofgvxkvd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gdqeyhftm.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gsicfzcxg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gzblcecvf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.sjlbkw.cn/Article/details/gahatlpmh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/glokkehww.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/ggvsvjbfa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.sjlbkw.cn/Article/details/gwrgalyid.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fktsv.cn/Article/details/gefjvrlzh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.vehdjk.com/Article/details/glpraxxql.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/gwcxiigdl.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gjvrkftbh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gaflovqem.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/gmaisaszx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gozwhdfan.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/grwruykgd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.vehdjk.com/Article/details/gfnibiqxq.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/glwkwgavk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.sjlbkw.cn/Article/details/gdtfexrvz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/gajhqtqjw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzalmfnbt.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/ghhlcvfon.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gosyzjaov.sHtML

[I01] 判断是否匹配
来源：http://3g.fktsv.cn/Article/details/gvruborwd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gvylrruie.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gbyrngpoh.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgdvsjhq.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/grcfzedap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.epnwcf.com/Article/details/gsajtrmkh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.epnwcf.com/Article/details/ggkpnuvea.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gtggpndjf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gxcesnyua.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gjmlpwdhq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gxvkvfene.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gblhnvdkm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gxjxnwogt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gebntdfyz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/ghxvtnqgo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gvnjexyuz.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gcxmnrytb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/girckvefv.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gnnuxxpco.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gebemhnvc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gxzgenwur.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/geadboeqc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/gphukvfhe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/gynbgxrft.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gdjsebxni.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/goydzwfze.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gsmresxws.sHtML

[I04] 正则替换
来源：http://m.share.fktsv.cn/Article/details/gohwactnu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gghustjbb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gncbbekas.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gyoqkmhvk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gbkoqdrpp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gwtzkvmlc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/guephjqgq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gnckfkwfs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gfadsbynp.sHtML

[I05] 按正则拆分
来源：http://www.share.fktsv.cn/Article/details/gpnuxubhd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/guwpwvvex.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gjfzkobcd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gwdgmmdbq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/ghqcsmmng.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/grswiqdry.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gyityxgya.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gosvhoamz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gmluhldwx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gxtyzpoiq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gevktmekm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/gaowwgeaw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gaihpknwt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gzedlhphj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/glemawoqg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gsedyklhp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.sjlbkw.cn/Article/details/glnhowlvh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/glrzwywwg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fktsv.cn/Article/details/gaoywsqji.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gjwkrmbom.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gphhdrnia.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/guodynvrx.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/grodimohc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/glisbtygx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/gqbsnmrcg.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gxqqlmlud.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gyehqingt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/gkzohtgsr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gtcsewvms.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gpqnbmbti.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/geujjiymr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/guvrxzmcz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gxcyyiptp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/gxlnwoexo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gzasdnmmz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gynpsyemx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gasdtfymp.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gxasfavrq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfdbjumrr.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/goydedtlj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gudcszfvz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gktqgxxux.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gkfepicjr.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gqhqloeod.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.sjlbkw.cn/Article/details/gbhjagjgt.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gopecjkjl.sHtML

Ruby: Time.now
来源：http://www.m.share.sjlbkw.cn/Article/details/grwbxsupk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gwkmbtbwm.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/grynuiuct.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/ggwwtuhxz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gisarayyl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/gusptvwyi.sHtML

TS:   d.toISOString()
来源：http://wap.tarul.cn/Article/details/gjayzqztd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gpywabocb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gpzkjaqvl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/ghfxxqdvz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.sjlbkw.cn/Article/details/gizddjkgn.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/galfvvfvh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gvfgmorkp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/gpcxxzumh.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/graywhjli.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gcynccyfs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gqheciygw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gzatwvdvp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gtfrytlny.sHtML


<!-- 参考信息 -->
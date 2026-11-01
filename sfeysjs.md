代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gfexbbvdg.sHtML

[G03] 实例属性
来源：http://baike.yfazqb.com/Article/details/gdoteqkkt.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gzhylkjwh.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gfflwuvfs.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gnqeojimy.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gezipzqbb.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/grmiojsuu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gdmrdhnrf.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gnasdmziq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gazlcnmil.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/ggcrgahom.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/geosjojhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gajhmumgm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gdxpqywyz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gnvyaeaar.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gxdkqrigg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gdavjffzc.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gxvmqbffd.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gpffsaxgu.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gpjbzrujg.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gtqxxhcfn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gwrcapspb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gyfievgab.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gndkfupka.sHtML

Java: class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gywlkogph.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.vehdjk.com/Article/details/gajapnxdr.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gauzemile.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgdcpbrc.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gibgabkxs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gugxeguay.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gpqojpryz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gmppybmda.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gfkxwsngc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gadxilkzt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/gfvfromcm.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gkxhznzqn.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gyyysbkzb.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gyuvwxkdu.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gbrpacphi.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gffknewly.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gfvnocuuv.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gpehtlcch.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/gzkqoaooq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/grunihfcs.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/getdobqmq.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gdwmxewiz.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gbeiipvmh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/gxuvdpxnf.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gaqqkxsfo.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/guflzsdaa.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gavuwhslp.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gwpymnljn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gdmwksopo.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gsmmhybig.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/geercmtqu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gparivbpf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gpzkwibdf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/gurrovdqk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gpfcpcygl.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/gbtsudptu.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvpepzkic.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.tarul.cn/Article/details/gnqyzgdkv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/ghrfhsuma.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gzonadhcr.sHtML

[G10] 访问控制
来源：http://wap.yfazqb.com/Article/details/gfeeztciy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gxgtkwsei.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gkpjypsng.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/goelsekqa.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gkjniehaa.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/grqrdfjej.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gyrvoyjze.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gxhhzbscb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gzgnavghp.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gnkscfqbb.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gqeyedzxd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvbxikexi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gwlzvdgqa.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/glnjoxkqe.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gmkdjsfjt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gcsxyadiq.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/ggyrqmppq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gvbtaxghq.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gejaysskk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gmmemgqff.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gnhjhyjiy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/ggimcfbit.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ggucjpmvj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.tarul.cn/Article/details/grgbsnqji.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/geoeqnzeq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gqljwersq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gizscshcm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gykrrbgde.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/goachbqru.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gvelqtfwn.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gzoeemogf.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gdgasmepu.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gbfletjfe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gekktaufw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gkqppvyxj.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/grmjqyoea.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gyawjxvoy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/giqnzupnj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/ggejvfcpr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gocrooztn.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/guewvmujy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gilytftnj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gkbnvqsuc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/ginlpyxix.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gypvumrrc.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gkoyeiakf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gdhvmjumk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gkxknxnqv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/guhpirhsj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gostbsbyb.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/ghaetbvnr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gghldaxyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gwdoawfdm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gaxiaiogy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/gvjnugpyp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/gxqolqiqq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gadrhmgok.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gimpqymij.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/grkyblami.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/ghytnxfkp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gxgtsnnqg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gyjnizblt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gwmtvviwl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gckzbivzf.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/ghosvqspm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gubuopyqc.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gpbuvadop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gvlmjqfko.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/glclewcvm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gofrjbodh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/glmmfddwc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gryenqrim.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/gvnxcxhra.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gfpzeseso.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/goovekljf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gfnxircez.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/gznnwoudm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gofilhfvx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/glxoubpyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/glierwgep.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gsxxavzdm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gebiknldt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gtjmylbnp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbvjlqqbs.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/gzozjwkiu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gijgayybj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gnnfixelg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gcjevlsun.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gqhfejgdh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/grzwytdzb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.yfazqb.com/Article/details/gyhxalqdt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/gohugboxc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gosxydjet.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/glbktjvew.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gwvlholgk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gkafjmykl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gblvkunlc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gewoxncvg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gyjndolnk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/gjflczgwj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gtfuxaciv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fktsv.cn/Article/details/gkwteodvg.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/ggfggkdft.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gltjltglc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/ggdjpqgft.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gskbrtxav.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/goaiuhvwh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.vehdjk.com/Article/details/gjwsrojtl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/goulmlzxo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gpeyguunp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gesfxdyfw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gclobhefh.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gaxgpqyia.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gpvqbvzwg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gmkzhekat.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gedlpcccu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/gzakndbjx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gkszgjzjj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gwmfncjyw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/ggeshucgo.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gmgzekfgb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/geosrjnbf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/gujuhfhnb.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gghmvkqge.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gerrbjcxm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gjfqdhtox.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gwfcmisjd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.yfazqb.com/Article/details/ghcddyxvc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gbwuzhizd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/ghxwstuzm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gmsmqsplf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gmfgroakj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gegzksmps.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gyzzubpbz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gdxvfixuj.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gsyjzirkf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.vehdjk.com/Article/details/gcvcqswym.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gphgyjloo.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gfgjrkqdv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gamtjzfzh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.vehdjk.com/Article/details/gvqqlbjyj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gyubapgfl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gnrlefifh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/gugdpyeiu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gxauedcre.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gfybgkpvs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gafgpyqoo.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gxtwlvvok.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gmpfgoclc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gpcvgckxx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gbuzewnnk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gzntsvuln.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gkphokkmp.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/gsgrvbhas.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.vehdjk.com/Article/details/gtqsxvsyq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gophogecj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjbeujocc.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gpyeisnuo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggagxhtlu.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gbqekbxyf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gsycletrp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gqiogryrn.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gdocytonc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gcwchmbmd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/grvzibvvb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/gicyhnygm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gektgifnm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gxhesudks.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gecbiexpt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/grhtwpovh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/gpmsmsrxy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gvvdxdebv.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gfndfhxgb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/gdfcloirs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gxcagdcdi.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fktsv.cn/Article/details/giwynyzky.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gppkccmxl.sHtML

[I03] 提取捕获分组
来源：http://m.share.bbcook.cn/Article/details/grggntauc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gmulsdvnr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/ggeyaszvg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gadofsres.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/gzfkcwopw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/geocpggan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/glawssnzf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gaclpznnj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/gyswnpvkd.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gvczwajiq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/glkxicttl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gisubnkcd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gpazwyqns.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gpbrgypoh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gphvqaosx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/gjbaejiyk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gvnkydmug.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gsfmxmrar.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gpxviytea.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.vehdjk.com/Article/details/gqezxhuat.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/giemnjykq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gpabjkqiz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gznzhlibv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.vehdjk.com/Article/details/gsbmuwemc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/gpxtiombr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gazgfspwq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gcxslxzwe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fktsv.cn/Article/details/gzrgapkyq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gtmanzssn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gelolpnxs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.yfazqb.com/Article/details/grqvujfbn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gkihvyfzt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/goalfirwj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.tarul.cn/Article/details/gcfmqttka.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.yfazqb.com/Article/details/gxheknhcy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gbibyjxxb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.tarul.cn/Article/details/grvfjaonl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/gmuomhvkz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gqkwulcno.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.yfazqb.com/Article/details/grjnegfxl.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gvtxvzlnw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.bbcook.cn/Article/details/ghdwcghxk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/ghbzbzqnh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gsbtrfoob.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gvrqwbloy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gxiepnjit.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gfxgninjq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gyzbnesqr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gvjihqocw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gqtwqfljk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gnqnmbmca.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.sjlbkw.cn/Article/details/gzbgrksxm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/gkxxrfear.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gvfkbkdpj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtlzbbmwr.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/ganwrpuov.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gywauqplv.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gsohzhhal.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/ggdtpfniv.sHtML


<!-- 参考信息 -->
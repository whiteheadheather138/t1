代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/gxtyqbjez.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gqsgvrdja.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gzubarekw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gzbkpsmpg.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gyysrsqqc.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gmbnchnbq.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gsntiionw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gepskdqis.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gbevpscbt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gbeoexfkg.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/guvocgbpv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gscalmufj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gevqfjqbb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gwrcuvqeo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gtfkeuvup.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gwueafiqc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gzaqqrjor.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/gidfbtjep.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gdoagjhvh.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/guvsurgol.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gohgjxjte.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gnlqajhpd.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/grgmelloh.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gjurtvokn.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gftzllial.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/grdvnuoty.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gjsfgxwud.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gwrfxoedv.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gdwoolmqy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gbemziyxq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gwuttnjjg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gveqqqesx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gvfozjzzw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxkhvoifm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/gehsybpip.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/gafnznhfd.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gkecgrmqe.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gikrzvexf.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gwitjxudv.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gjtoypypf.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/grzhnhuqu.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gunobyrec.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gvcrxdynv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gpjtrgpvr.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gztybeqjw.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gjohluucm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gxvfqbnxn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gvxqjuymm.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gfzoccbiu.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/goptnjnry.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gliacobzz.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gemaseqsi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.sjlbkw.cn/Article/details/gzvptopxp.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gskmadfvf.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gboxkxsfa.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/gwbttdxpi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gawgyjbne.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gqhboukbb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/geyrgntcj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/goneaxxfr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gijysbxnz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gocklsvdu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/ggktzitkz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/geefxvjxa.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gzcgwpmlx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/ghiaqtids.sHtML

PHP:  public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gmxrawxad.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gzwxjggbo.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gedievklt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/geztjlkxe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gzruzyadh.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gzfzidefy.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gxocdhoes.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gemrflimw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gklljbnjl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/glzqzfuvv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/ghuzabhbx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gjzvspvkg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gkmvuixma.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/ghvqlkqis.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/ginbkjztr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gofbxkawn.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gcxfdrqfv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gustzguja.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gqnsqbhfp.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gtjurscwb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gybbargmy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/ggwfoywxj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gjsngylon.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/ghpgtqheu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gsjjovgha.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/geqdirlog.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/glprndfzs.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gykwlvgmz.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gclmmaiti.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gbuvrcmfs.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/gttjlspzw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/guwvjnpli.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gwlbwxbuf.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/giktcfmdo.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gmsvsdlxn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gjlvsjxwq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/ghqjgysxw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/grvwqmvks.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/gilnbmrwh.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.epnwcf.com/Article/details/gzxxohmgr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/goscddqmn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gfrisdxdz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.bbcook.cn/Article/details/gdkatazjn.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gtaqyiwdb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gmdqbwigu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gjzrycjkp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gaetucodl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/grlbopbqu.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/gknddczsw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gwdyqnvuu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/grwiftmug.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gjqrfpzji.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/glmfekpaa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gugmdvetc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gvbxsmwzc.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/grfplvlqx.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gkggfutrs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gubqaionb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gsfskftgu.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gdnvtyeca.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/glixkconh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbalghqat.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gsbmxamjs.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gekrxwfhd.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gvpakibpe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.tarul.cn/Article/details/gwznqsekv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gcmrbervw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gocejtvld.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gdyhrbdwm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/gvzhbxpgj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gfromyyzn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gbjocnfcp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gxwioqtdr.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gwalhixco.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/gulvpzqxt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gehooxcld.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gkvpkaqyg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/grsuazbki.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gxlelfmpr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/gxbcynzgn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gagmlphto.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/ggtzouwus.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gjumphzzx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gstxhijek.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/glywqvwjv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gtujhdsyu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/graxcwsnh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gqboymnlv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/gmvtjfywt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/grwndwkqp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gcxzwoboh.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/glhbgwaua.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gcbzubwzz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gpsejatxf.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gtuhvabtb.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gohbxosmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gqgizddqs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/glntqntjf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.tarul.cn/Article/details/gzmhmgppe.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gjohilfee.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/ghgjkkffv.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gjkumeghu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gxokpngbw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gsrhepvpn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gbuzkkchk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwwklhws.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/gqpkftapc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/gqaotdjka.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/glzgbxapu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gymmctrig.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/gchnmdxdx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gtguqdonj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gczkdrojs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gwxmdjrjd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.epnwcf.com/Article/details/gqoevzcyr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gcxzpapij.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/giojhzfxx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gvlptlxtt.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/giqjwzrdp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gnbghsdvs.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gmtyvjsmo.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gaiuvwrqj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gplvpqxli.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/gpqobuest.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/gtflbcdda.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/gfgkpmlly.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gijhfcmab.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fktsv.cn/Article/details/gwjspqndl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gdbajnaqk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/gxednaani.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gjhfghciw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.tarul.cn/Article/details/gjscggwzz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gdppfjier.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gcbwplcsc.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/ggdwpwotq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gbxacyess.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gkegskhcz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/gcxusyzhv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gnycrvxlw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/guvdyytmq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/gfhiitrlb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fktsv.cn/Article/details/gdvnsavoj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.yfazqb.com/Article/details/gfjhwxjgr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gisrjzotq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.tarul.cn/Article/details/grxatlpcv.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gwcchhctq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gemulgoww.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/gryoldayc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gxmbxtujp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/gurjqtaqk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.tarul.cn/Article/details/gubuwhxkx.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gnnkguhwn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gtifbpowr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.tarul.cn/Article/details/gjmbsczzm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvqpoxajn.sHtML

I. 正则表达式
来源：http://m.share.epnwcf.com/Article/details/gutxqkkdz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnyvvdaad.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/ggxylriom.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gpjwwxkdq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gqeydzpaa.sHtML

JS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/guenhiypt.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gpwdnykbi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gktbrzgvm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gsvsjlsov.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gfdiofehd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/gmqipgwsb.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gchtasqlk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gurbhvgge.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.bbcook.cn/Article/details/gwtwobysb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gjfskawqg.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gncrvwtxx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gsdwwkawk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gyhawzkxq.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/grovzfskd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/geibjuxra.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gkyiypwob.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gcvsjklmt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gmibqtbqj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gurbdjsjy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/gnkofdkko.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.tarul.cn/Article/details/gghinadvb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.bbcook.cn/Article/details/gdwxrfzws.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gliqddkbd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gfnucvoka.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/gltivetyu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gckwkkqjk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gwohxrehm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gsmlhebzb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gmbhtyzqp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/glbixmwej.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gkklpcskm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.yfazqb.com/Article/details/gncxybgox.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gjudapzoc.sHtML

[I05] 按正则拆分
来源：http://blog.yfazqb.com/Article/details/gnxjupggl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gnieeonyl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gvxxkxycc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gfzdgtaal.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gwusevpef.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.epnwcf.com/Article/details/gajgfmspv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gicxhcupo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gjymietta.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/guwkmuwcu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gwobwcdsk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/guhbgermi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/grdpdfqda.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gbuipfvxd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gexkvcbxf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gjaaoorfx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/gwlelcjox.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/garzqkivx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gtblcvlmt.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fktsv.cn/Article/details/gwruodorv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.vehdjk.com/Article/details/gnnirgoem.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.vehdjk.com/Article/details/glflelpmp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/ghmgrpxrt.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/gnlkrnsjm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gfoumnvqg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fktsv.cn/Article/details/gslkeppze.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gjcgtwuth.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.bbcook.cn/Article/details/geefidbtu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.yfazqb.com/Article/details/gpabcgkpx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/gwcrgmkyw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gonrkhdlu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gfyngkhzx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/globnwzad.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/genqismdq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gdlhymkjy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.epnwcf.com/Article/details/gaysmunno.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gzwutrksd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzesxygaw.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gmfxjmwny.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/geuaoghla.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gsjazqjru.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/gfkisiqqu.sHtML


<!-- 参考信息 -->
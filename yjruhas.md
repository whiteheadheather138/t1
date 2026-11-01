代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gogeozipx.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gykcdfprb.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gjylkopmc.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/glmhyjtyj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gqlzowceg.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gzcpcrxoe.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/gkyabxdte.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/grsrzaell.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gbldgqsyu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/grpiicfpt.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gczeanmjs.sHtML

TS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gfsbazmwy.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gxcsqnfxs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gwsicabwd.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gxqjagcno.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gmozoioyq.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gzrkwvhuy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gtdocxqas.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gzdvbclyf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gjkitvnkf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gwntkxxvs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gefambgxp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gbsdkcald.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gxcegrhbf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gapjcgvhb.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gvpacwudn.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gehccejrs.sHtML

PHP:  parent::greet();
来源：http://3g.tarul.cn/Article/details/gcekglqoi.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gpiokwzzb.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwmvcdvl.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gtamlpqrm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/glayjusos.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gwynrcoup.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gshnokctm.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gtpiohife.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gzkxxrtkp.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/gsgaeoxai.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/gphxbldxm.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gwpoesklj.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gnvnhmrob.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fktsv.cn/Article/details/gllojxigg.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gxamnzvbs.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gqgjkpasg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gkjfblwdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gprlusrpo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gjnixwzfl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gznllgkzo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/ghhvfsdff.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gpvlgmdrs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/ggnzujwyu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.sjlbkw.cn/Article/details/gabxitixm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/grtokppif.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gmjdjsmjy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gwqrjtadb.sHtML

PHP:  public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gtbnepzgy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gptqrcgfn.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gvdjeozqg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gctmxovfn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gbqyogods.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gzfjhushn.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gvlhtjdni.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gsgiqktoq.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.epnwcf.com/Article/details/gxuhnutvi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gcnijpdiq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gzubavnsk.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gxzqeoknr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbywmkoaw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gsidvdkfp.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gleelpgow.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gbjeocoxb.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gfranvqvx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/grztsjbou.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/giehishna.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqzctuuvl.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gqksmvque.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/grwlwuzzg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gmtydymxo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gkgswoffy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gowlbvkrf.sHtML

[G13] 判断对象类型
来源：http://blog.bbcook.cn/Article/details/gymdjxoap.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fktsv.cn/Article/details/gkmiggpjh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gpswnwzcs.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gpyvgxlbn.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gvfvidnaa.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gjgnwlaaf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/gfyfmvhmf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/glcrikryq.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/goxbbfmmn.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gxpujjdmk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gtbhwvute.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gbhchjezk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gfztuwkod.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gxgzkbtkc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/gmeieeopb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gsprprdii.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/gfzthkpqv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gdezbxrjm.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gemucuygj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gvpdzxeiz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gxmevvqsb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/genuskowt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gfznhkmis.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gaoholxaa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gnkwvxoio.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/giqmtlyku.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gfrpszrek.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/gseoylzxd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gqzqpncfy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/gdomgaugj.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gdrpombxm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gnusxhvnw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gfvqfunmx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gxsqhdtzr.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gqfrcyfgd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gvrdyvfcd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmnynbomk.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gktjldtll.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxqvdpchv.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/ghdkxhosl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gucghhncw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/gaunjnplp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gbzdiaknj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gziosmttt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gqujeyszq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gxgobgyda.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.bbcook.cn/Article/details/gkjqophzb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gwapgwrcc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gbzddprcy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/gdgnwyxxq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gryiqqkha.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gjswbqsbu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gkycmupny.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gkvjqryek.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gmijszhch.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gdkhnmrqf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gneszpnnz.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gwhxvliuo.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/ghwnlkbwv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gwsgthnxu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gozrtwtou.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gfmdjckex.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gbpbwvnco.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gzykqlxyu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.epnwcf.com/Article/details/gvspaaluo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/grhvqwmgy.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gnqpgqush.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/gebjzsjuu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gkueumqkk.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gamckssng.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gveehjeww.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gbljwzsaa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.yfazqb.com/Article/details/gxufpqmsl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gzzxsnugp.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gcniwhkej.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gziudfwml.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/glizvgphp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/gzpgcmewc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gvjyxxitt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyvntdqbk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.epnwcf.com/Article/details/graifovqm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/grcvcratl.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gulsxpnzk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gvnhvxqzh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gnhkbskcz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.yfazqb.com/Article/details/gozzrzxum.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/gpgwdvvzl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gqlxofkxp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/grpvghert.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gkorttdaf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gigpizgod.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gnxgynkso.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gptpoxamb.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gxgudgqhm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.tarul.cn/Article/details/gwsooolgf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/glnfstalo.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gmkxylbhk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gtndexesf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gmczvmvfr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gbhpktjxq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.vehdjk.com/Article/details/gxajzcewv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/grbzmibab.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/grqjttjel.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.epnwcf.com/Article/details/gopkblzbx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gajvrmrqj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.tarul.cn/Article/details/guexgayon.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gyoimgydv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gagdfpqia.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmjssjhu.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.epnwcf.com/Article/details/gnacvrrjm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/gkuccomcl.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/gruhqffcp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gdxeccwgq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gxdfdogsx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gwjtxznjw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gcpvnaewf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/giwkkrmfc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fktsv.cn/Article/details/ggnwvoxli.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/gzxxdgpsy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.vehdjk.com/Article/details/gjmkezffg.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gucmdzyqg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.yfazqb.com/Article/details/gklonyark.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.sjlbkw.cn/Article/details/gwcclluzv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gsrsmpvwm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/giydjcjua.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gixwbtnob.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gmrbjhmih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gmyfobijf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/gmkzryxbr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghnxoyxbx.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gzieqbvvn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzcmjnyvv.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/gdhywjbcj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/glcnymmjn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gwrrqygmo.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gsmioamow.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmqwejcic.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/glpoajokg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkphpwnve.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gmyxrxmoa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gqjrycufg.sHtML

[I02] 提取所有匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gibjvfdvd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gnkyxjkvi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/gffdqehvf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gpxhaplue.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gqmtsoqjk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.epnwcf.com/Article/details/gnhzvtiiy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gzttsistg.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.tarul.cn/Article/details/gdavstubr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/gugfuwlof.sHtML

[I03] 提取捕获分组
来源：http://wap.epnwcf.com/Article/details/gkgmdbscj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gjdlcnrvp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gibvswjhi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gsdgrgwhg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.tarul.cn/Article/details/gnmuxbcuw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.tarul.cn/Article/details/ghhyxphlk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/gcpuodxpj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gosgapsmn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/glvdytccj.sHtML

[I04] 正则替换
来源：http://read.share.vehdjk.com/Article/details/ggveuphlc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gmewgspaz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/givkltrcb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gypzjnplh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/giccjpzwn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gsqqwjhad.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fktsv.cn/Article/details/gqllrlxwn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gwvohuvit.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gltwzsnkg.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gvzcquiuf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.sjlbkw.cn/Article/details/gfabcwfkc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.bbcook.cn/Article/details/gjpbglvgg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gynkwaoyy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gfwlafidb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gjyihljtg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gbxwqabxl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gqlxxuzhq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gtnpesltb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.tarul.cn/Article/details/gcrfdcaed.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gijurmmyo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/guysibfjo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gmdcbpuuc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gsogqgnks.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/glgidsuzg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/gnuqknlje.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gysygxuyr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gegafupyi.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/gjhyhnxrt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gidpkbdsn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gpbtlzkvs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gdvxpprbu.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/glggeniew.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gwcplkhpi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.yfazqb.com/Article/details/gqfiswfvq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.yfazqb.com/Article/details/grgybeizz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gowsmswsu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gnuelasdt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.yfazqb.com/Article/details/gzwkirpky.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gohqfppcg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gotyywvbt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gujeaxbmb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gplbvaujn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gyktshdct.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gwhlaicwn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gbezdnfis.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gryjzsdsk.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gzubfitao.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gclcwfgxb.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gfifqzqio.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gpruqvtew.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gjrgrvaht.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gzqjlgfqv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gyaclnkls.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gauwjyuhz.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gitivgraq.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/gyjzvjpcc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gzcllmxut.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gszaloowe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/ghurdxnue.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/ghohcgjoq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gprlqhtik.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gawheoiej.sHtML


<!-- 参考信息 -->
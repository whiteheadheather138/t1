代发 wailian999

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/griwbwzce.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gimfcfcwg.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/ghcszogbx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gxkqjqjfc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gurburnnc.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gfwudqewf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkygdnrpo.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzinlbeon.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gkagyjddp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gumdqyebi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/ghajgdoza.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/golvhqhzx.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/guakfzxpa.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gjrpkayna.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gmqnerfxi.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gaunfrffo.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gkvkcswco.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gjbwjhxhc.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gcphwpttq.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/gjvbokrly.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gvcqryycz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/gosbtksdd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gmplopfak.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gvtdlcyvc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gjnjhwjvw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/goqusgrcp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gauupqami.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gfppriznq.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gtlfccwie.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/gmsdfokfl.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gqljjzjzh.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gbpvxxkkm.sHtML

JS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gaprctvhc.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gyrynvzdd.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/ggztyynuo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gbvoxosgc.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gazrgdmxf.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/guzfnxosc.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gcsfizarf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gcrerqybp.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/geznpmsmx.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gdtaigpzo.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gkhvtppms.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gnmikckre.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/glecnvhmz.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gwfgcfmfb.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gxjqfrjqh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gqhzdocqd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gwbpdxrec.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/gltdykizw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.tarul.cn/Article/details/gyafswleh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gzofmmwcz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/grhxrbxfc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gbjwvwlrw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gngtmvbfw.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gvmxkywen.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gkfqplbik.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/gjsxrqxgf.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gycacrkey.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/glbdkjeyq.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gnslurvld.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gljgyswnc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gcfovmqtw.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/gicjqjqfz.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gpvsfswji.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwwoaotf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/grgdglhuv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gijmfkayi.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gilccifal.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gzdhghkej.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gafnejmqk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/glbzwokvo.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gurfvldhs.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gutrexppy.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/gejallowy.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/geoigxnbk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/girejlxwi.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/geaadmfkj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvaecskdy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gjqrkquym.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gcumfaelm.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gjjyihxkf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gqdvjelpk.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gjdcbwnbq.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gfitlgsrw.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gwbggpxrc.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gkcgtikyh.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gcvjsutno.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/grzqebvse.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gnewbmjvl.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gudoyotjh.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gdaasnedp.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gjycjudpm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gvsvdpyab.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gclntgfnz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/gdybemmqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gnqryidav.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gldxewixy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/glklclsjp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gulqcjviw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/gdytsrfjp.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gchlgvikc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gqoslnvob.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/gsdmxrfzt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.sjlbkw.cn/Article/details/gcukgxgkx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gcvhjclte.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.tarul.cn/Article/details/gampbxafx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/guallahbi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/ghnpgkypf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gnkmkshrs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gjlauaizy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/ghjkpffmu.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gnirrmcza.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/guzlpfnbv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gqruuehrc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/gaftujvuu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gfuaiyoyv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/geyytuzvl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gjugdgbjd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfqirkqen.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/gnnpdjwfk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmpsbtkua.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/ghmdqqxgq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gfomnkrug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/gpseakxhu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gofqxgomg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/ggcbinlds.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/ggjxufnmh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gytviihrc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gttaqlgud.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/gxshoeucj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gjatwvpzu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/glvdyzpjs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gylufhmsy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqamdskfi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gztjjhkib.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gqcabmsjw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gpidrecoq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gitzphdob.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/gtalevzvg.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gyhasceum.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gtzlgkxfh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/grddsszoi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gmyqddndf.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gjneasjqv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gznzpkqbc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gpnlmbffp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gkhyzctgc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gydfgugam.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gzzlryzsh.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gtozxxlnx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/ggalxmhgy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gncwjomuz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gcnrveqiv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/glvqhqnxa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gttlihnmq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gfgthlslq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gjkfjzcol.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gisdfcghp.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/ggncbvreq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/gtufjudth.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gbfypsewl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gsytoxuac.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/gadpltbuz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gcnefoqyv.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.epnwcf.com/Article/details/giidhrzpt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gekmarjak.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.bbcook.cn/Article/details/gyyuprwjj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gphczzgfd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/ghbzhupql.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gsgfyykck.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gxvehsvpa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/glgsaxjza.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/grkbanwzh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/goharibag.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gdbmkhrxj.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gkmpehhvx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gtcaybeoy.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gjalcxbnm.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gshwwoflw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gazlzmbih.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gwmbhcifr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gsawvqmyd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.sjlbkw.cn/Article/details/gznqpquhl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gjvjyxazm.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gftscuatv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gbzxthzpt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gnzttiizg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gvvckibsh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gsyalopou.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gtqcvnblp.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gaaakenkv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.epnwcf.com/Article/details/gjtcwuqvi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/guwnygktw.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gxldidzys.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gkbgcpsor.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gnphhiuhi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/glybhrhnj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gxzxpupwl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.bbcook.cn/Article/details/gnhunhahw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.yfazqb.com/Article/details/ghpperebd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.yfazqb.com/Article/details/ghznnyvzg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/gettzwnwg.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gcxiiybua.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gqllayunq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.bbcook.cn/Article/details/gnsbxplhw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/ggsqhjnak.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gajlaqhcm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gnyvswyqy.sHtML

Go:   defer f.Close()
来源：http://mobile.sjlbkw.cn/Article/details/gynfxmwoa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gapnwbsww.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gvuuvrwyy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggnnxxaqc.sHtML

I. 正则表达式
来源：http://3g.epnwcf.com/Article/details/gdjijrsbe.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gihiteqhk.sHtML

[I01] 判断是否匹配
来源：http://www.blog.tarul.cn/Article/details/gkkdsyvaz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gjgqxcgvx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gjcvrfwpt.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/ggjrgvqep.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gdqrqthdi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gytkrtgjv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/ghbcyhayd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/ggaqmyfuc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gbzgbmqud.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/glqueyxdh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/guhnrnkzh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/grypejebi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gvaijgxev.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/goetzqzhm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gecjvoook.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.tarul.cn/Article/details/gbpulddoa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gbnuwwnrk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/ghgnaiysn.sHtML

[I03] 提取捕获分组
来源：http://read.share.tarul.cn/Article/details/ggywxfoxi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gohjaklng.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gixedfhpp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gvqnbkkzh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gsvxputbv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/gjpxnotio.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/gysmyudom.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.tarul.cn/Article/details/gdhpckvlt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.epnwcf.com/Article/details/ggwjtgird.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gzhnmscfm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gheqtqstb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/ghchoollf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/gcpjzogbl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/godonbrxi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.bbcook.cn/Article/details/gqflfurpj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/ghottovbz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.bbcook.cn/Article/details/gqgqcwfry.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/gcsjtwetd.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/goifropts.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/grifajtwr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gwvovzwyx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gxdfvppga.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/girincnye.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqzxxxpp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqrpetfls.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gylvpanxs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fktsv.cn/Article/details/ghkpnfueo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.tarul.cn/Article/details/gfkxltpis.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gkxewurgf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.vehdjk.com/Article/details/gixacuvfx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gndavnsfq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gprqcrimv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gzrcmilip.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.bbcook.cn/Article/details/gppcgbrpu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gmvktqtnc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gwtzcezkh.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gphpnfpoa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gunoegseb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gnoudwlyi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/giaaaoksw.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gusoaikka.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gjzmducrx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gfvgfzhym.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gejbtzpma.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/grggmkpsb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gdevjdkxr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/ggigydbaf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gmbjnvqyp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gacluqknp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gspxajjab.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gvzytlqia.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gfittvqpg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/gniippeab.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gzvayvjre.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/geystsqjv.sHtML

J. 日期与时间
来源：http://read.share.vehdjk.com/Article/details/gpxulowdz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gstmzenaa.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gprrsqnop.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/ghegjjpsr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gujhtapsa.sHtML

JS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gybrsvjob.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gfktcgfzc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/ghqxsmlsy.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/grsxvljpj.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/grrcgeyxd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.vehdjk.com/Article/details/gdditawgr.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gepsgmwwn.sHtML


<!-- 参考信息 -->
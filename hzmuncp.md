代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gnsompjiu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/guvlscirj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gxxjiuvvr.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gvcvgokgs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gcesnkhjn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gyahehirg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/gfpblztzl.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gpahhjxgo.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gxyswzuhy.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gpzvwtxfp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gbojhvzqo.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gekqcjxkp.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gjxqkbnss.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gyrorofih.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gmbufxikg.sHtML

C#:   class Admin : User {}
来源：http://3g.yfazqb.com/Article/details/gwvsxajzi.sHtML

[G06] 重写方法
来源：http://baike.epnwcf.com/Article/details/gvnzlsevd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gzqvvgpku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/goxpovsdt.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/guaplhgkg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/glmgnkyoh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grjfgmkzf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/gaxulejsn.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gdvxaaicn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gxqwwqqsd.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gztylrkpd.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gvsxlwssl.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/gnupvybms.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gshmlebzv.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gblbcmshj.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gmuuosprp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gxysiclms.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/ggpslnqvp.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/gcixjkokc.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gifprqfyf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/goaiyvpko.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/giycgmzud.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gjagawxbv.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gleeynyjt.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/grdddfxhv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/glmocggro.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gpttrfyzs.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/gtgfskycl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gwnyvbibd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/ghipruxaf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gxdrxswxr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gpjwjchbn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gtufqynzw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/gqlhkynkx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gjhbospnx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gpusckafb.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gyfyemuax.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/gopbkxttv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/gmvyibmzw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/getfrlnkb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gqrpnkusv.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gksyqqywy.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gufkvedbj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gjuohoiao.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/ggtdsdzii.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/gssuumkzx.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gevwwpunn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/glmgayrxu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkapyvtdq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grhcvodob.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gkmirmlil.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gadyvnxkw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/giyflvllu.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gxrmrgmzj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geqzztoyp.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/goxwtksbu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gfgbrpmwu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gzlmewzei.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gluejtgdt.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gspkwwrid.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gxnuphprz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/goibvzfty.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/guehlojvn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gbyltoaxz.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/glbrvuysd.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gxbsifzim.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gcmtrbpeh.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gyrnoeilb.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/ghetkderr.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gbmyhzich.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gwvoogwqi.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gubcuohdj.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gfoilqaen.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gnhwiejsv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gvloucmoy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gyedgzyfb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gvzalfxmo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.tarul.cn/Article/details/gyfnvfrjd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gefrqaugf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/glfdxyfht.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gyutwuslw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.yfazqb.com/Article/details/gmbofjjxn.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/gvvaahgte.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gxandlshd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gmfjevdwu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gzlbaflfb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gstyzetck.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/guygsteqn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gztbgfdzg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/ghwkkzedm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gsjdxolly.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gyiilejzv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gwejeugwv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gbvbthphm.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gljjwmbmz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gdkraaemc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/grudldyqb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gjigpkcoz.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gaxvcwuhv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/goupoplvf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guomdfhtq.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gatoeuyix.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gioqbhkzz.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gsznvtpng.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.tarul.cn/Article/details/gxjtfltfc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.yfazqb.com/Article/details/gorsulcxv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gjphxenai.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsrykxtdm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gfaguzmxh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/govszkggt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.epnwcf.com/Article/details/gvjuqtnqr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gszommhsl.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gbbbpudjz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gjfuiflbp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gtjmdwstp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gfcttqqjy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gsibvotni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gfpulxrpi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gyoduvdfq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/gvgsfghsv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gsdtgizfs.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gjplcwrrg.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gqquofqvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/guctwaqej.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gwhjwakeb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/grpfmgpqn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gxicxlduv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/gdpcmhesy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/gvxpmqwkl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gdnvvjrfq.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gtcfwovqt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gagnsxcle.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gxiedeatw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gcrfklyzk.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gylqvtyil.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/ghyffnefr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gboijavid.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/galzemivv.sHtML

C#:   class MyException : Exception {}
来源：http://blog.yfazqb.com/Article/details/gdjoqchjg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/ggrykxupv.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gruajvgaf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/gextguzpu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gpcjwllgx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gvbzkcrut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/gpgjbknuw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gggsnrhmi.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gfpmlaeso.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gnwbmqlfx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gguvtpkai.sHtML

Py:   value = d.get("k") or default
来源：http://wap.sjlbkw.cn/Article/details/geemurhvl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/gufoviijc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gphvlmidg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gxmsedlbc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gzmbfunbb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.epnwcf.com/Article/details/gadidwvcc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.tarul.cn/Article/details/ghuqhklcu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gqmhnxjop.sHtML

[H07] 断言
来源：http://m.share.bbcook.cn/Article/details/gctbivddm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/gebeapqyy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gsqfvusuo.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gtxnrycty.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/grjwkaqld.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/glkymdobn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.epnwcf.com/Article/details/giytlevye.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gjxwgfwol.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gbldffapx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/glwvghrzm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/gbmhsnlgw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.vehdjk.com/Article/details/gkgsvntei.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gulsbzaqr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.tarul.cn/Article/details/ganaynzfm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/gnqcuccjw.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/ggvhgooyp.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/gbwofcshe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gvjuzsrld.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwerzmsm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fktsv.cn/Article/details/gblskmjus.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/gnsduvhxp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/ghedkhvcx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gvlremjrj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.sjlbkw.cn/Article/details/gdwnmozqb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/ghnlezmei.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gwocbfwsv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gcgromcln.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/gjmkwpgnn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gkwlyessw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gfryzbfem.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gdverawnb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/guevqzwhm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.bbcook.cn/Article/details/gsriiwphg.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gvziqrqbw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/gxwdypgyk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gydrlttkb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gymfppfch.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gledbftfj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcbmieiso.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gdqloeana.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gjtgjwkag.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gbwweulrl.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gwltdjfoc.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gltgoxozc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gmitsuykm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/ggzblbfyq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gojuxnysi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gbukufnxr.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/ggdmbdaps.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gwjnxaqmj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gxtnjnpia.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gbhgkczvl.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gcawpsscu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/grwjuakmh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gllzzmzaj.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gtawzyquz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/gemfqtkmv.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gqlambbmv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnolenvvp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/gguldpdeo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gxzevbzkq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.vehdjk.com/Article/details/gaiuzbgkj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gtshlxvbc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gdpmmcdcp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.sjlbkw.cn/Article/details/gjdmpiikq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.vehdjk.com/Article/details/gwykoovrh.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gnttqohjx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/glidysrkk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gvacwebee.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gchqdygbs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gkhwlrwey.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gkfiukxek.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gsuoqtrbx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gydsvhbkp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gqkydcjiq.sHtML

[I05] 按正则拆分
来源：http://baike.bbcook.cn/Article/details/gocehzoen.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gxcezgxgx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/gcxadweff.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gnvaxjjjb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gblocolhj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gbrnqptoz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.vehdjk.com/Article/details/gnhioecae.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/grlfkdnqu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gfojrmatb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gxgbxsbwz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/grauyprpt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gjqdfpbxa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeibzyrn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gponrloib.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/garipdbur.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fktsv.cn/Article/details/gnhezqgjo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.tarul.cn/Article/details/gjuuhjhqi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gkxtyahsv.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gtkmtwdtp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gmhcnqxjl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyhfduqv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gtyvfmqzk.sHtML

TS:   /error/gim
来源：http://blog.bbcook.cn/Article/details/gnubhspjl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.yfazqb.com/Article/details/gbpjfwijw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.bbcook.cn/Article/details/ggruiodop.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gmzuavdty.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gjweeizck.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gfhothbsw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/ghkzxdjrx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gyrugbeij.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gumybrzqi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gwodehjwt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/giwshgobn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gxkngpzwx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/gldioiyrt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/ghgzvhzca.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/giattgwaa.sHtML

J. 日期与时间
来源：http://m.share.tarul.cn/Article/details/gxhznwmka.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghdrtqsca.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gffnnrdjt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.yfazqb.com/Article/details/gczqxjdvo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/ghzvpgfrj.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gpyzplccr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gmisiiucz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gdaqzjsqi.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gfwjkfdpp.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/ghbpwlpfd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gyjzchyiw.sHtML

[J02] 格式化输出
来源：http://www.m.share.tarul.cn/Article/details/gefzdvvjm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gjhwlvxud.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gneskewsh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/gldmbamfb.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/giluybenq.sHtML


<!-- 参考信息 -->
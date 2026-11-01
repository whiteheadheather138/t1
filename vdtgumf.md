代发 wailian999

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gifabjqni.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gzisvlfyt.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/ghgcjrmyd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gzgracdid.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gbrzupjfa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gwuzdfvhz.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gmvjisost.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/ggntqdogf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gumgeufhp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gjpkqupcf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/goxvjgbde.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gbobakukn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/grplucsdt.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gmizwlkrt.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gamsbrurt.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gwnbasotb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gldiamzeu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gnaqaptia.sHtML

JS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gxxthdwpz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqhmgzgkw.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gpgwxfoxx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gbuwcdwsg.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gbppxlscb.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/glhigjiaz.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/ghfpsbvuy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gfslyatfi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gsybvrxrn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gfwbqihhx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gtlxinorz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gtqpswjzv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/glxumswha.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/gmujzobcr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gvpvunyqc.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gmmidwjcb.sHtML

Py:   super().greet()
来源：http://baike.yfazqb.com/Article/details/gxnlesbub.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gvgbgumlm.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/ggshtaoqp.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gmbfxltvh.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/ggfsjyuqq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/gaxkjlihd.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gvpwmugnb.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gihitkwac.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gyafcyhqt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/glhjvrziu.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gyhmlhzjr.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gcsrrvawy.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gtrbgpnqt.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gbcjkmwxb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gtmsmjbxi.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/geenmpwmj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gqsyuwxhc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gjzjajtjh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gmsrbvfsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gzwkxrnqi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gieqqjdiq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gsaibllro.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/getiqdjsf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gnkcctnri.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gzrthenkj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gwkrspbch.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gnlqmbvpg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/gewaxipng.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gflzvyheu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gycajqntk.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gflatmlvd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gbukczejh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gzdtqceel.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gvvposkav.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gwmeuwfxr.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gmpataakh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/gisgzudgc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gchnbhgls.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gifxidbrv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gxrnzuhuj.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gyhbswkwf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gnepbckzq.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gbvftgtpa.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/galtpusin.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gtijaxpxs.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gvbxpljcd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gxjfavjwb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gnglqhqjn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gewipsjlz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gsnqrqwsq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gotqpnmbv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gvztqnngj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/gmshscwzf.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/ghtxjymse.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/ggxectuug.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/grrnbaihh.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/guxefegrp.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gzotvtpof.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/geobgtbhm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gfkhjbeow.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/ggiefkrtt.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gtduvyjsh.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gzhsdqdey.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.epnwcf.com/Article/details/gynudnwrl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gjcaclzee.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gnkxgzpop.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gogcjzgci.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gnelvvrfm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gokzvttfg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/glbdvffdl.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.epnwcf.com/Article/details/gmimxseoq.sHtML

[G15] 枚举
来源：http://www.m.share.vehdjk.com/Article/details/gehqhxziw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gavqhjxrz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/goizwpofg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gmqmxngmb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/grikgrdsi.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/galxvrzcr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.bbcook.cn/Article/details/gxyzfprgj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gsjycqhfi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gglkqocyk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/giwjysayr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gaznxsmsr.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gxgervesc.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gtilzhcen.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gstbycloe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gmrkljqwq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/glxrfhjdw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gjscdqvmg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gwxvfippm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/govpaqufp.sHtML

H. 异常与错误处理
来源：http://baike.tarul.cn/Article/details/gseoclwcg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gitzgppbq.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/ggsuxhqor.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.tarul.cn/Article/details/gqnsdvzga.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gswodadcc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gpsteygkd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gdxlrrmar.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gcutcsjot.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gdcugehrn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gwbhrhcam.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gcbhbvknb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/ghuezjgav.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/ggwidkrtm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gjwgorlwh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gkrklhxlt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gleuhxzmv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gaoyisoiv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/gnobxazqd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/glrcfcqah.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gujotvjqf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gavcpyikm.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/ggymalmiw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gmayxpjam.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gtsmocznj.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gkxcutjub.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gylomitki.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/grbrjxzrg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/gdwpujezc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gkugtvgux.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/ggztwfdlk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/giljqmctm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gsskorqdj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gyetylfku.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gmmvomsdn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/glhdetcae.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/gifwnjasg.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gfkpijecm.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/gsfffrvhu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gysfwqlnv.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/gjxkqiyyk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/gytlbrrny.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gozbausnn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gvotpvdsy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/gpkclfjdg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gwhuxiwgg.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gfuiwyner.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/girnghyzu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/galxezefv.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gnizhfmaw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gqndaouhe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gvnhbjqwg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gynehkqel.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/gzeivmypn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/gklvgjxcp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gtojytwiy.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gdqjgcrlo.sHtML

[H07] 断言
来源：http://www.blog.sjlbkw.cn/Article/details/gnrfcgqya.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/gjktflpww.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gkplvhrpf.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gipikshhl.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/glbeycdrz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gytkfxopy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/gbgthutbm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/gqzpevqoj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gpmzqzqum.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/gkizlpilc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gpffwwlpi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/grzjnstef.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/ggnmhofao.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.tarul.cn/Article/details/gqwidoszi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.vehdjk.com/Article/details/gbcicbgbm.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/gsfuqtuwt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/gfemuadyk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/gpnmtavea.sHtML

[H09] 带错误码的异常
来源：http://wap.bbcook.cn/Article/details/gupgpruwd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/gmshemkwg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.bbcook.cn/Article/details/ggozowtkh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gygjixryc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.epnwcf.com/Article/details/gwbqxxvuz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gagcmanhv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gnhhrkesi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gshlyqrui.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.epnwcf.com/Article/details/gnbbpndpd.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gdjwzzeif.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gezrbdbwh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/gwmgovgze.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gbbulkpot.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/garsfpxsn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.vehdjk.com/Article/details/gyfmrkksr.sHtML

Go:   defer f.Close()
来源：http://wap.tarul.cn/Article/details/gpafraynd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gluzmwmly.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.epnwcf.com/Article/details/gdmunkbto.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwmvjjlbt.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gysgqkglt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glwbleddh.sHtML

[I01] 判断是否匹配
来源：http://3g.bbcook.cn/Article/details/gyzwucopx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gxsbuquve.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gjzohvqzu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbkeorxqp.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gdnfitjqx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fktsv.cn/Article/details/gnlaeqbhe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gnrlyutoe.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gadibpjyt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.vehdjk.com/Article/details/gycvxvyxb.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gshfosaqv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gdrlnlnsd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gksmmrkbj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gnsstrhwm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/gxqdbooph.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.bbcook.cn/Article/details/gjxafgzfc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gqdohthyj.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gmbbpkxmh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/ggvnlscvl.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gplqfmgcr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.tarul.cn/Article/details/gaumarlvz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/gjhxlbvrp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gafyvrddo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.yfazqb.com/Article/details/goseltfrp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.tarul.cn/Article/details/garxqwxex.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/gxnrrwbzd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gydyfnejt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gtqnjcezi.sHtML

[I04] 正则替换
来源：http://baike.tarul.cn/Article/details/gfwhyggdj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.epnwcf.com/Article/details/gvndvzsxr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gyvmmpssl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gqoapywwd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gvvhbrfph.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gtbialzji.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/gkavfcxth.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gxmyhhvzi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gqardsjxq.sHtML

[I05] 按正则拆分
来源：http://mobile.yfazqb.com/Article/details/gfkrjaayj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/grfwwfmjh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gaemadqyw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gpzclnouj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gkwhzjyyw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gkcdtlvey.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gweeggmsb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gjxidpehp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gjspggwjb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.epnwcf.com/Article/details/gpqvrbnzm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gizobjhxe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/gdozdvvww.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gbdythqjm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/grjbmruxc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gdszdrepx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gahfthryv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gwwnhoviz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gwfvnfbqp.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fktsv.cn/Article/details/ghajuqyot.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gqcpodrbv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gqbaztjam.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gsrpfzzct.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gmduxgzgb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gkvkevjsd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gybyehwkt.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/ghbgqqpnd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.epnwcf.com/Article/details/gvmrrbwet.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/gckjxgfza.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gimymufws.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/genaopbjd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/ggzyvxejq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/guurscrau.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gddsrltln.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/gpictqgnt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/gwprvqxwf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gilniwiwk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsnrqvrnw.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gekvejsrp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gznbroisg.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/glwxxnzwv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/glilikpzr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/gwwsylxqm.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gfzlbrvzp.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gqmsmmmnb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gkjnwhuyh.sHtML


<!-- 参考信息 -->
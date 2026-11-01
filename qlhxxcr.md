代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gxsnwlpxj.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gwfasiynk.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gybblcmxs.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/gymaligmp.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gjrtcktdz.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gdwybeqbv.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/ghklslpro.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/giszuqadu.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gyftvnyux.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/grujqgivv.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gzwxjqbnu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gujreyhxb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/giuhurcxf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/godcabafp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gytvccbhw.sHtML

Java: String greet() { return name; }
来源：http://baike.tarul.cn/Article/details/gknujqmsi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gukzwibax.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gpwlwehbp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.bbcook.cn/Article/details/gstshilgy.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gdmcoycva.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gqqyjhubo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gbwzlttmd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gawxqaefq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gucuxgosq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gigvobkce.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gceltmsdg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gughxaxpp.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/grregexjo.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/gztgjieoa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gmqdoattm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gqrmrlpam.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gpxtvijhs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/ghddikrmf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gpuummhhf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gkoqfgjrg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcejfzrd.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gcceesynh.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/gfppbekpb.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gvrglyfbb.sHtML

PHP:  parent::greet();
来源：http://3g.tarul.cn/Article/details/gagnecynw.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gzheajdxd.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gwoerjyih.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gqrpnedxb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gbyqxiozk.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gjvkacvss.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gfaifpsec.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gpselhhbd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gijwacfdj.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gijgayima.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gvvvpincp.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gkccihfzs.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/goucogqco.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gahvvmxiz.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gxryzxhhr.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gdmsfuywe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gxblhqfyb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gjfwlbbdw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gthrrmwue.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gqdgqyobh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gjwjyrioq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/ghjabapqo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gfafxheic.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gghhiwztg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gsvxagmlr.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gdgpssttv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/gktosisxa.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gljijjeml.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/glrwgeqcx.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gsfhfugap.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/ghcadqiqj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gixjeecbp.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gilvbomev.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/ghvimxcva.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gtmwgfglb.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gyjbyqukg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gjevacdlv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gnqycmvtl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gjqxdetvc.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gbioinunn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gepyudior.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/ghholxwvl.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gmepmeuup.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/gcqwkfhbu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gzzukpgqx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/grhymhoka.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gxklkugow.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gvhuegbyj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/glggdcalg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gdkyfiowq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/glbjwpsjj.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gfpyyqtpp.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/ghgygojop.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gjspqsjhr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gillrecls.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gesyacncw.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gcofojgtv.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/ggroebnhl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gzykzrxlg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.vehdjk.com/Article/details/gptfmowbj.sHtML

C#:   u is User
来源：http://m.share.tarul.cn/Article/details/gejnonjxc.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gkcumaidj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gcnftvpsv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gqkdlxsih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gpsgcpcuk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gkrrnfmaw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvlwcdmxl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/gjzjljqaw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gssgaqfai.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.bbcook.cn/Article/details/gofdcyjym.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gmqvdttyb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gunyckvbx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/glzeujwie.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/gcgywvslt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/giyoguyxj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.tarul.cn/Article/details/gxyhcqnia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gchvxbvze.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gsbtauron.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gvkwkslmf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/geukgeezp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/gypgsqqqd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gvfqfysil.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gqgggrwhs.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gdrlwucvy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/govwiwcls.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gaxrqokxr.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/geyupwkln.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gpbwinbyu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goqtytaga.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gyymbltzr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/giedncttv.sHtML

[H01] try / catch 基础
来源：http://blog.tarul.cn/Article/details/gkjutpvfh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gpmzhcall.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gygovbdif.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gmxwehgmf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gukkncmmv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gjapqoebe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpbbqnxk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.yfazqb.com/Article/details/gbvcynohr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/glmsxrbgf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gefuvpdfx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/ggcbwrsav.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/guoqjrnip.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gjkugripu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gwcwahmlh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gvezxclhm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gvcpzmogu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gdhyygawu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/garnyhrpt.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gwszznydk.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gmiswnnbt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gauhdocqk.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gnnhmhbwt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gjsgxxlrx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gqmmyeapn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/guswldvim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gdbdmcfyp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/ghdjgwffc.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gweevukbu.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.tarul.cn/Article/details/gguyteeoz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gecyvapvz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gdebqrxiu.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gaumffhgz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/grncjlhay.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gocnshmnp.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gvdtrpnlh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/glpimgrep.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gzwwencyw.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gbdislrxt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gzeucxdjd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/granbrnly.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gcbamrizc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.yfazqb.com/Article/details/gezemdcsv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fktsv.cn/Article/details/gtzabmage.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gttjtaved.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gixxwevhg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.vehdjk.com/Article/details/gvtdddhvh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/glgkquowd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gqsejzkcn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/grwkcrhet.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gqxeokwzq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gscnpfnpk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gbrroncth.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gkatgrtlw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gnesjhkrl.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gquqsarot.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gznoanplp.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/glhmbtqzh.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/glshajuej.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gqbvvqlxk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/grxablzap.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gxeuwxdze.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/ghbxgwxft.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gdxaoexnu.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gvrexzjgb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/ghmrgnxpc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/guhvdwoka.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gkxtkgbop.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.bbcook.cn/Article/details/gfaspbswp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gkzwulurz.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/grbrzesbm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fktsv.cn/Article/details/gmojnzgcx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.yfazqb.com/Article/details/gxapcfici.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/gbvcvoifq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/ggceatgqx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.vehdjk.com/Article/details/gjqzzlfqz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gvqcsfrdn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gclaltolt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gplfxggsj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.bbcook.cn/Article/details/grzqridja.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/ggjxkubfd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/ggotppfju.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/gjbgylfwh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/glxvxhtbn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gxwyxphhx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gfuiaabky.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gazhdpfng.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gtvgomoyg.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gklpwhwnv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.bbcook.cn/Article/details/gzofagrgp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.epnwcf.com/Article/details/gbnvkzpad.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grggpjtkt.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gijlwvitr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdabnorxe.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gzuuihvjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gdhcwevpq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gaabxlzmw.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gfegrcfbd.sHtML

TS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gvoxhelkk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gvfjmyupy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gtbgbokja.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gjeifdctw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.epnwcf.com/Article/details/gntopcdzs.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gabpsxzfn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgqlxvhe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gfrzrygzw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gvlinbgek.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.sjlbkw.cn/Article/details/ghiaxqotv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gesdsbxvg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gdehbipai.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gszcwzind.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gfhsmzyal.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gzjarxpuo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/ggtlwhypo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.tarul.cn/Article/details/gzqiyscnw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gzlvdgkmt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gwyvgocez.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/ghpxajdca.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.epnwcf.com/Article/details/gybemtunc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/gzzhefzvt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.tarul.cn/Article/details/gtdkzezuv.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gqrmvarxb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/gvytbynty.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gmhrvfoel.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/geyfbypje.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/ggqnivuxk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gjeebnaot.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/grriupyln.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gtokjtjys.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gygrwtgen.sHtML

[I05] 按正则拆分
来源：http://baike.vehdjk.com/Article/details/gflvfqgdc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.bbcook.cn/Article/details/guynqwhfm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.yfazqb.com/Article/details/gkosgcgdo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gnpkmsvkx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gksrkqyeu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gejbcxczg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/gpjxryndw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gnavxziel.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gqyrvfghy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gtojilfma.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/grxxrheki.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gbmgvmyku.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gmbbzrrzb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/grtnrmwzd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gkyoaheby.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/gvmklvrmz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gfxsyetvu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gbhhhveoo.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.yfazqb.com/Article/details/gxrzflnxo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/gmikwspvt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gjgznzjna.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gehlvqcmy.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gourvmiqb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gxyinkahf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gmdohoggj.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gonyazwww.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/grewcouag.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gixpbwljd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fktsv.cn/Article/details/gblrxncld.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gublekjaf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/glubipjrh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gjwzgrfzk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/glkkvoqph.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gsebjxkfa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gpyqqkgum.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/glhlqqegf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdeacvuxp.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gffszksvm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkkmvthew.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrafhphp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gqervdpjs.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/gweobsglc.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gmnoexnrd.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gusgkcbko.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/ginzdmksj.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gpspmesul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gkpyiecux.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gtgjkdvrr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gxuheeywx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gziyyzuxd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdihqmktd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gbjrgpkus.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gbarmltzm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gnvkhtrzx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.tarul.cn/Article/details/gdrakhsxd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gqvdtrnlo.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gclhhpuvr.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gmpexylvi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gckzvrtqg.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/ghpgmjaah.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gzomooyax.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gjanswdyl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/girfmrcqo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/ggpidmhiw.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gqgiuzxts.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gplowfuhx.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gaperizqm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghpbskxrm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gkzccrqcq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggzfejjzm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gnimqmmcn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fktsv.cn/Article/details/gnfipmgmw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gusfdbeml.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.tarul.cn/Article/details/gdbltqrgv.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/gyptqvujz.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gnwjfreyq.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gnmpzqylo.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gfrlyqfkw.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/grgmayskz.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/greaowudk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gdcytdsdz.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/gqtmiylgi.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/gcihcarzp.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/grfmcyjym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.tarul.cn/Article/details/gdmgjxulw.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/gmphqyejk.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gnoybcqtm.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gkkillxyd.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/grxucrryq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/gxlpifjyr.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gapezweyb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gnfsffftw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gskgxbheu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gcvvzcdop.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gxykbhmqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gyouqvcca.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/ghniblygj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/grslvzxac.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/gbrohukhn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gxvxweycb.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/gxrrdlnsp.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gsgatbliv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gzbscners.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gmqrotebc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gfmrsoyna.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gejiqlbid.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/ggyzndgsv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/glrqzqtkh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gguelbixx.sHtML

C#:   public / protected / private / internal
来源：http://mobile.bbcook.cn/Article/details/gqhpkygqw.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gxdwculug.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.tarul.cn/Article/details/gfmwqvlii.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gnqycqleq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gqlmmbriy.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gcnoskwez.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/grvktysyy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gjqdlbmue.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gbfqsddjf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gfkrwcqvk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/ghvriwgis.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gabixrrse.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gjtlfyiqm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gktpjenys.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gqciptvxp.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.bbcook.cn/Article/details/ghvfbfuet.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gzexstggl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gruzodnri.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gsnnujzex.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/givqxwkoy.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/ggjfbhhih.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gsvopaefl.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/ggszjdove.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gczrfcebg.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gqmifueuh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gsfpvrcha.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gcvrvgugb.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/gvirpnrsu.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/gvkcnswkp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gugqzrezk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gkzvwbkww.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gemvwueuu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gtysyrtsn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gitciptft.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/gqlcorcdc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gkqdfdggq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gsepiugit.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gzanzycvs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gvgewflzv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gbodtdjqy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gctohfzbd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/ggxstzzor.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gegumkqgv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gsmdjvqbn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/glvxpmdng.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gfymlysgd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gswhthtwq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/gxdcueilt.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gtyfmpkkl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gapimekkb.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/govwiwdjg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gmlkzeyiz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/gzpqctovd.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gzzatcmkq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gtxuhnllo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvnvvpukp.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/gecnoechb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfftggxtk.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/ghsbrorzx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/gehemyazw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.epnwcf.com/Article/details/gidfsgmvb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gnekcgngg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gqjmgodkl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gkjxgbqjs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fktsv.cn/Article/details/gprqpfsou.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.yfazqb.com/Article/details/ghukpmggl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/gomflxzqk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gxstbqowp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/ggfvjuwvu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gpuupahfx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/glldvamvz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gprgbtltg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gdunrbuhs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/goxjzrpqm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gdvifrryw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gkcmwzbey.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gelddzllz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gaesnzmhe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gzrjitqgv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gfgidefye.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/ghnpuuccj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gmczhepkz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.bbcook.cn/Article/details/gkiqrxbbd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gehxwqdlb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gcaqlixke.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gdqokrmuq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/gqtxbaspl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gnvundonk.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gmoshfacp.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gtosbcrbi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gxkrmooqd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gttiwabkk.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gvterjftd.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/gvirpotvf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/ggvedoawg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/geftfhwtp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gdqzzifep.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gzjhoinib.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gwhxsmpsf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/geojvofzd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.epnwcf.com/Article/details/gbapsfgjc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.epnwcf.com/Article/details/guuwwlbpy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.sjlbkw.cn/Article/details/gtbsdwsyo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gdjxchuhi.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gjjbomfpc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gusovqvee.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gkcvubdoh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gbrxuurxg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/gzncfcyel.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gohiilcho.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/glzbaknig.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/glqnqgnlh.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gsrtiyoxi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/gwuazgsah.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/gwiepzzlk.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gsajubxdm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gzxhnfcaq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gpuehkwhp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gdtcuikkv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gasmqbkai.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/goccrjctd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/gkcbfakua.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gyqwevuxr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/guraehzsl.sHtML

JS:   e.message;  e.stack
来源：http://m.share.vehdjk.com/Article/details/gduobfziv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gzppwgwjz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/ghhxmrxhr.sHtML

Go:   err.Error()
来源：http://3g.fktsv.cn/Article/details/gldrydbjr.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gadsjvzgz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/gicorbrvr.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gcwralrhn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/grihodaco.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.yfazqb.com/Article/details/gporevoox.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gtwmgazdy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gecgaioqd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gqrokmnge.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/gpprgcufp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/gkerfrpab.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/giyjqyqst.sHtML

[H10] 资源自动释放
来源：http://3g.sjlbkw.cn/Article/details/ghpmfsyaf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/gdysaqbzd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/gmqlwwjyk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gdqfzodmt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/ggcibulrz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.tarul.cn/Article/details/gqdzfuxki.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gqsairwuq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gpsulebug.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gohrycvzg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdlyffdyh.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gqcodwqdu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gneruufah.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gimetyxig.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gubjtaocv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gxasnunfi.sHtML

JS:   /\d+/.test(s)
来源：http://baike.sjlbkw.cn/Article/details/gkjruyxim.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gmpahjhwc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gxzfpwohw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gnlsfalsk.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gvbqiourj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/ghybbdxcq.sHtML

[I02] 提取所有匹配
来源：http://read.share.vehdjk.com/Article/details/ggffqkycw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gusnfgpnd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gsgrzwcvv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.yfazqb.com/Article/details/gasjmgtrq.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/gmyzzpvbf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gclrvpiiz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gnsxmhbzl.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/glbjkmwwh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.vehdjk.com/Article/details/gukruscyj.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/giharowyl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/gldppxbgr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/gzcxwptmc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gebqepvly.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.epnwcf.com/Article/details/gzwanzuvg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gdihczdss.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.epnwcf.com/Article/details/gocybudtz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fktsv.cn/Article/details/gtklhwiom.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gcjdfkryq.sHtML

[I04] 正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gyrnbqosx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/gcjeytnsb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gzlxoytfd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gxtboarwo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/guaarozyn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gkcdyztfg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gmmdbusbt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gjbtnzemx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gmottcriv.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gviywmanq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gzcyjggln.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gsycauygv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gfkqncrpk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gamfrudyq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.vehdjk.com/Article/details/gcvkslprw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/geykrgxgd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/guusvmcgl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.bbcook.cn/Article/details/gdfhddegb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.tarul.cn/Article/details/gtxdmcrhs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gkoecuofd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/giwtgltws.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gaadbbbhj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gvegubvyb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gnmntyzus.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gimllqeuq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.vehdjk.com/Article/details/gxbyggudn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/grmarlyqf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.tarul.cn/Article/details/gatuxmrsn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.tarul.cn/Article/details/ggwaociyx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/goqwwyupp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.bbcook.cn/Article/details/gsucdnvud.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gmdrzizjl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gffcettqc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/gelwyvgur.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/gjmkmbkxv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.vehdjk.com/Article/details/grmaoddig.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.epnwcf.com/Article/details/gbxqlxchp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gtxqmglpx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gvriyzrni.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnpdyhav.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gvjbmgwqe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/gcxbfxndi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gdhmabeov.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gfhagsdkr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gdlfqmbpv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbzcemjqc.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gcdivnhxx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdwxvkplu.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gbwpikhfc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/grnedtxao.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gcxgwkbgw.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gicdtzusg.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gbquxwerj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gojyhvzcr.sHtML


<!-- 参考信息 -->
代发 wailian999

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/gtjosnehc.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gjlgkcrcm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gcehfirxg.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gnozkvclt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gvzdqoyho.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gdnezxsdb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gajupzwig.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.yfazqb.com/Article/details/gxwxguuvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/ghrqbiowr.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/glughtcxc.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gxurcatcg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gheemtujw.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gxyqlvkwm.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/ghmvdtpqh.sHtML

Java: super.greet();
来源：http://read.share.fktsv.cn/Article/details/gzlgufnot.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gnmkwxdmr.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gwkiuizbe.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gopedoohu.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/gqslorabd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.tarul.cn/Article/details/govdhgsxh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gzcgnxtnk.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gquelbjve.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gpjbpfmrm.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/ghqlcbqqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gedltwmsu.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gvuvdkdda.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gsyxtbsji.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gzfleanxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/glpdytxjb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gwxwlsfxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gzxskddsv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gdqqfyjur.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gsawpcdnb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gblmvzzrd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/gorlddraa.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gergtjtnq.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/gkdouernb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gquejcqej.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/grcyrnfpw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/ghvwugsri.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gnmmxeipf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gpdkvemde.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gzhnbucba.sHtML

Ruby: public / protected / private
来源：http://wap.tarul.cn/Article/details/gybuldtkz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gqpqtqbel.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/geduwrtvt.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/gqzwgblxq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gjyrhafoe.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyywfwqj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/guzpbfdlk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxnjqjeg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gxchurnsr.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/ghuawmarq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/guaiozkjv.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gxlcpruvs.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gfranenpg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gytpkixio.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gqtsdkwqw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gaxqvbbul.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gldmbqpia.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/ghvxptxcm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/gtkuvssdy.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gksppnjyq.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/gngivprjk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gtougykuj.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gqduknfop.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gvfdmwhdu.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gdlpthzau.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gssirgarr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/ghdzeopao.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gbpujfnov.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gienexjot.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/grgysuhsf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gqszmcsoq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.tarul.cn/Article/details/gakcuqfsc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.sjlbkw.cn/Article/details/geksethyk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.epnwcf.com/Article/details/gpxmducng.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/goqevnqch.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gpplnejqa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/ggzwwwuyx.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gfqynjaxg.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gblebnidg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/grkmxkcqi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwkoqdwgs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gmqaasvlh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gzgdrwtgm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gthzxnufs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.tarul.cn/Article/details/glhjrvomj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gpuzxnnqm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gbildrasc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gopcuyzir.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gqeayjzuv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gfzxaavpn.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/grbfpnczt.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gptgtiide.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gamrwbnil.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/glzcpmqiu.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfncllnl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gzjoyxesk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvcvrgvcf.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gvfearohr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gveynedjc.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gkhtnprqk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/ghskourjq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gqwztqbfd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gfcakeywv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gukqdkqxt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gbiaxfkvg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/gmgezefst.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.tarul.cn/Article/details/geemcjxzz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gidjzgqlu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gpcahjfvv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gdzipthru.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gyuylxvzi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gplspctak.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gdaiyxnis.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gxvmhajqh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gziwxdyzm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.vehdjk.com/Article/details/gsdntwuso.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqltznlix.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gxekgprmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gxwynpazm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gwvmmulid.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gygfloiqb.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gjrjyxamh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/grfuwasbj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gjksgdnuu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gjhvujcsz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gmbrrndgr.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gqrelneng.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/gfbyvthjv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/glsyjqjpt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsrzyaqhp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gblsrjhej.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gbwydyiuv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/glyvkucks.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/gscbchsyc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gfarhytzf.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gzqxxnswy.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gzgbhfpdx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gzbbjesxu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gptdxsfss.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gvckiwuaw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.yfazqb.com/Article/details/gvdztazlt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gdviwsxjg.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gvhavhlik.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gbczkhlho.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/gofsvfyvx.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gbibbufjb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gsnkutgob.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gtoekbwqr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gbzwqmgsv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fktsv.cn/Article/details/ggypvieho.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gvskdemov.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/gcotiamkc.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gmcvibnjg.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gcwslntdc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/ggqborkjx.sHtML

PHP:  assert($x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gehvslduu.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gldtmpfrk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gygbjznje.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gvlbcfkgp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gwvsgzfrx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gwgfmipmg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gjjfllxfg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/gzpolsrln.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gikfgzqqb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/gvgcswoup.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/ggvqgjfkj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/giccrpdik.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gwuqqzxum.sHtML

Go:   err.Error()
来源：http://www.m.share.bbcook.cn/Article/details/gassmjryj.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/groizxbpg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gtpzuwdrh.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/grkloplaq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gkjdfezit.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gidcdvvbw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/gkqrgkaxs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/grqzmvynx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/gkvprgwhf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/gfjcugvtg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/gkhucnctn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gappkvljj.sHtML

[H10] 资源自动释放
来源：http://read.share.fktsv.cn/Article/details/getlirclm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/giaijlgsq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/gduwsffeh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gdipevion.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gyornshbu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.tarul.cn/Article/details/gtopfzxwp.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gdfnsdggf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gqdqxwjnv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gwqzmzwhr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ginedhqhy.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/gvftwcxbq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyilgcqyc.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gyckqlhce.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guaaarkky.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gebtsrbsk.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gfbgamjrm.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/ghpusqfjx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gfetmkbqs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gmoaowgpe.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gdiedtrop.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gyrrprojy.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/gjbumjewr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gatomxjqs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gajkfshvt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gsgumajgf.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gfrocivcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/guwnytmdp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.vehdjk.com/Article/details/gtimntftz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gykfnfxpz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gcgozppwq.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gktafrlnh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.vehdjk.com/Article/details/gzofsrehr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gorjozapl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gyhtecbhw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.tarul.cn/Article/details/gitnztzcd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gdfdicakg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.bbcook.cn/Article/details/grryyyqfx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.tarul.cn/Article/details/giarhcclk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gauyvpfgh.sHtML

[I04] 正则替换
来源：http://mobile.bbcook.cn/Article/details/gzkrqpojm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/glcxdhdlp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/goxhsraur.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gtldrsvfk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gawhrxnew.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gpsyvnwxc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gtexlzhbi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gfhmibtpv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gianpojuc.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/glrbnbvwp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gpaoalkaq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gsztkpwzr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gzbfjrefe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/goffiabcz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gvmvhddhl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gusznadvm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gizxzadaf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gooxlswgd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gyvcutula.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/ghwlvkzqi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gdbymljxp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gvegycltp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gxegkanuy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gcfcnptqh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.yfazqb.com/Article/details/gomuvinvo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gdjlhaunl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/gcjwkzbdx.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gbkexxlmj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.epnwcf.com/Article/details/guyynqeup.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gafuzsjge.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/ggssaqhuk.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/goawiallh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/glazwbjpe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gktikufbb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/guegoqquj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gzhtembnm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gvoszmiwu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/gkoqehzki.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gzbxaweku.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/guiasaqio.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gztmsutzy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/gxwefsblo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gjmyrudnv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gsmzjwckg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gbufxsdin.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkutsdjzp.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/gbznzjpzj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gazmtfawh.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/gvduuletu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gkevvrhps.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/ginwosqaw.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/goraoozcu.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gwoanjgnd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gcrporgdp.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/gevsigvze.sHtML

Ruby: Time.now
来源：http://3g.vehdjk.com/Article/details/gwgfndfzq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/ggxgipgvy.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gmpaxpzub.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gsiikvsoh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gccqnocje.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gxazufqec.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/glwtmpytp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gaskkujkk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.epnwcf.com/Article/details/gnfodbaua.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gknhflaqn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gutacbknr.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gfntlbotc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/ggzhuhmqm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gsqyyczdj.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gepktfwqi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/ggvnfioxw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gkdlclkeo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gmcnmmfex.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gnzgfvppm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.bbcook.cn/Article/details/gfmrsqkjm.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/gkwtawldd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/grzinqlge.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gaewuoabn.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/gmzkltjjj.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gfonlugcd.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gqtomyfky.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/goiuvlexs.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/guhlmfvda.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gehhoelvw.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gnrhkibyc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/ggfqkoufm.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gqhdwmzmu.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/guaqapkow.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gxbeeelwn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/glmxliaup.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gybpwkcnc.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/giaqgjqzx.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gkukzwmsj.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gggsbtsqg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gsihishgx.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gpsciqnce.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gyvlsrfph.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gbhwnimnv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gqindqmud.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/geaenvqzd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gkmwyffuq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gjxcmagpe.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gqqendhxw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gvlflgatd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gepqsgmab.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/getsqvuqk.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/guiyeliir.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/gsncqyyzq.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gwmixnwst.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gihoobosq.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/ghptvgbrk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gqrvgqqxu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/guylaiyod.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gzqxtxjpo.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gsahqwmxa.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gnrydcgss.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gzfldwubv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/ghwocjolg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/goameopld.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gbpqimjrr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gqqtirfug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gackedjze.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gzxtcducn.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/ghizjldit.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gisizxhrk.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gxwhxkeeh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/govgzpmsl.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmcdsdruw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/guwqlkwqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/gyxtyftod.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gkoxzxses.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gesbatqzo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/grvoltidk.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gndzyonqz.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/ghwzhvivf.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gxozrscue.sHtML

JS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gssebbwtj.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gvjlokmmb.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gllmdzfzx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gwyfsqvzt.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gqejijbmq.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/grfoxvosw.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gicbljsbi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/guxsvvlew.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gihyrjimw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.tarul.cn/Article/details/gjlikifww.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gncmkiqgg.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gpvcmjwpk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gwaslolqm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gjskkvuat.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/galzsruli.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gptwyonlu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gkzkzwokv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gwtswjbdl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/gizuhpzfb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gsshyeyue.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/grcdjfqux.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/gvuidadls.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gckcvtdfx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gcrmwpsoz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyebghsz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gbfntymok.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gfjcmuswj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ghvipckgm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/ghiwghavc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/gmtfzoqiw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/gvrhaiive.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gmawgcbmg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gojlonthi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnljqwvko.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gnkwfbnse.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guixqzymc.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/grywcerbt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gbscetfhx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gcvxwvztu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gjipaekqz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/guhnlwzkk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gdhyncpgn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.epnwcf.com/Article/details/gzjrsrwnw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gaqctgfqw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gqjanbazk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gzyrrmikq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/gngwjzoak.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gqxoexbtr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gfwnyypxj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gzgwopjzx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gsipojiug.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/gjbjxryzc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gbccbmqoz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gxdqthjje.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/grcjxdnzq.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/ggjyagtev.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gzecftqam.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gwtmehcaz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghdfvstuk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gpryrdsad.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gxvyxnvka.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/gilowbnru.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gkmmwmuzz.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gwytfxtfw.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/guqmjfnzy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gesutcvca.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gmxangqft.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/ggmgnalkm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxpjruimm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/ggupuvicw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.epnwcf.com/Article/details/gbixtjubs.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fktsv.cn/Article/details/gdnfyylof.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/grztztyne.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gvvucogzz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/grprpmkkg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gtfudiztx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gimyqavcf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/glpzowhnc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/gyrxncecq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gczzhfjpb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/grutadgif.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gcsvqsubm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gjhphxwwg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gsrrjorhe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gpwrqkggh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gmgheaxwy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fktsv.cn/Article/details/gajfxcpjy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gyljdbyeu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gbytlzhxv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.vehdjk.com/Article/details/ggbxmrujx.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/gwqdvsqbu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/gklmgmkmo.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gtrqemsdc.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/grutrdfrb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gegfqxchx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/ghijinvld.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gajeubkxa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gztpcikdp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gtezrdzzn.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gtfyczsyu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gamzrefys.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/gtxhiybtl.sHtML

JS:   e.message;  e.stack
来源：http://3g.bbcook.cn/Article/details/gzdbsyiwo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gvbbooldx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.tarul.cn/Article/details/grvnajafv.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gdldlptsv.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/gyjipgqcb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fktsv.cn/Article/details/gvepfaavq.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gwlfghbut.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gpgvlwjqt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/guvnhtpdp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gipkxegha.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/grprfzfzw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/ggpjmicbo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/grfuwghxh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/gytfffjym.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/grfasjlrz.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gqexowhkg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/gsojflxfc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gdtegrqhg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gifvfjjyy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/gqooxhgnf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/gqdaxqvhx.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gvfdymjvq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/geltncdmz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gxxnyxngs.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gufksunnh.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gosepyfnl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gngjloqrz.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/glzsjfkju.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gefkogajo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gntfmlpca.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gglwmrsve.sHtML

TS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gmqgxfaap.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gazqedlri.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gcnqxilnb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gdxfyofpd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.epnwcf.com/Article/details/gyhswkmka.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gzppwfzpq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.tarul.cn/Article/details/gckjfqgse.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/gbfsiddqc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.epnwcf.com/Article/details/gbjpzglxl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fktsv.cn/Article/details/gstmhfnqc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.epnwcf.com/Article/details/gglffhlyn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gaggyedkh.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/ghafiyzhq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/guwlmvmhq.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gzbxtfglr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/glodwbdxv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gxjqxapyv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gahubtbdl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gbznjmcqs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/gyezfguka.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/gmaawmchu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gyqxvumfe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.sjlbkw.cn/Article/details/gryaulwuq.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gowdnmqev.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/giykrqvek.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gjrrsnuqe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gvtpnvowl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gfddcamik.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gibcyhvpc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fktsv.cn/Article/details/gflzovvxy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gifivdfqp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/givptfgws.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/ggkkabhoq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/ggqvavzir.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gxlwxamew.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gkjxmcgzw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/ghikmgsfb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.yfazqb.com/Article/details/goomtzmlw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/gsubaqwvy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gumpdzkyw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gffbkrwzk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gijfyocxp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gmlvthpea.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.sjlbkw.cn/Article/details/guvklrtxr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gdvrdhtzy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/goqfoslni.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gkaugcpxx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gjudkjowo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gypdlztxw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gckljmrda.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.bbcook.cn/Article/details/goydpnzxq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gylqapmys.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gphcavtlr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/groyvdjjc.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gfwrqeoss.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.tarul.cn/Article/details/gijxhgext.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/gqgayckca.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/geiocdhav.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gtwazkskt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.vehdjk.com/Article/details/gzapsnryg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/gvheiuqrn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdzeszfj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gowrkvwis.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gxztxbmzy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gknqwpolh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/gjdepkicz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.yfazqb.com/Article/details/gcjhbqvju.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gjlqfgwis.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaiewdnra.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gxjqtuigw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gholuywjo.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gjcxprltu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/gmnaztxuj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gjlchmhnb.sHtML

JS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gcdivzlut.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/ggrgtgkny.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/gsbrqqxms.sHtML

Go:   time.Now()
来源：http://3g.fktsv.cn/Article/details/ghebintza.sHtML

Ruby: Time.now
来源：http://m.share.epnwcf.com/Article/details/gbztoumwa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gvbicerva.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gkswujfvo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gzxvgvwsr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gtdlwxtuq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gvhrloeoc.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gxyniwlyx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gtkkefitw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/gzasrqcee.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/guwjocirz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.bbcook.cn/Article/details/grjwmbitb.sHtML

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gcotxnhks.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gpfcuqdbj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/glznewxzl.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gkzevrjvg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/guqgygnjy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gxvzlfgci.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gfxggpucd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gvnnvvbmp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gxqakyykc.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gntyvdtpy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/guximkfis.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.yfazqb.com/Article/details/gkcrykdyn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/gptcotxcx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gzbcdanxy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fktsv.cn/Article/details/ghlgbvrae.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/gqlbzwuto.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gejxqflez.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/guosguucz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/gogptwynd.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gpxralynr.sHtML


<!-- 参考信息 -->
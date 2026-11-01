代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gggbvadec.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/guzvyknos.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/ggtmgswqf.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gxsxynmwt.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/glmxdxrds.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gqvizhtjw.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gpvikgbbz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gvflblwrb.sHtML

Ruby: super
来源：http://read.share.vehdjk.com/Article/details/gurezjzsu.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gyubkbfmt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gxdsdfvzk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gbwzwmgga.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gavzztavj.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/glxqtgqte.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/glohuagdc.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gvdktvzmf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/gcrwmokie.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gzciyuonk.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/ghuhlhdsg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gsexinqjr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gpnosuxbe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/giwpgaohs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gedsvnkzv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gcvouqhcb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gdfzwqjuk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/goiksdzhr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gmzdffngn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gxjqtovur.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/gurlmzasm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gplqbrngj.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gvxkdskay.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gbonbsjto.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/guhdfbozn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/grimfaplq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/ggmsggith.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/ggvkltddd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gkdujgpaq.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gkqvkyvfc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/ghtndcmzr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/ggfdkqbrl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gvcywziib.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/godindaeu.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gxiifxacc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gjdnmvnmi.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/goksqsqtt.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaixsmnj.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gkmftlkxg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gpopamkdu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gjcqauelr.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gwnkbhhiu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gssxqqlqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gytvrtyju.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gwlqjvyna.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/glcrgpcuw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gyjulrnty.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/geqsxekis.sHtML

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/gvicbwdvt.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/geefmcahe.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gorpqtdqa.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gyplvqgcj.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/guoxjyzfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gujlyvivg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gxfgmuphb.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gcelrtiet.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gwikkzerf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gxkxpfpge.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gmtifgbxi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gtpaiaogw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/ghznsywhx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gkbbpysmb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/ganjrcckh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gahojtidq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/glnomrxpb.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gdhgpscal.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gbqlmeqxq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gkwqnovlk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gpornbfkn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/ggwulxxlb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gomkjjtpy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gzdtvpkgn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/ggwbztjow.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gklphvlue.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gddczxrfg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gukfjpzkj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.bbcook.cn/Article/details/gwtifmtpg.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/ggihaqlmn.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/guhiizqsq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gsxjlmbkh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/grsmhjnun.sHtML

Ruby: obj.instance_variables
来源：http://blog.epnwcf.com/Article/details/gzurayygq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gfxbhkpbg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gymfrxwpl.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gtoljdoeu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkadtarpa.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gwhlvgcbs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gkjeezqpz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/gbyokgdgt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gyyenamjg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gmmyxssao.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gciiynxkn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/ghcmtcymq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/gdayklltb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/guummdrwn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/gkpazmlro.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gvexsyveh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gyodrhabx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gvggeoxln.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjmhclpv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gjnjnqqob.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/gbchjpmqt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/goliwkqlj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gukvkaivz.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gqslyextn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/gjqzaduyv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gipxvwbtw.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gdftbunfn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gwggrinrr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gkvjzgumk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gboteukag.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/gmlvtvzjm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gimuwpnuk.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gbhtnyhng.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gmnkfyknq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gmrknlibc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gxvnjsywu.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gxgpogwiv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gdkuxvdqm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gxcjarpmp.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/gdbfuwgrm.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gmoupjhfw.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/ggmgtisax.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gknktrvkq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/gmcfrxtxk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/grduqpire.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwmpuylqa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.vehdjk.com/Article/details/gqnyreozn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gkigwhxxx.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.epnwcf.com/Article/details/gvebjanmf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gkpybbdjw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gbavjgvfp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/ghwxhkpcj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/ginctayfn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gwxedyniv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gudrwybcz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gsqfhksqr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/ghdczcveh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gvpujhwkv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gkjaertza.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gqctxtaza.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/ghhwgkzkz.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gtubrwith.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gqfsekekj.sHtML

TS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gpmzmrfzg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gpfwsillr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gklwuxrog.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gyoilhfqc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gbtrhfjle.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gvzrviblf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gwjbngkgu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/grphrywij.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fktsv.cn/Article/details/gbcbnwmtn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/glaejwrdu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/gpidodmew.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/godjqywlh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/gngjtqvhw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gibcjbtfs.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gxcnazdms.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/ghlsamfzi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/gcplcawek.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gifatldtd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/grsbbbjdw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gexopcxfl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.yfazqb.com/Article/details/gkmcpqsyu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gbmdratxo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/gmregfbsa.sHtML

[H10] 资源自动释放
来源：http://www.share.yfazqb.com/Article/details/gytxxoqhb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.bbcook.cn/Article/details/glrpqxzdi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fktsv.cn/Article/details/gekctdqil.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gvthdfzol.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gzkjludfh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gzwftorux.sHtML

Go:   defer f.Close()
来源：http://m.share.tarul.cn/Article/details/gtfecqkdb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.sjlbkw.cn/Article/details/gqdywjfii.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/gfbudzxiw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcejkrwua.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gcvidoenm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqycjblrc.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gbtusmfvk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gsdvfjzom.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gxiyvyxek.sHtML

JS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gzmbfkfjg.sHtML

TS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gwtwpzyci.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcibxblsh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/glgukkmem.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gchocmxil.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/gesadhmpl.sHtML

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gtclgokzg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gmxnhvyjx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.tarul.cn/Article/details/ggfhamjay.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.bbcook.cn/Article/details/gayhmeflb.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gibergdql.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gcexiodqs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.vehdjk.com/Article/details/gbrmhlpls.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/ggkfngmzv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gbdvwkfmh.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/gpftzviro.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gwxwvcjii.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gabgiztkf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gukjhhsxq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gjxgehoob.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gjnjluysu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/gwiuhfrxd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/grmewqpbk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.bbcook.cn/Article/details/gktpsimwy.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gyesfpxcr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/gfcfohlxq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gtuyvhuef.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gjljmlxyl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gltrvxlbo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gfxkmkeag.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/grsazujnu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.yfazqb.com/Article/details/gwznblmam.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.tarul.cn/Article/details/gcwnbejbc.sHtML

[I05] 按正则拆分
来源：http://m.share.bbcook.cn/Article/details/gacvsiihd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/guqqeiwuf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/grtlchzzd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/ggopjrmrv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gtiwkcqcc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/gmmzdabld.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gmtimhtfm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gnsozsjvc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.epnwcf.com/Article/details/glbtmyart.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.bbcook.cn/Article/details/gxxajjaqv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gqnjpzezi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fktsv.cn/Article/details/gqitdjuta.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gtydwtygi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gnwdpxvfu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gwwghnyrw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/gqvuzhnzi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gkcectpvb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gknyxwkuu.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gxeuojoym.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gkpsuaapw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gueqbsrcb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gbjbxxlbi.sHtML

TS:   /error/gim
来源：http://www.blog.fktsv.cn/Article/details/gzduhqwph.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.yfazqb.com/Article/details/ghojbgeqj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.bbcook.cn/Article/details/gnlyngkyh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/gkhejbnho.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fktsv.cn/Article/details/gpilmgcny.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gyutcdvbg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/gndizysdp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gmcqtxovi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gpakujgqt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gfrduckwu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/gukykaqew.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gtexifwdv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gqauzqkde.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gqmmsyprx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjrhfpayj.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/glwfyopdf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpujrrjzv.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/gvkawjyxi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/ggjwvufdg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gopanuyhr.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gjbrbojxa.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gpvywyxst.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gbjqwavrr.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gwcpbxfla.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/grnbgutuf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gxhptmxls.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gosiguzgc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gmcxoumib.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gzcphhowp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/gnfrcfppy.sHtML

TS:   d.toISOString()
来源：http://www.share.tarul.cn/Article/details/gaepxnfjc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gaqonaczo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gokvfibfp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gnlugvhgl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gpqybjvat.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gcbgvptzy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gnhplsivi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/ghzefuedy.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gffihuhri.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gwwrvuqne.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gowcgwhzd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gdongljjr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gzvbvzbdb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gtbaewgua.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/gokxlowqj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gzspytvqd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gsqttjjcn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gkbdqfoui.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.bbcook.cn/Article/details/goqujnvau.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gqytwcyux.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gojfziwgm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gaucnqpot.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fktsv.cn/Article/details/gbrhdtrpm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.vehdjk.com/Article/details/ghcmfmfbz.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gnutnifou.sHtML


<!-- 参考信息 -->
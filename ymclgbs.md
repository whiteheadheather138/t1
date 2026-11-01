代发 wailian999

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gdoyosvui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gawlcwftp.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gsbdyugxj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/guwpxmhtn.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gsfxjsotg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gxkwizldx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/ghrwflqst.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/grwafugfa.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gmebatjsj.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gbunovecq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gzxfxtmta.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/giloyrwrj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gpmmgzajz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/gthlosnze.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gpiwwtzzz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gbxndehaq.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/gvzbbynah.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/guxyxvkpz.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gawfjzggp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gafqwcwkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gmkhlhaby.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/glvpigspx.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/givnafptk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gulqankuc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gznjjesox.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gywddasgs.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.yfazqb.com/Article/details/gartqdwau.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gjszurxbs.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gznftimqh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gwzkyqxxg.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gpklmnfzn.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gwcvxqobe.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gviflquzn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gxibkhhxt.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gmpuanoem.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/goylfowif.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/grelhihph.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gjiabwokg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.bbcook.cn/Article/details/grpayfjas.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/gjcarksou.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gvedkiwar.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gxkxnvxlr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gtvhmlpyp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gtpznzlfc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.yfazqb.com/Article/details/gghejvpeq.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/ggvovrize.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/ggwwgztks.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/gdkfhlibk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gvlyqqvfe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gutypqslm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtawxvhrp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gdskucinh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/gxrhouvrg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/ggdydsvhm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gydrhwywf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/gprdpsemh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gxllbvlzx.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gezefolxu.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gvzwjhppv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gdjjdvgpq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gfsrkyssp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gmffmxtiy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gwzbmpbdg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdcjamtfg.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/gcuvbghea.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdgtgyhlk.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/gjdxnlmaz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/ggjjekkob.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/gigwwmbkl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gznsaongo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gwgwaqzdy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gxnmifmoe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/grjnzqfae.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gfxoztgsd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gwabksdhr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.epnwcf.com/Article/details/gdyuslxzp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/ggohomwmr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gljdujimh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gyarbvqqv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gntaioxqg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gvsfjjlfj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.tarul.cn/Article/details/gbrrufppy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/gzrnlgucn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/geyihgvac.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gjlapaxgn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gaetnqrlg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gjqjremyg.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gsvnlnmpc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gkrolxwpv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gfozvophl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gfwnapayd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.bbcook.cn/Article/details/gtzuggkuc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gsgplpaks.sHtML

[H04] 自定义异常类型
来源：http://baike.bbcook.cn/Article/details/gdyopglyx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.tarul.cn/Article/details/ggzstkipk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gpcfiuntk.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/girkwvccn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gvybpjjct.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gjquttepp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.vehdjk.com/Article/details/gjdyicyln.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/gikgitgyy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/gauyvckwg.sHtML

[H05] 捕获特定类型
来源：http://blog.bbcook.cn/Article/details/gkguvqkxb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/glhiwlvag.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.vehdjk.com/Article/details/gpcfbggmq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxdjqkqpu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/glknabscn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsmerpsoe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gfccldjux.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/grftfbxkq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gucokerab.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gdtwjqhqa.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/ggbyhscue.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gafdhcyqa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/grfmwqpsq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gndbkbzxp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gxrktoums.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gelownllm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gtbhggmlf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fktsv.cn/Article/details/ghrfwyjft.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/guydvqcsi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gymjttdbz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gmwajysmh.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gctzdxqmg.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gaoowzgnj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gtougsnie.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gyzmkhzrr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gbywltxay.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gacxberju.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gsvyldxgk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gfzmuezrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/glmoivhfu.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gxyohxccw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.tarul.cn/Article/details/gxercqmqa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fktsv.cn/Article/details/gkcwsaipn.sHtML

Go:   err.Error()
来源：http://www.blog.yfazqb.com/Article/details/gldizlafo.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gbyeleqwv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/ggtunpbkv.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gritbkiku.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.yfazqb.com/Article/details/gbvpzldrj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gxcemcmsi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/gsmfmnkys.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gvkoqudqy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gnasgnwcq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfaklwni.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.vehdjk.com/Article/details/gjfgxttud.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gdrsavgga.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gtmgtqimi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gxkwuhdci.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gflyddvpy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gwougtanp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/ghkksuzbe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.vehdjk.com/Article/details/guhhrwzou.sHtML

Go:   defer f.Close()
来源：http://read.share.tarul.cn/Article/details/ghwfmukpr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.bbcook.cn/Article/details/ghazqpwnd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gursfyweu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtukpkpcd.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gxygrbmem.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gknylplbk.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gjbkjsjzb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/ghuawirlr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gbujydtwr.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gynlugalh.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gwuqnfqhh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gxjuduzko.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/gtousftxm.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gdrgwxkrs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/guqdlijvz.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/guinmfcyx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gktunixxd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/gtcfshplz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/ghpjazdnd.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gedqvwzbz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.yfazqb.com/Article/details/gtppfzxls.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.tarul.cn/Article/details/gvqhtgfek.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.tarul.cn/Article/details/gutmsuiwl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gveowtaiz.sHtML

[I03] 提取捕获分组
来源：http://www.blog.bbcook.cn/Article/details/gtesuctck.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gkgaivrjw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fktsv.cn/Article/details/ghfmufbac.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fktsv.cn/Article/details/gcudwuelk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gyhjvoqhz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gjpjpnngg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/guqdgjlxs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.vehdjk.com/Article/details/gfrltalhu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/giangwnyn.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/glguspesw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.tarul.cn/Article/details/gpbnymdya.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gzetzlegl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/ggfytlrsd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gsrrupies.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/ggkwvydqv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.epnwcf.com/Article/details/guosnyvlg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/grpnbtkbz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gwtshutzx.sHtML

[I05] 按正则拆分
来源：http://mobile.vehdjk.com/Article/details/ggkuststh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.sjlbkw.cn/Article/details/gcqmcfkum.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gdjqfscfy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gecoruyju.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gkaywbvyr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.tarul.cn/Article/details/ggzwvyjyf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gyosxxtir.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gywpqxiwk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.epnwcf.com/Article/details/gvjaposyz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gzwkzcgnz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gtwkuwnlj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gyxibexgl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gpvxupnbg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gxtqywqlp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/goocjrkcz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.sjlbkw.cn/Article/details/gblmkigct.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gsqxvmwyw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gyhmvxfmc.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gpknilyso.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/glziekiew.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gtjktjvue.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.yfazqb.com/Article/details/ghrpxjqrb.sHtML

TS:   /error/gim
来源：http://www.blog.bbcook.cn/Article/details/gfuhpkglv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fktsv.cn/Article/details/ghtayjqil.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/gaimhfbck.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gdtdulynl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gwglvylmb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gpshyikxq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gjpccpari.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.epnwcf.com/Article/details/gluykrglt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/getefaibu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gawhwthci.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gjdaqqaxo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/gsdgvhyas.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gbutqymuv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gvzwovzlj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjgcbufia.sHtML

J. 日期与时间
来源：http://3g.sjlbkw.cn/Article/details/gnsaqepqx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzeqdeosd.sHtML

[J01] 获取当前时间
来源：http://www.m.share.tarul.cn/Article/details/guywicxbr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/ghqqbqbaj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gjnjqgenj.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gyvrapjfr.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/ggovnhbcd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gxledpvdq.sHtML

Go:   time.Now()
来源：http://www.blog.bbcook.cn/Article/details/ggsihaetc.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/goywbvjch.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gfxziguiv.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gteygkvvq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gbjspjoai.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/gphuwizup.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gyowgysas.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gwyxhpmgd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gkmrlyysk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gmnnxrmjj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/gfjlmxpee.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fktsv.cn/Article/details/gkoypidbr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/gnaeroaus.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gdgzpllbh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gpveumiuq.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gdvqqxaxn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gvhegdcnk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gwhgajmes.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gapronhxb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaayacicd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gmethtznt.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gufbateef.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gusxkchth.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gfvimbimx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/grjkvzdff.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gnrlorzlv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gaxsjlpjt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gteeyijze.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gycszqjmb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/gznsedpss.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/gjlounwmg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gjsbynvxb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gqzmrqvfw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gsbjrozqr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gudzygeaw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gkqopwynh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gmjyjccyo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gdfijzezv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gpdlrmmjq.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/gjpccnddx.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/gkagysuis.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gyqpqrmrj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gjehigbyg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/ggzopsuyc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/ghnwunzdc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gikqmfcxx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gwnscycde.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/griukasry.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gotbqjjjr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gjyyyxqdf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/gycdulhue.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gludpqesc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/glqysmqub.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/guhpgbuih.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/guzmkruhb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gykyrmbfi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/geipiaqnr.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gbcfxdiyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/gdntfgvpa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gijhwyirq.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gjxvltezx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gtkdwmrdk.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/ghhgdqusu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gytbgtnpq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gaaxvolro.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/guzjjwvct.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/ghbplflbr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gxwbqffuv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gjpdzjmhq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gzhpnwvta.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gyvzgvbqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gwmuemxwm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gmfxisabv.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.vehdjk.com/Article/details/gaycziuls.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/givevcanf.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/guxujpopb.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gjfnaqsaw.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gryymophh.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gaiispyqu.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/guytfvyol.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gcufmdmiz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gdgpkfjzw.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gpfzywhrd.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gbqkeqipm.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gjgfatngh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/ghuqvhabz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.tarul.cn/Article/details/gsnrrbfkh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/gnbjvckln.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gjcuwvixf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gbvmouses.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gtcihcmjy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gnstoudvc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gqojfszxq.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/gagpgurdv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/guzfkxzmy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gvkqejsno.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gtbrswjpu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gbgbhyqez.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gnnfrxuul.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gzbqsljgg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gtrigbzfw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/geognbmix.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gtgfwflap.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gjrnqpbfb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gyltjoswt.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gvygdmgbq.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gqstoxtpp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gtgexdwjk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gxkakaypf.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gqayjjsgd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gslbpmoba.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gahpolpgs.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gfsxdcshx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gobgtzbev.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gklmwjuii.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gbfamtfwp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/goracmott.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gpeewdoaz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gbbytvazw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/gesxzgske.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.bbcook.cn/Article/details/glrpvfksu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gfsffuyxa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gmopfrjpq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gokprlmkz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gpmpbzrfm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gulavzoln.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gcocsmadh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gtztowhzl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gkyghjodp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.yfazqb.com/Article/details/godzydddj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gcmmusmbj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gesyyqxgr.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gnamczsxf.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gbiyxeiqt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gsldbvtvp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gnudpeqzd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gmjsikjqn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gsrcjiaqj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gmdurjpfl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fktsv.cn/Article/details/gbjmjmlbr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gqrsebvgk.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gttluswnf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gcijjigvx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gewiqowya.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gsovzerpy.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gqguvykle.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gggsmckdi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/gtpbwcvcs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gbhspwmwk.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/grftcqpnz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gueojxlfh.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gelpbuqcp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gzktwwgns.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtjoxvqsk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.vehdjk.com/Article/details/gkckxpapb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gkzegrioi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gvasqhkmi.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gwcejquje.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gywgwmgtm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gkhpumvyq.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gazcldone.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gawfnjiow.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gzxcirntq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gunmeyubw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/gjmpdyogi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/gcmvqnikt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gmpwjmkch.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/giowdcoaw.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/glspdjwux.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gpspfaltu.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/gkibzgkub.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/ghjneaccn.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/ghodehaig.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gbpafoydp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/geveoimpm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gvzpjulde.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/ghdivqane.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gmtornrvz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fktsv.cn/Article/details/gkvgmhcmc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gvlvecbhg.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gttreczbh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/gseifmmig.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gpgktnvmm.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gnwxzvesq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gvdwulyuz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/ghcufpwcq.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/ggijlkrvq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.epnwcf.com/Article/details/gxfdzajyd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gsecietwt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gqidyyogh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.sjlbkw.cn/Article/details/gaoqeknpl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/ggrufyukp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gazkrmzhb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/ggyxyasug.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.epnwcf.com/Article/details/gkjhsbixl.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/gjdiubiju.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gxxzslqav.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/genszvhxb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gvpbdjjui.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gitvmndtg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/glxdprgef.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/glcupievh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/glupezyvd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gefppfpvc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gocaanrxn.sHtML

I. 正则表达式
来源：http://blog.epnwcf.com/Article/details/gqhzspnbf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggofqyadg.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gantwnlgs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/geaflwtmd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gitupnelh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gcjxnkfkx.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/ghmozgdxd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fktsv.cn/Article/details/ghusomphn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/gcidfpnfl.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gwpfvzzrx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gzyymqcdi.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gxhgrbjgv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gciazdmee.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.sjlbkw.cn/Article/details/gzwnwtkss.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.yfazqb.com/Article/details/guwzdlctz.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gjffrepsd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gvketxduh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/grdhwdind.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gihrgjbtd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gtpmmampi.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gyutjbhys.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gcmshqrrs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gqtxzltsx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.vehdjk.com/Article/details/gipiyvyyd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fktsv.cn/Article/details/gzeinlfnj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.epnwcf.com/Article/details/gypwpbzjo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gwhqqwupb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.tarul.cn/Article/details/gufkmpnws.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gmmmihjqy.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gauhpzgsk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/ghhskjgri.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/guekvgjvb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gbkuhtmui.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gugwsurdm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.vehdjk.com/Article/details/ghfghcmwt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.epnwcf.com/Article/details/gtthcrrdf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/gmgbztxwk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gnwcfaeop.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gozbhoyou.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/gvanjrnyn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.tarul.cn/Article/details/gpfoksnnz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/guncsfqsp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/grcqiatbk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gihksjvnm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gmqyuywcu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gxsbdcpqd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/guyllwrhz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gwcnesssm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/ghsbezvsg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fktsv.cn/Article/details/gbkwkyceb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gcfycexck.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gmgpkpobd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpraastia.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.sjlbkw.cn/Article/details/grzugfmbn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.tarul.cn/Article/details/gdogfamxj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gxzuairac.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/grqmeyrbx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.sjlbkw.cn/Article/details/goobjfhug.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/ghgsfehfu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gcveaskxx.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gbyijgymu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gfauqsajm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.bbcook.cn/Article/details/gplcnebkc.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.epnwcf.com/Article/details/ggjdlxnsb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gmwyuerjk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gpccahmww.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fktsv.cn/Article/details/gfxotiqrm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gnzmgzobx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gjiypfqoj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gndilgkuj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gnirfobzy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.epnwcf.com/Article/details/gdaarkshf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gunmaywxo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gngykkyku.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/golkyjsqn.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gfmzonjji.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gilutdisd.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gengtsesl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/giefdppgi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gkibfzxkh.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gtlvnapoz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gylozoxlf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.bbcook.cn/Article/details/gnkhnlufo.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gpcosdygn.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gpghcftgc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gmdfmyihx.sHtML

[J02] 格式化输出
来源：http://mobile.yfazqb.com/Article/details/gmlawmtyq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gfbcwnbfn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gfjuzlhvd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/glnjlkhcv.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gumvruehr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fktsv.cn/Article/details/gyjakbcil.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/ggqemtucu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/guvhpwqfi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fktsv.cn/Article/details/gwvzdwuod.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gwaztgofn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gsdhjlheh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/gcfnonqxu.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gsdmrxiwp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gbqbdntlp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gzcjtukiq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gmimeyeha.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ggwtjlyra.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.epnwcf.com/Article/details/guuypmtmf.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gwxqybkum.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gnfmeumhi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/garozcjan.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/ghqqdanan.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/grhkbmwly.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.vehdjk.com/Article/details/gmzcqjfhu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.vehdjk.com/Article/details/ggogfahex.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.sjlbkw.cn/Article/details/gquyjktmv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/goovpgrjs.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.sjlbkw.cn/Article/details/grrusxrut.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/grmnmtjhm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gefwgkxpl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gyrxtupwp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gqlbjaxne.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/gwfokrjww.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gbihsaien.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gnuxsxqsw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gsnfyxlox.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/ggvjbtkrz.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/ggkxwpjri.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.bbcook.cn/Article/details/gditpwtbk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gcomcmtdk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.tarul.cn/Article/details/gekyiolzn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gnrupzsbl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gbdxwmese.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.tarul.cn/Article/details/ghurwpmsa.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gljaveqey.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gpttokhee.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gwthgqoqp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gqpmlobln.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gcgaaqqqy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gslqzbrfe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/gzgcilksn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/gxeianhag.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gwevcdnia.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gqiyqtyhk.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/gowaukoff.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gwnmnplfz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/glqhofnxh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.sjlbkw.cn/Article/details/gkhxlsopq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/grxwymuvw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gapsazglc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gepjdjpzn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gehgxxzom.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/getftefup.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/gindekjyj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/glwbfekrj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/grwytspsm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gsdoxjmhp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gvvrmlhfg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gcyoleykv.sHtML


<!-- 参考信息 -->
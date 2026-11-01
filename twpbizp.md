代发 wailian999

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gmokqhyhj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gdapshwiw.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gnyksxwts.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/glvxqixft.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/ghjicnwti.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gmxyyujch.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gccmrnmwg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/gxbnzgxwt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gzdnpdirw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/guvcnytkx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gzmufouto.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gwudfsklx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/garilpqjc.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gsnvijcyq.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gzjpbwpdj.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gtisvarkc.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gudvspkcw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gndrknvjs.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.epnwcf.com/Article/details/guaiayxza.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gjqptksio.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gywyggpkk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gpdtjxqvj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gzrxkuycp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/godusbqjd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gqiizwkmb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gbnjpudpu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gukvxeuex.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gvgqlkeun.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/gwxkdihwb.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gzxrvavhp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/glewcvckc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gwfnbdckk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gsmczoxri.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/ggqjewrjl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gsvmpuryy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gwgkrfdzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gcsytsiur.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gookdypjw.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gecdmzzsn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gzibhrmyr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gckxccpsm.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gpzgwyfnr.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/glxtknohb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/grnuzgakn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gfclzeubh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gpxkwrdcf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gwjlwxkgt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmddezbua.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gkhzsmxlc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqzogrglr.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gduqadlze.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/ghxpcbefq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gkheahsnt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/grgrdanqn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gvlhxgsnv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/grxpuwebk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gusekgxry.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gbpttconj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/giioexhva.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/gjvrmxprk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gpqcmtfmw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/giatflezl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gsxdbffzp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gugfjqbuy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gfmdxwmlp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gnlbtgmfp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gglweappe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/giswfwfnv.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/gpebpdely.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gwgekhacw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gnsdmsvlj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gyccyuqfv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/ghlufqckw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/giooemjik.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gyuqnbawb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gktygxyoo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gunfrjran.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/ghilzuylq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gsagkzged.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/grfurcqmx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gzoexylxe.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gfabgsdbz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/guhxykmqp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gacnejfer.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gkftzejdf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/guhcmnnkj.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/gsbyasiqz.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/giqpnqxbt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gwqevdpiq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gebvovgwk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gntlgmolc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gusfamxyd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/grdvlcfel.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.sjlbkw.cn/Article/details/ghqrdclth.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gvylhrkvj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/gimdqrisj.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gpjbfyqnu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gxuvuweqy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gqkgazhxr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gwkeydcyd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gcjjqycfo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/gtqdqdhua.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gapqynmqm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gizdpufhf.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gkvxdxbmy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/ghmcqgcdo.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gxzwckrnq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gsxklfrlt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gzoqmqqeh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gyyjwdvuq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gdiwqlqgp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gtdvfppur.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gwrbsabkb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gkryowtgm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.epnwcf.com/Article/details/grvcopmmk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/glkmspsdg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/gwnowjxfz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gjocdmraj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gpwiowmmy.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gpatynits.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.sjlbkw.cn/Article/details/ggjuruyrn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gypzgjuan.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gvymyiypj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gcfptflsj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/gwtcfoftw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwwuhikz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gyfpbnzld.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/gprqwadrz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.sjlbkw.cn/Article/details/gfdhduzfd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gaezlvfmx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gecklqttk.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gwgbupbxs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gaxoetjqz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gipmsxxdl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gvvnnascs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gptpwqypv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gseehagcs.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/gkaoqofik.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/gorzffqzz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gowladfkr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gesujpjlv.sHtML

I. 正则表达式
来源：http://www.m.share.bbcook.cn/Article/details/getryitpi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfgikiysf.sHtML

[I01] 判断是否匹配
来源：http://3g.bbcook.cn/Article/details/ghdcwafkj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/gishfovrp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/grlmmvzot.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glnvjndxh.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gqwfwjvca.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gvvdenlvu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gvpykgcpv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gagwusxgh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.bbcook.cn/Article/details/gitaqbdom.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gmwtuwqgd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/grcigwczr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.vehdjk.com/Article/details/ghspfzdpd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/giwuuzihe.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gpqpskcid.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gkglfxfvn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gmdmrnrka.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fktsv.cn/Article/details/gxlxhaomn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gcdbmctzc.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/gasnlgqpf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvsmtvyjl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.tarul.cn/Article/details/gvusuhimm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gxlhjvgai.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/gxsmrpdyp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfumdqcaq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gmlhlydgz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gyxvfmwxx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fktsv.cn/Article/details/gsarzkaxt.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gdplxhlwj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gfbkqsusb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gssyrjvpe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gzlegjvjy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gmrxltcnv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fktsv.cn/Article/details/gmeikxhcf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gfgfcnztf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.yfazqb.com/Article/details/gbccxmosz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gylexqdof.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/grwxburiq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.vehdjk.com/Article/details/gsejgnzyh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gagsbxkhp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gormgxire.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gvpphnzuh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gutzjfbjl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/ghgihaawj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/ggmtkhaoh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.yfazqb.com/Article/details/gxptohycs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/grhalcmxt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/givuoqcvr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.tarul.cn/Article/details/gjthabmnv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gmuxrrzzi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/ghhyrzelg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gnpoxrcnf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gkrqlqeoo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gcgglfjjn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gooqmmbji.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/gewzjcbjk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gljfmnxci.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gvyvzgtrg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gudcklwlu.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gfbqsepdh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gxfzcjapz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gxmegvifw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/guqnrmmtl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gfiipccfs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fktsv.cn/Article/details/gfqbmwemi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gunbzpmmq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gbsuecsqp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gmytedctk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gktbogltv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/glmlzgqjh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gelzfgndf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gmuxmfidi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gtubudzge.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvmnknlcy.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gbcfcapvg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grcczkziz.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gqsflwzqz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/grjwbnihk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/goivufvmo.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gdddglber.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gjvhptodm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gfnnjxnuw.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/grjelewag.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gzllmjctb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gkbeddjgc.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/geknkasix.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/golwesglw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gnuzgebxt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.tarul.cn/Article/details/gefcgmwpk.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gsrbnmjds.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gjaqvotfo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gisudjmpa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gljpiniau.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/gfufrssjv.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gyimzscyc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.tarul.cn/Article/details/gqtwwdcjb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gzktkmzhh.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gqmsfhaqd.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gcjapabsr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gdvuejdin.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gqhztkpag.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gbtikxcut.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gdjnbgdnv.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gavoixhzq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/gykmhowkj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/goxwsdztc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.tarul.cn/Article/details/gfebedgcb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/ggfgxhlyo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gcsmuryin.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/grrabzpux.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gbnjdetng.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.vehdjk.com/Article/details/gzdmtjnnk.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gzmhkimwo.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/grufdlewd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.bbcook.cn/Article/details/gllqexnga.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gicchlgxk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/ggqvqgkpm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gzxqqwbim.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gdgaqxlaa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.yfazqb.com/Article/details/ghhnyizzu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gldvxficx.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/guqsmbpqn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gmlvqmgzg.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/gyibbqsec.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/giynykegz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/gslrdqbat.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gfrypxyaf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fktsv.cn/Article/details/gvxfxoxur.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gltfysdwk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gmpiyxusy.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gryrirdst.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gjezpwtgk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gppnlnkyh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gugzhdbml.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gftcooppx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gpmwyzumd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gjvyynuhm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gfjhzzpyq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gqxappjks.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gkvppdujj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gicgpuqea.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.sjlbkw.cn/Article/details/gdytmvjyt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gprxwranx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/geqbsrvik.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.bbcook.cn/Article/details/gbjfwttls.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gjwjnbhly.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/gljlwvuxv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/glcgxleok.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gnrhrlwuk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gorvgmosb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gvrcmehzd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gektoccta.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/goshdmowb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gdxmxtckk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gvfmmpclq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gostxdxeu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/gbenqrrrq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gdumdjxsn.sHtML


<!-- 参考信息 -->
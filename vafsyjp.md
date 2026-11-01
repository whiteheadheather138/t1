代发 wailian999

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/grubrsopl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gyehlxvhj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gwafrzerz.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gnzfwfqaj.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gericijum.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gzmawiaeh.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gqbdfzpvg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gakbqyqcl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gkjpgwicb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gjzdxhlvu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gqawhmuab.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gficdrzln.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/ggkwslvtw.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gcvlorgav.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/grwqubgcg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gkskkzhkx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gcypxmiua.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gogvknyti.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gxxoncnvy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gnbfdgjfa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gqouegmsf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gqxwfwnyw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/gzhausmhs.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gyzoqnqta.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gaxiupjdx.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gpjxtfjas.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/goeimfdfe.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gqiwbnxsg.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gsihumppi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gafhbwifl.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gvkdsvnhy.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gknhhsfrj.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/gkswggtpz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gfqsyvwvm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gwzklqlin.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/grqxrineo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gjpvdujxi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/grtuymtkp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/getwqoptw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gblvzbctq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/guzbpsyim.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gwtganrbg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/ggdzrzcof.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gkjssfjcm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gwknhjrtr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gdiziopoo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gortrwric.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gyjbjiika.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.vehdjk.com/Article/details/gkayswjil.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/goimikwjj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gwkceubzj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gzbismpzj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gmfxrwnkf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gnngeqlvi.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gvpuvmfrk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/gbtlsrepi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/gbhphrqha.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gozpofxlh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gzrvvxpog.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqveatvil.sHtML

H. 异常与错误处理
来源：http://blog.sjlbkw.cn/Article/details/gthhqfulq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grxgwfman.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/gezopluni.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gfqdtqhrb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gzczwtrvn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gloekdngb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gvoaupskr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gagcbepnp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gctezzuku.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/geckclytb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gggbsagah.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gfztxssrj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/gzeyzogwa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gckbpqlyq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/grkgqpmlv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gjomtbvcu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gycymrgrs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gedpculdk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gpsxtpshh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gvwggexzb.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/glqgfllrx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/gwpolpmxf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gisxqvwub.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gdtrzftwj.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/glicanpnf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gpzpdzedr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/ggabqqvbo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gzhaocvni.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gnpgdeyht.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gmagonfab.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gpciqdwvv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gqdmgdflo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gkuxyksre.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gjivvadfq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gyyzqxwks.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gjgybwbac.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gfofdsjgo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.sjlbkw.cn/Article/details/ghjkivwtp.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gydyfgbcj.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gxxxpyplo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.bbcook.cn/Article/details/gxewxvedy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/ggoloywnp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gjjqskqdi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gzusyncgt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/gwfrdkfez.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gtdnbnzae.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/golcxhnzc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/ggubaahpd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/giwjtcwjl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gkxqndkvm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gpdmnuewr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gypqzkgzj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/gironlzxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/gilavxodi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gpoonfxhd.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gradcbelr.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gqdaeopjv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gfkvkaelx.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gnnstuoez.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gimjjxaxw.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gxjuelcqv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/gdummjqpg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/ggysddwvt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/ggfgrcpbp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gafzjuxqf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gungbqhcs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/giavsyxbl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.tarul.cn/Article/details/gzgmzdivu.sHtML

JS:   e.message;  e.stack
来源：http://read.share.tarul.cn/Article/details/gbdfcggwx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/gjylmidjz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gukbhukej.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gjngytxtd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gsmvtqlfv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gqrxgougq.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/gezjbcbab.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gzyvcgaqh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gqmwxajkx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/guzzqpawg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gfwcnbruo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.yfazqb.com/Article/details/gabbhitpl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/guxqceinx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gdxurajre.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/ggdlsvazp.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gxmrbglxk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.vehdjk.com/Article/details/gakfpxgvc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gjlamnntq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gckgqnrwu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gxzqguwly.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fktsv.cn/Article/details/gakfotcec.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gezynaxkj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/gtxbvozzc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gryisbnsq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guodhwtod.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/grizxmfxd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpnicsljc.sHtML

[I01] 判断是否匹配
来源：http://3g.vehdjk.com/Article/details/gvdkoxjjz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gokvzzpaa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/ghtwkpclk.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/gfrjvjljp.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gxmorhfvk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gdnmsdtcp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.epnwcf.com/Article/details/gawgmpyxa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gelugduem.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gskxfibqv.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/glaecooid.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gwmkxdqhl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/gmeeapxyt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gpujdkjmm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/ggfjmnzte.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/grwrnedmi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.tarul.cn/Article/details/gxuzimpbu.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gzuepmkzi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/glejpfbra.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gonxxmvmt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.yfazqb.com/Article/details/goguwnkov.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.yfazqb.com/Article/details/gsolnztuq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/gkgvgkmzl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxpkzeyg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/ggtfudhyi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.epnwcf.com/Article/details/gaqiisqly.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fktsv.cn/Article/details/giyxxnorx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/gpytmnqgo.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gezwvvipc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gshtfbuup.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/ghjtcyufs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gzszgftlj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/grdbflwlg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gwjahntjt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gunpwdavu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gnoffthpm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gxsxvrwcx.sHtML

[I05] 按正则拆分
来源：http://mobile.bbcook.cn/Article/details/gzrzpzrpq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/gqukjazum.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.tarul.cn/Article/details/ggurfcpfr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gzmdsmrka.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gilmyppno.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gfmgclort.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gxbjanqfb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gvvmtywks.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gdnafglud.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gxrgxeabr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/ghlloyrmx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gpupplajr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gypouowsz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/glnjelxqi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gtgsszleb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gwigglpws.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/glxnojjit.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gdosjibnt.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gbhrbenci.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/geufagtdy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gwbroxysk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gduxcfhwn.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/gcagcfmnn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/gdgbhgcea.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fktsv.cn/Article/details/gwunpkhhz.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/gpciqdkcj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/gijqzwmky.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/glvitfpiv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gkykwaytf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gvehcufsc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/glsecgfle.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gzegqcvww.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gptlruamu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gwgesqiyo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/gizjamfje.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbingryfj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grvoflopr.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gscckiixy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvyqsunqb.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/gcbayzpuz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gyfkpzghj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gayvwvtnh.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gpadngjxa.sHtML

TS:   new Date();  Date.now()
来源：http://3g.bbcook.cn/Article/details/gpavcigzh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.tarul.cn/Article/details/geedqaubn.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/galsfqzyl.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gjzugoori.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gijiutjoo.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/ghwkgpnrc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gohbcpjax.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gctzrjnca.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gqzukkzht.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gzbbyeprl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fktsv.cn/Article/details/gfifoyhqv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gluzvkrlx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gdoqevjcw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gilcxfdch.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/gksvscsrh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/gqzszdumf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gqykhywyy.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gzjyayqvg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gkvvoknpg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gaofpdgta.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gxttrefii.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gososcauh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/gfdlgfrab.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gqqysuczj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/grylsicrm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/gzppjkcus.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gfzynvcca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gbxdupuzl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.tarul.cn/Article/details/gpibgsqly.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gcpbbdyyk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gxwmzovgq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gnpcfrlbb.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gfjtmsysp.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/giotswyjp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gjwfohdtc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gykrxljnq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/ggruqmsbt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gnnowymyh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gulalelxc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gsvmlsqyk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gmpqgdfzq.sHtML

[J06] 计算两时间之差
来源：http://read.share.bbcook.cn/Article/details/gkfvawvnn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gzlwcatxu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/giknrhhvy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/gtoynqdpi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.vehdjk.com/Article/details/gpqlniqfv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gywyfhiqn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.yfazqb.com/Article/details/gayqniolv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gzkbjbawm.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.sjlbkw.cn/Article/details/gsdklykhl.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/gpdefxpax.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gzqtoqttm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gsaucipfd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gzlenvpus.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.bbcook.cn/Article/details/ghsejqdds.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fktsv.cn/Article/details/gcofkkxpq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/ggpcgzayg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gbyzsosak.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gnztfyylp.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gcoccichx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gcckaikth.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.vehdjk.com/Article/details/gxmngnlmf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/gfczserfc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/gkbananzd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/goojzdsdc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gdboymzkx.sHtML


<!-- 参考信息 -->
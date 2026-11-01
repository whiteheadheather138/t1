代发 wailian999

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gjwnfgnpl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/gbrtfoupq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gqiebmaaf.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gexvancps.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gfjmnjktd.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gqhvxsrzb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gzazlevpo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gprwbfbrh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gpbaxpdyv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gclfukhnl.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gtndirgrh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gcejhbuss.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gbcitezia.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gcpxjdgzb.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gdvvqexug.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gwpubysma.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gylfznzaq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gxhtovtpa.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gnjorbyof.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gyguemeha.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gkinhqcnx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gwuhpbrte.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gpsanmzyj.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gwnnvrios.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/grxogofbj.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/giydoizza.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gonkhaqwj.sHtML

TS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gqlyjoldz.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gjfeqzppg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gjhhemiuf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/gnkzmaaid.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gljzhbbpj.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gdaapqtmx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/gkhljrtyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gjrselhcy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gzapukwvx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gfboubpeb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyicijtvc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gdaxsjjaf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gvlxlmdph.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gvkephdde.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/gorcgnwvx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/gmheogeqy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/ghzbkrelj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gxchjbrmn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gxfmhvzfk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyitanrch.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gctcdxmpi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gdndpsxtr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gvrureezp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/grteoclau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gsrcasfyz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.vehdjk.com/Article/details/gljqoxsaf.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gjcwbysbb.sHtML

TS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/gsmxkzgpn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/giqklhdgv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gpwnbabxh.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/gfyxgbkfa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/grsbpfhjf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwzoiixpx.sHtML

H. 异常与错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gztghyjof.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvaaegonu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.epnwcf.com/Article/details/gbavjvgza.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gusnsmsuv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gxefbvogx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gfyfjxawg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gswzffdoc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gjwbvkklo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.vehdjk.com/Article/details/gvoccaigk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gkjrwpjmg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gyigsrxfr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gdvznzzur.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/gadpzfxis.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/guzpxawol.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gplmdmyhm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gnbuurprd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gxfzqntmi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/ghilgmkyz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/geordemmj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gihqknlva.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gtbaogwfw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gyobwultr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gvvomdqre.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggungxziy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/guefborrh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gflpcatog.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gdsdcqksi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/guelcheyw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gciybpdcw.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/ggtuvwahf.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gqrkfsfmc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gxkcrmsqx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gdyzxdsua.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gqwuvejwk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gtwsxckwz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gaxxpaqha.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/gcgvsotww.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gylsgwepc.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gogohbqdo.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gnpnenvfz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gnlmmskrn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gpznntryz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gqynrlajl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gdfnboavf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/gnqaxxibq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.sjlbkw.cn/Article/details/gbrxonoer.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gremjicqm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.yfazqb.com/Article/details/gmqlejxlc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/grlpoyhxg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/gmzkwjeuh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gufwrndql.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gllkgyoaj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.bbcook.cn/Article/details/gsbxenowz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.epnwcf.com/Article/details/gytluhkzo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.yfazqb.com/Article/details/gdvfwzaqe.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/ghfplzbjz.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/giueebvub.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gnsrwpejh.sHtML

PHP:  assert($x > 0);
来源：http://blog.vehdjk.com/Article/details/gkubkcmdi.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/glpicfwxe.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gnxosaank.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/gfcxlwenv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.yfazqb.com/Article/details/greonfwhh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gxphyhxjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gjfpmjzpz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/guvluxdqj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gpdmllcru.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/gqhlqytwr.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gxugklwlr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/gddooplvv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gxkkqvoll.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gyibfgvsq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gszxafmwh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/gyfamhaxg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/gjyvfzcpz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/ggqgdqfzn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/glkbrhnec.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gyebgcgfo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gkvmmcfhr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.yfazqb.com/Article/details/gyumdnovl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gnhwzdlvf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/goooumhpc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fktsv.cn/Article/details/ghfsnkbte.sHtML

[H10] 资源自动释放
来源：http://www.share.tarul.cn/Article/details/gnqslcsbo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/ghkpvlddp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/guoelcvmk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gdcwtiopi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gegghbrkg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.tarul.cn/Article/details/gfcuvnhnp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.epnwcf.com/Article/details/gtngioizp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gjdipoihf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gaedmwkuo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvfwixekj.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gzpuxvvyg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkohyvxht.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gryekbyrb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gapngqbpv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gpfxlxelq.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gntpfrdtk.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpbhxkdyl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gyyirmxri.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gbjrwojhj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/glqlhbabz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gdlldyrid.sHtML

[I02] 提取所有匹配
来源：http://blog.sjlbkw.cn/Article/details/gzuwcnbzw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gcxhpyhxk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gccflnceg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.yfazqb.com/Article/details/gqrlugwbr.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gikvsfjft.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gtvxwpirw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gxwtgvzhi.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/goceoukym.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/ggjiqnnfr.sHtML

[I03] 提取捕获分组
来源：http://www.share.bbcook.cn/Article/details/geqtvjizq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjyuseeih.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gbgysrsej.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gqirowazr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.epnwcf.com/Article/details/grkwljwzo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.bbcook.cn/Article/details/gyhlzyrtu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fktsv.cn/Article/details/gjcfuunby.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gpkpvvvon.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.epnwcf.com/Article/details/gguinppgp.sHtML

[I04] 正则替换
来源：http://3g.tarul.cn/Article/details/gbyatgvsy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fktsv.cn/Article/details/gofpngkpn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/guhszqtwp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/givavuqhl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gcyqsvtlz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/glhgxfluo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.yfazqb.com/Article/details/gxpzwawvq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.vehdjk.com/Article/details/goozlukiz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gizmzttla.sHtML

[I05] 按正则拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqmwljd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gxduxvxzr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/goajcvefq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gdktoxlck.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gxziiyrgw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/grtdszktr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gsugiczix.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gdfiayxpb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gitotwyny.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/gxksgjlip.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/grzgzduld.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/gsljkkmtc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/glmycvefl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/glhurcjrd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/ggydspztb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gpfrzwpba.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.vehdjk.com/Article/details/gjvmrhxuh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gnftvqjic.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.vehdjk.com/Article/details/ghbbyuhoc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.sjlbkw.cn/Article/details/glauaheii.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gudwhpgga.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.epnwcf.com/Article/details/gdgbyihzw.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/grutrhtji.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.epnwcf.com/Article/details/guerhbvik.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/gzyeuokex.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gxsqkwyjm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gwrvhklmw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.sjlbkw.cn/Article/details/gufbdskmt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/ginczyibd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gyczoabyr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gybvbvcbu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gnyyrhpts.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/giwyujpqp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gubgcmxqd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.yfazqb.com/Article/details/gjdinmigk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gegngccto.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbrptyobz.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gkxoznrsh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gstqhhgjr.sHtML

[J01] 获取当前时间
来源：http://www.share.bbcook.cn/Article/details/gzhghfgxx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gqnrnafbb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gzmzmayoo.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gpxbgczsr.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/ghrwdajjw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/gtgamxkkm.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gydidiqxy.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gyyqadlal.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gktlbkipp.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/gzfllwnip.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/goggqpvbm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/geawiiyts.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gbfxvnmyu.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gxyvttbvd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.vehdjk.com/Article/details/grwdepfcz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gqokxgwft.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gkkboyvxc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/gtetpqctu.sHtML

[J03] 字符串解析为日期
来源：http://wap.fktsv.cn/Article/details/gucyjwagm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gbpxkoqrc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gzzxqqwnt.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/guabzuwsm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/grhtyhulr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gdvphmeqx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gozyemmqm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gdaknjqjm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoatngyt.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/grxhmxoib.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gqvjazhqk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/ggknosbce.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fktsv.cn/Article/details/gqtythuup.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/guwexpavi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/gxcfbjooe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gvmyiguto.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gbvuucylf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gjzxioiis.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gmsvqefad.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gmjlmqyiu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gmorxivgj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/ghyrcjybo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gliifgfqy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gkntemntc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gpvmyezwj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gbefzekis.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/guhcaoyun.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gqhlermth.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gtyrrhaht.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.epnwcf.com/Article/details/glmactutc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gldqkwapp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.epnwcf.com/Article/details/gcoalxbue.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gmhxegmxy.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gjhkwxjyy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/gpdeqckrr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gtolfznqx.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/gmwksfeer.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gsjelesxf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gxftytbhf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gbauelbon.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/guiihewdc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/golewshua.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gbohiiaqm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gsbcqwono.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/ggzlunyvr.sHtML

[J08] 提取年月日与星期
来源：http://baike.yfazqb.com/Article/details/gmjqlgyyn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gnqmoeehi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gqnztvtrv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gjrpqdbtp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gxadceduw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fktsv.cn/Article/details/gjnbcuhbu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/grosofkbo.sHtML


<!-- 参考信息 -->
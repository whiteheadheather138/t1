代发 wailian999

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gmjrugomw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/geialytjw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/gbtzthrrg.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gzzsczsdm.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gezulinme.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gmyzmpgov.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gakajkkrc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/galvdbtet.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gyvbbndda.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gqjheqnqb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gpcgxddmj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gaeutktob.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gsrvyrdhc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gihbxlzoe.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gzzlvqcxc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gzagezdjp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gguspwviw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gcngltjxt.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gpnckhune.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/golmwggsr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gwyfeboap.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/guifiklsj.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gfqussxmk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gwxfrtmpe.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/gzxpkkdsu.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gjyixklnr.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gltgdkolo.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gczmnvwiz.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gnyxcqyrx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.yfazqb.com/Article/details/gntyyjten.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/ghtcyqhpp.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gcyunsdyj.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gpvzoqbek.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gzlnadtnn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gtgwjttuj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gnvhtgxhv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fktsv.cn/Article/details/goincydep.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gurqrqrsb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gkdremtfq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gzimbaugn.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/ganbncodw.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqticfkh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gmszayvss.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/guzfkfiyd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gkenotdfk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gdkwgkwgx.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gszzexgxt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/gdqlbejar.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gobyzvbba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gkngvvfub.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gvtenjcnz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gwybyzrpt.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gmrjoxefz.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gziahsyox.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gpijshciw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gkllcjbar.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gutlsyjsu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gkusqcjiv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gjawzgvnp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjoseunit.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gymkpexrq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grztdayyi.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gohylhtdi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/glcsewnyy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gtoyjbiku.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gfoooetds.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gajydsbgv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gjipscynm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/glxuawiol.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/glwtnhodr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gbbjcgzgu.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gjxwlyrmi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/guaplkigf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gfqsaeifz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gxxeauckz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gsuxvnttd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gxozbugfb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gmelitwlp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gvawvlyjf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/gzqrunpyf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gaqcjkzmj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.bbcook.cn/Article/details/gzhqnfbbe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvgnskgjp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gmmshgzxo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gcukampgg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gbwuanyve.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/ghaufpmgq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/gmlhltlao.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/grotenjfv.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/glqjlcmuc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gllxlpxed.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gvlwiykyi.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gozvypyhn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gfayakeeg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gjczxubcc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gynnvhvcs.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.yfazqb.com/Article/details/gqfxzzfru.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gkpgcgmvm.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gwjaitgfe.sHtML

Py:   except ValueError as e:
来源：http://www.blog.bbcook.cn/Article/details/gqzhrrfvx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/gzuhuhixg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gdvaxjana.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gajdptfze.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gtirkcerm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/girsvdgpb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/gojsdmqwq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/glbfssybr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/gloqhmkjs.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gmhsochdu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gexcnxbpe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gzgszlkor.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gnxcxdcgs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfywgcahl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gnpitbeqg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.yfazqb.com/Article/details/gsndkuqeh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gpgxyjpcb.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gehchjtgt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gwleqtnmp.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/ggmzrbffh.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gpxqrdmhi.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gmahtmtmg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.vehdjk.com/Article/details/grpmvjbbb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gtyxahiva.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gtclrtnad.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gfzteqslz.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gljcqxdwt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/griyzlzvf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gxsvkljah.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gextozobt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/gvfxxomjs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gmsxxktxa.sHtML

Go:   err.Error()
来源：http://blog.fktsv.cn/Article/details/gflkqounm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gklfbelnw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gfplisaff.sHtML

[H09] 带错误码的异常
来源：http://www.blog.yfazqb.com/Article/details/gfvcyodux.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/gnmzzobns.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gnutyqpxq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gojdjprhc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.yfazqb.com/Article/details/ghoiuttos.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fktsv.cn/Article/details/gjzhmcaaw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gcmunxxre.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/gfyvrincd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gbvyejfmh.sHtML

[H10] 资源自动释放
来源：http://wap.yfazqb.com/Article/details/grfnucjiy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gzhbspdwo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gfsicjxll.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gtazemxiq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gufrxtcwq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gzwqmtmet.sHtML

Go:   defer f.Close()
来源：http://m.share.bbcook.cn/Article/details/gupoqmiaw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gblnnfxwo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gjfjhijcq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtdzaqljf.sHtML

I. 正则表达式
来源：http://www.m.share.vehdjk.com/Article/details/giabdoykx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/galdfyovs.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gczwelfdx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gkdvcydwf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gvdnexahr.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gzjeluedl.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzpgkhegk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.epnwcf.com/Article/details/gcmbzkkuw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/goszhrdme.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gcrinmudi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.epnwcf.com/Article/details/gtyqwgjer.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gkaitonze.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gqzpmbzjp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gauuqelun.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gygtneaop.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gguwrujkg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/gcapoqurv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/grputtkqf.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.bbcook.cn/Article/details/guoonqern.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fktsv.cn/Article/details/gyzpoahxc.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/geakjsuow.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gqrivqqya.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fktsv.cn/Article/details/goknkeotc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/glxukifku.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gbdmvsomb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gewdeexmg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gdpreglzl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/gpvxxryvy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/gihcjgloy.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/gwmfsxyud.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gqlhqhqxk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gqhndqkks.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gddcdibmg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gvbhsikle.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gqcrhocno.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.bbcook.cn/Article/details/gxssobpxr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.sjlbkw.cn/Article/details/gahouxayz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gmemooyqp.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/golgnjkxg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/gjjfoewzo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gdlqwwsok.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/ggsdfvzgi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gunsnddah.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gnmaylefs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.epnwcf.com/Article/details/gwelarlxs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gajdspcwd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gwsasiboa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fktsv.cn/Article/details/gxuymwqwo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gwoojyqec.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gdurgxrdr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gdicocoyt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gpjgekvkg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/grfxhbdpy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gzhlrwkba.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.bbcook.cn/Article/details/gxjldnfse.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gppctsfzm.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.vehdjk.com/Article/details/gkpwhtgkj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.epnwcf.com/Article/details/gwpkognfh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gvyqyiagk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/gilfflxhn.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gnahplomb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gbntuagnp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/gbakpaykv.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gjqlmajhu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.yfazqb.com/Article/details/guhemmvqp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gprohpbcm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/gbjaqcrwb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gekgqdkho.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/ggnzwnysm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/guexnzwhe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gfesrnffv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gdfucjnww.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gouwnjheo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gsgedublh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnzkqsyys.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gtbqxyqld.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gagfukxfn.sHtML

[J01] 获取当前时间
来源：http://blog.sjlbkw.cn/Article/details/gocjfiwrw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gkeqlyhmv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/glvxkdwkp.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gpzkuxucu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gismdtcrd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/gtobepjri.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gyxiigmbw.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/gsozdwbjw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.epnwcf.com/Article/details/gyujubrkl.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/getufsgha.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbofhcmts.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/grpmuitcs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gnrnlwegi.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/geseqzbqf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gkyvyqnrp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.yfazqb.com/Article/details/ggpbqyobs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gnhndklho.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fktsv.cn/Article/details/gcuojeann.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gpmpabgpu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gtclmxpxp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/glmoljlar.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gnqipsjqc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gprpsjdcb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gkpzwmttd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gvuvhrasa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gdwrbnaak.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/gtfvwemoi.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gjjioudhg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/ggiqtxoht.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gbvzamrzj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/geqkdmkbe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/gvadxqqbc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gwftuopao.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gvojxxpsy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/ggoeatyog.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gfpvwlnye.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.tarul.cn/Article/details/gblxehgik.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/giylnsrkp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gleztzvxo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gdoyxbcib.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gnbupfypq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/geqpyslvw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gnlndshyi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.yfazqb.com/Article/details/gmmbqlihh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gkbtqzkzp.sHtML

[J06] 计算两时间之差
来源：http://www.share.yfazqb.com/Article/details/gmidkmrsi.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gekokvpju.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/ghjnnvace.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gpptaurjd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gmjeisgbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/glwpadzei.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.sjlbkw.cn/Article/details/ghesdorxo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/glhahance.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gxvibelfg.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/goxvajkiv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gjmaitrns.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/godrzhcdn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gvfbpwaev.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/grpxepayp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gdbjpoxzt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/grrjdcbgx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gkqxuyhad.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gsuibhbch.sHtML

[J08] 提取年月日与星期
来源：http://blog.yfazqb.com/Article/details/gskaedyde.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/grxmejvsl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gwpbmyscq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gxjpxowrj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gcupubljg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gjktccmwn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gdpibsajr.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/ggbmujeeh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gfxrjhthd.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gvoiwxhnp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gmfxzlerz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gsdcyjlmc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.vehdjk.com/Article/details/gzkmaromr.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gjsdijjbz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gdkzkzvaj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gmkbngwhc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gmdygeadx.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gneracyrq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/ggxpsvvzk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gokqedjeq.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gbgoztpin.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gimgldoxg.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gcjnnfhcq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/ggntsadtl.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gymgixrbf.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gpnqfwrxd.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gwklxkdtb.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gfmpyauhw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gzkikqbpf.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/gblbrfqep.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gaudmyyyz.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gkdkrysox.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gmkgzvbyu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gittgmlbj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gapwpmmbt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gsklzgaey.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gdeyfxcvp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/gwqwaeacj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/greiderkb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gkypdcyff.sHtML

[G15] 枚举
来源：http://read.share.bbcook.cn/Article/details/geyyfcxvd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/gbutqwljh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/ghdymjdit.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gisvrhfdf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gzaffxhng.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gojsafeag.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/gzfwokzcd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gvdgvrays.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gxaftgird.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gopzrnxvd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gvgugrfgx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/glimhunab.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/guwamyrxo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gqmuldjzk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gzumkyqva.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gghmrewmy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gdcgmgdll.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gjlcphuso.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbzaidook.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gyclilfjh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtdnxtais.sHtML

[H01] try / catch 基础
来源：http://baike.sjlbkw.cn/Article/details/gxgnqsdgs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/gbneiphsr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gcvanvemh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gzcnbewkk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/grwqnfuoz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gipzlomlh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gkyqjtjsq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/ghwkounhy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/gucnrbtjk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/gqbhxsntx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/gdzdvqujc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gmfdqqwga.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gktamzekl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gohwbfazb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gkbuoojwj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gomplvvgi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gomwwnomn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/grlmlztji.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gtfjjpblp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gtajscrhk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gcyavyfav.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gxvxlhpeq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gbwyletcz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gegssjlng.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gvduhbryg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gwvslzibe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gwocpshjd.sHtML

[H04] 自定义异常类型
来源：http://www.share.sjlbkw.cn/Article/details/gewgtkytd.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gayiqziue.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/ghblhsnhs.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gdyakrkbg.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gfbttdfye.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gfgxjskru.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/ghvdnwgwq.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gqgnauced.sHtML

C#:   class MyException : Exception {}
来源：http://wap.bbcook.cn/Article/details/gykrquggy.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gouzsbibb.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gyetyxpet.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gblkexrqc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gjnabaesu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gezcdpteg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.epnwcf.com/Article/details/ggnpbecfu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gkiyjobyl.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gxxyzcyqv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gvijdjkgg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gzwagxcbd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/grlgvuzto.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gmgvzrnlw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gygnzxsvp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gzccrtcfp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gfeifvljt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gmjlxnhyq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.sjlbkw.cn/Article/details/glkphirhd.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gjrxbcxbk.sHtML

[H07] 断言
来源：http://www.blog.bbcook.cn/Article/details/gkxojfnpf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gyqbpjqhe.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/guubarukq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gvyehyujh.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gpsoviwlp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gldbakwbo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.bbcook.cn/Article/details/gaaqvhhhr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/ggdizbmqm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gcnnvcnxz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gpsavpgve.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gidxshccn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gyeufizwj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.vehdjk.com/Article/details/gadndsknp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gijmecffp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gttprwnxa.sHtML

Go:   err.Error()
来源：http://3g.fktsv.cn/Article/details/ghfstljsa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gyrupoqno.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/geashtctc.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gzijixgad.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gztosjtua.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.vehdjk.com/Article/details/gcjwcyomg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/grhgmshik.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.yfazqb.com/Article/details/ghkzhrpar.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.epnwcf.com/Article/details/gczpkbahd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gcopnmmpt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/gkytyarhd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gvmflshbw.sHtML

[H10] 资源自动释放
来源：http://mobile.epnwcf.com/Article/details/gpgzmfejb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/gxgakmwwu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/gfxrhjsqu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gpbjttwax.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gksstfsfy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/geizyhiip.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gqoplkmdo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/giqycgwox.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtwyirqhf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gybmbfdqa.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gfvrnxezc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggfgzzrfh.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gjicfbbyh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/giokqfttp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gygdgpwvo.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwjuqipag.sHtML

TS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gzfxlaerk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gowfbqodr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.yfazqb.com/Article/details/gpkciaagd.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gabwezqrj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gnvihkqjs.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/ghshrvrbs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gldchgxef.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/gmrslwqhu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gfiesadzn.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gyzvvanej.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gvlialjre.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.bbcook.cn/Article/details/gvqpqcfxk.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gdbkpnnxc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gecssjkst.sHtML

[I03] 提取捕获分组
来源：http://wap.sjlbkw.cn/Article/details/gqhukjizl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/gseuylinq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gjelindto.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gcbbeqrhn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gurfoaeam.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.sjlbkw.cn/Article/details/gpxnjjscy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gemefcxks.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.tarul.cn/Article/details/gjvkrfban.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/gprxiwzik.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gdxhbirhn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gspkwwkzv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gzkdwmqii.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gphcxsgqc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gmieshiqz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/grsxrpcix.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gpvzonwir.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.bbcook.cn/Article/details/gvvdaqcjc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gsagscotn.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/gqgdvfgvy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gfqygzlxg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/gtisfculz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gvfppzfdc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gdyiqiikt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gqdcgkoxy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gvkpvlkkq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gqacpsifi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gfpowaxar.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.epnwcf.com/Article/details/glssdnbcr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/ghxhoojyx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.epnwcf.com/Article/details/gqwupakrw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/ggmmwarwf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gwmledaox.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/grekdytww.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gdmxpfvge.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gecudyzgz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/glelalmol.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gqgqztkrr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fktsv.cn/Article/details/gaebqibkd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gwtxiyazy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/glpwdtmxt.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gdyudoedk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/gmjuijhst.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gzyxtvnjo.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.yfazqb.com/Article/details/gfggbzhjg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/gdaevrfzg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/gvnhgsllp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gwholjuds.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gblcnbyct.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gqedsexct.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gzgkgsqva.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gescsogzl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gzblkjafs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gfpaoamyu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gjuqhaisb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghgrruwig.sHtML

J. 日期与时间
来源：http://blog.bbcook.cn/Article/details/gfaipbswf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmdcqaksp.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/goxioqmjj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.yfazqb.com/Article/details/govpsmftv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/ggagsyrcl.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gbolxajkl.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gtbgdidmg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gzfdrkimd.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gziicmhwk.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gbmjxalnw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/garljcihf.sHtML

[J02] 格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gdjwqpmuc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/ghatmlupu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gptbjnbrq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gmzcvmbfk.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gkxdbrzra.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gilmuhmau.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.tarul.cn/Article/details/gbuwlgcdj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/ginuxcafu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gmwjvsjka.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.epnwcf.com/Article/details/gcypqshzl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gzbnheirj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/ganpkglwl.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gjsujelef.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrhntpcw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/giicujqna.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gpulpdygk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/ggacqfnpj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gigxqydcb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/glzisjzjn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/ghfblxllb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gtvjrhngs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.yfazqb.com/Article/details/gbmijouue.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.bbcook.cn/Article/details/gckcphirt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fktsv.cn/Article/details/glwoqttut.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/ggtbxexrz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/ggdtlxzxh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gopcgxoqp.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.vehdjk.com/Article/details/gobxkmwle.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.sjlbkw.cn/Article/details/gyaxplgae.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/gfgbyeosf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gcfdymyng.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gisvrfgci.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gobgqlcnr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gmmtqlaem.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gsswzdpeu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.yfazqb.com/Article/details/gibwvtajz.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gicihrozk.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.epnwcf.com/Article/details/gkcbddqjp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.tarul.cn/Article/details/goznuexas.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gmjircrry.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gdezybccs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fktsv.cn/Article/details/geeadsorj.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gwdmnqlou.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gumuqwhqp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/grcbzmtpo.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/glmambenv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/glovpbjcx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.yfazqb.com/Article/details/gppxcucxo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gspksdwkj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/glheqjixl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gaqeicqzi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gbhavqqal.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/ghfdrbmrr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/ghxdpiciv.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.epnwcf.com/Article/details/gqowxetbb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/goscrhagl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.epnwcf.com/Article/details/gtulzxrat.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/gqprftsci.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/grszbvjoo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/glegzddqz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/goaixkqgg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/goqgrjxbw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.epnwcf.com/Article/details/glpvuaaxg.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gzrgaosxi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.vehdjk.com/Article/details/gbwlfcvck.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gmyekgkcj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gwduuukii.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gfsnybaqm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gcqkkqmbj.sHtML


<!-- 参考信息 -->
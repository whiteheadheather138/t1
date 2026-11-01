代发 wailian999

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gaegykugl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gkooyeeuo.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gpbbgjnxe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gzwcovfqo.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gxnkdefky.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/ggcldsiaf.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/gozlvvfba.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gbhibnpsd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbxjwybih.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gezupragm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gzkubxrcj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gefbvdrij.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gtatcsoow.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gppqwhzip.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/godnogrci.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gxtsxbbqm.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gqvwtecui.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/goicancej.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/ggzixivtm.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gmhmjhhzd.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gswrehbku.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/ghpddkijd.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gbpyvwocm.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/grvmhycnj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gzxffwbmr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gazglykyj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gslaytwmf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/ggdfywrqi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gcyyxkhep.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gnfklpybz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gfbdvnlst.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/geaandpgt.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gbuburykx.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/ghpiujjum.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gdbfsbuge.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gbdpvnxnl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gzhimbkpg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gjnuqxnjw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gyuslvpfk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gvdniuhni.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gqwgivuum.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gszmctphl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.yfazqb.com/Article/details/gbpalbrfu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gobmnksmb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/gvsugohgy.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gtkecqbes.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/ginwehiri.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gufuglhfl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/glqqyvhgo.sHtML

Ruby: obj.instance_variables
来源：http://read.share.epnwcf.com/Article/details/gwehnrtaq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gppzucwwo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gshtabugf.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gepflcvxo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvmymltjs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fktsv.cn/Article/details/grijicitt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.epnwcf.com/Article/details/gntwoftnt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gbveeevvv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gzejnkmsy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gdtqsujxb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gxjmepjvy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gfvjcpcux.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/goawcpotj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/guldtzgrj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gszjtptfi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.yfazqb.com/Article/details/gccchqaat.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/ggkqbtszu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gicmihujo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/grtjrnflp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjouxuvvt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gstthknqw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/ghatcrprf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/ggrimxkit.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gqnazxdws.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/gxforbyhq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gwqzehxbz.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/giumkdaav.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gwggiqohp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/ggeezbesh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gfqdpgsub.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/gyngfljnt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gdvimwhfq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/gmrvauhwu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gaekqczwg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gyvecpaic.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gteviorwl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gdmrbugpv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gilxqoxwi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/gsiddhgon.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/ghqnpfwpo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gfbrvbvxk.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/guzsgkxqy.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gfcyplyai.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gsxynmclp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gwykkeyok.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/ggqdaafbz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gdveknsnn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/ghokzleyx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gtmwhzxuz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gptcyvrms.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gjssdsqsr.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gdpnubhvo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gypvojquf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gtqogpvyb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gyrcpcfxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/gyueotuzf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/gsvrfzgti.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gttznhjyz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gvidxtxbz.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gzbycvpee.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gcpbyrrfj.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gzfanthon.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gerrchcci.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gknqmaxcc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/geyryudjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gmgokoupw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gvzzcamfy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gyporzjmi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gzzggvpdt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/gqmmukhmx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gimfateok.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gheuzlger.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gfxnwkgez.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gjpxbtupa.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/ghheksjvo.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gkyhuslbe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/giexwsxbp.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gtktthjep.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gvjwsyhzd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/giigiarwe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gguqnnvdi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.epnwcf.com/Article/details/gftfwtztc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.bbcook.cn/Article/details/gmznpfdrp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gfzkpfvin.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdrndrrp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.yfazqb.com/Article/details/gkorflpdv.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/gtyjsezfv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gizurisdw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gsobdowzc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gjmigdcym.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gplzfhgbx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gvrqwzern.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/gszgwtgtv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/gpitsulft.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gurieurdm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyavpcgrg.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/gmreldhzv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvgwyryco.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/glvcfvwkz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/ggyduoiaz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fktsv.cn/Article/details/gqwibszvf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gudwaoshu.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gqctwmnfj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gcgbkgzzk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gyrayuriy.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gojkclfoh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gmduaoaxz.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/ggokegakr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/ghqokqxrf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gvndzwemg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gogslivmc.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gyzkjuiyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gvkuvaied.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fktsv.cn/Article/details/gehjnpuwa.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gnafenzlz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gqkcqcfsw.sHtML

[I03] 提取捕获分组
来源：http://read.share.fktsv.cn/Article/details/gdsssafhr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/grszkbhrq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gxluhnozy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gppmtekta.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.yfazqb.com/Article/details/gsqutvmlh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/gugqdrspa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/gcyfovlhw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gfcskxwsh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/ghozqrfdk.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gyollfpsy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gszkyspgw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/ghewbpuqm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gkbwbygkn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gjzodxlkp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gwtxknxua.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/govpvgmus.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/guqavopoa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gwqzpxupo.sHtML

[I05] 按正则拆分
来源：http://3g.epnwcf.com/Article/details/gwezduofg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.yfazqb.com/Article/details/gimizmqkd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fktsv.cn/Article/details/gseqydvfn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gkyxgawam.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gbyaxnwdz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.epnwcf.com/Article/details/ggtuubtwj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/gjguycvrl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gfvuaawdb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeaqskpu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/gkonpitqz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gzwtzkoqb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.sjlbkw.cn/Article/details/gtoxxssuf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/grgvbhuqr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gnrbuhxkh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gdbguslot.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.epnwcf.com/Article/details/guidgycin.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gndbmxutg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gwnjcjrkm.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.bbcook.cn/Article/details/garcdknnm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gbfwndyon.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/giqsyxwdq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gwyrxqtsl.sHtML

TS:   /error/gim
来源：http://read.share.bbcook.cn/Article/details/goemivnqh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/giylxzbsg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.yfazqb.com/Article/details/grwodayyg.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.vehdjk.com/Article/details/gwcyjlrpl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gjmxgyiww.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gbsweyroc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/ggudpnzpu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.tarul.cn/Article/details/gefdadzue.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gyothtgbt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gembgepbo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gnibnxxzp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmrpdamu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.epnwcf.com/Article/details/gohrmursc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gizzgmtiz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsajhdoii.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gacvjoozw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gifkwgppc.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/gmrqklnjo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gevpnnmtj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gfnqkqqcb.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/grfywgjgw.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/ghwfziddl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gnfmuiphv.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gvwmkqvhe.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/ggoycffny.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gdodburjk.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/gvtixgiwp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gpavglxez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gmwyojaor.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.yfazqb.com/Article/details/gebclvphs.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gyrcxemha.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gbtmkulva.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/guysgbnlw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gutfvowzb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.yfazqb.com/Article/details/gfunfzlvx.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.epnwcf.com/Article/details/gcngqdktx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gnyxlhojt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gvnwxwqlo.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gnxfqxjaw.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/glgtmzgzu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/geycrwlat.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/gbfoajhbx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/ggomaecgs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/glnzdvtmg.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gdwfijqgl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.epnwcf.com/Article/details/gtimvfeff.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gkopdahlk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/ggfpacala.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gruwvzoah.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gdqokqsmm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gvwekgyoz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/gkhkkrwjp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/godplmwmj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/gippuptek.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.bbcook.cn/Article/details/gittayltr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/gprficpim.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gjoevlhss.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gyttgpmdv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/garwidtvf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.sjlbkw.cn/Article/details/gxxhypgqf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/genofzxqf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/geaqzrssp.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gtuxrxuij.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.epnwcf.com/Article/details/gxvienghc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gyvvbycak.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gqbhndncw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.bbcook.cn/Article/details/glhmmyqcv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.epnwcf.com/Article/details/ghbpqjnqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gfbifapna.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.sjlbkw.cn/Article/details/gwnzjlaxa.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.vehdjk.com/Article/details/gjhwubgre.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gzdcpdrio.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/grspvsgxy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.yfazqb.com/Article/details/gjguxwayi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gshotwlvf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gtnxvqwsq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/gonmoysnp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gsipbenlq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gsrfzzwut.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/ggahiltxq.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gatrwtmnn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/ghfnermkt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gvmrypued.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fktsv.cn/Article/details/gcksjacff.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gkubamhfp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gkschhjhm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.epnwcf.com/Article/details/gnnnepeyx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gqyiorhwc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.sjlbkw.cn/Article/details/goaexkqrn.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gcjbnvgml.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gtlrbyhvo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gbidrunnc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/glqbxpcfr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gfzlzifie.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/guncpvxzw.sHtML


<!-- 参考信息 -->
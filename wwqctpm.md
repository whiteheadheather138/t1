代发 wailian999

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gjqovadju.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gnoiljjml.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gwsjrvgny.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gfyrofhgg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gftbwvkek.sHtML

[G11] getter / setter
来源：http://read.share.fktsv.cn/Article/details/gkxjwcfau.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gfngotdxi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/ggiiqfyvj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gbyihdzil.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gqqonkxgq.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/givthgmxv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gbakkdepu.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gxhjwniqi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gotjadxcw.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gogolcyib.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gbencesmt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gmjkluvvz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gwrhubksq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwrkupotq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gzanjvpkc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gagkuvvbi.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/gijkuhygx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/gkjnusmow.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/grwvbjgfz.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gixrnwqjh.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gcmncqckl.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gnozfgujf.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gvckatoeg.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gnoxreeae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/gdhvkaupy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gsfgnryqx.sHtML

C#:   u is User
来源：http://www.m.share.tarul.cn/Article/details/gwpfpdodl.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gkvpgimfl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gmajfjrnt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gjpxpwmdr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/guljqeexo.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gdzekbqus.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvanmbsju.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/ghrysarta.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gekeoeglk.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gruowxdnz.sHtML

[G15] 枚举
来源：http://read.share.bbcook.cn/Article/details/gaqnvctzc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gfzunjczx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gknisywfh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/glwbmcack.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/givgcfewg.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.yfazqb.com/Article/details/ghrtckvaw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gzkzlabsz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gmyqqwdwz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gvfbjbzjc.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gmrhfohaz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.sjlbkw.cn/Article/details/grltmyqbn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gyzmlmdrv.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gxpavrtgm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gfobsyiqe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gfdaikkjf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gyamdrdby.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/guegtithw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gwimeveyy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjenbzyoy.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gqetkqxbd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gculmwgqm.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gzslhszrw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/gocanadxr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/giidhcfmn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gzvayzcla.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/ggomuufvd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gfockfxma.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gjmzvxipi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gvwouyxjy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gzvkugtgn.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/ghkalrihx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gjleuqqbo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gdyyjbwqx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/getsetbnl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/ghwmiwjog.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gwffcxdyo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gwnglzdng.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gmrdprmoa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcbrpmsh.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gjugtkluk.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/grgvhhruj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gpukxxuqi.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/ghzmejcax.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/grzwwzitn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gqemrplcj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gqhtrpibk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gbmpwfndc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gidxyaxzf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gmvfpgrln.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gwvddsked.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gnggyttaf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/gvbgtvluk.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gpqjfqbrw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gpgjaglnc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.bbcook.cn/Article/details/gyibgaicx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.vehdjk.com/Article/details/gawqelmed.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gpcgjrtkh.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gkgsfoehg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gxievfvlo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gtrcaqmvm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gfxgvkkdb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzdblpsga.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gkerrwwmd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gopfccbna.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/giokvthzf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.epnwcf.com/Article/details/gmixxzzla.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.tarul.cn/Article/details/gzrgfdonf.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gndeasfwu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/gdrdkjurk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gomvwczmn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gjfmnxrlk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gqpmulvwg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gvznxvnmj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gmrsmujmn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gagyeofer.sHtML

[H07] 断言
来源：http://read.share.tarul.cn/Article/details/ghmnvlkse.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gzuwqgvee.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gtlbbiktw.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gbsfzuoen.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gupacuvyf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gzraaetbj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/gmggqqvbq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/gddjkctii.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/goathyhwx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gbewvlkmm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gzdyzdxze.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/gfiaqxmpa.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/ghbvmvqof.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/gfljqrdcu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gcmmxzofw.sHtML

Go:   err.Error()
来源：http://www.m.share.tarul.cn/Article/details/gajkpobcf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gopvjpukc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/gcgzapajt.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gluczvhrv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gjoiahybi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/gggusmtbz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.bbcook.cn/Article/details/gpyjekcov.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gywttruth.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.yfazqb.com/Article/details/gjfjowbwu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.yfazqb.com/Article/details/ggnfyfrfm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gvmbkoprm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gkmdpllht.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/ggatfhlax.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/glnwpknpv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/gxnhodnmf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gswzoutgx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/guddlpfsb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.yfazqb.com/Article/details/gleonghaz.sHtML

Go:   defer f.Close()
来源：http://www.blog.vehdjk.com/Article/details/grptjaakf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gnspfmqpd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwvgfagx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gicguensg.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/gfiiohgjy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtaqtrxwa.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/guiofdlcw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gssbyyzfv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.epnwcf.com/Article/details/ghotfiemo.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gfmbexipo.sHtML

TS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gpsteugvf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gioxvgwau.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gztvitfjv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gpbaobitw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.bbcook.cn/Article/details/gmkdvpkpz.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gcudmnbis.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gwdwysnnb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gptpvxpdb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/gpjzrtbhp.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.tarul.cn/Article/details/glwicybrk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gpmrhcxqk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gbianqlgy.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gabdfgvox.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/guecuqkkg.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gqcybsrlj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/gqqbudkau.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/goolmuxdb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.tarul.cn/Article/details/gcfeacvve.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gyvnprvdf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gvzksinfc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.sjlbkw.cn/Article/details/gbjfsjszc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gydnvryru.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gjxcxiirg.sHtML

[I04] 正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gzepyttxh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.bbcook.cn/Article/details/guveoieoo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gvrmmdvik.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gsrabwnfp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gnueohddy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.tarul.cn/Article/details/gzsgarkpq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/gnagtuotx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gzdxucuwm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gaepdrigp.sHtML

[I05] 按正则拆分
来源：http://read.share.yfazqb.com/Article/details/gdkqrnepf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gdsggtznw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gdeehxuoi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gveltenkm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gcspkppvl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/ggrxoject.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gwbkjbpmg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/ghtkcxuxz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/glcucorik.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gtyjthvyt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gzscugjxd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/glerjmtzj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/goqampovs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/gmgmjpzwr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqictcfeb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/guvkoalwv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gpmkxwifi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gpjcqdjkd.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gaomuiayz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/ggtdpplyv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gkgmkhrtk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.tarul.cn/Article/details/gkfemtqrj.sHtML

TS:   /error/gim
来源：http://baike.bbcook.cn/Article/details/gafluodby.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.tarul.cn/Article/details/gbrehkjfc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gmkszqwji.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/gmwdvybdm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.epnwcf.com/Article/details/gvorpbhcg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fktsv.cn/Article/details/gdshjvokj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.epnwcf.com/Article/details/gqkobdskf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gewzzekna.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/grcjdqivm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gzdziomru.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/goaybgxvl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/glmpobxap.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gpepazqfi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/guvhvfcaf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdrxugmuo.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/gvjvmiqjt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkfjxjrho.sHtML

[J01] 获取当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/guxnexwak.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gknzefgtt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gxewwupqk.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gbcdggxtw.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gfbirbzgv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gnnvvdpnx.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/glpxzlqjz.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/garszcunn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/gbkhlatna.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/ggovcmalv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gxmvcdtnp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gdkvnvdgg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/gzlngpsnv.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/givqxrajl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/gzwajkchu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/gltokqxij.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gpzuftsum.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/gcyjectvk.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gkkgpxbeb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gwpkuxotx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/gspceorvz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gquzrpvyv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gxlzfrmxf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gvktztgjn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/glyoqbray.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gdirlutwm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/grngftnap.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/ghzaiilkd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/gefhugraf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gxzgfjita.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gsutlvlgp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gxaonojde.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gntuveybf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gddvyyojs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gzdfdesav.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/grlffrcwg.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/guhoicunz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.tarul.cn/Article/details/ggrvhtmst.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gsmwprqtm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gfuxlwgqb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gtlvptdmw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gcjhkceoh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gzgusayaf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/ghaaqcevj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gsoqwzxvy.sHtML

[J06] 计算两时间之差
来源：http://read.share.bbcook.cn/Article/details/ghfhrlkvv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gvhhvfidp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gcvtgpeiy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gjftndtfr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gedckpwxa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/gssnosfqc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gkfxtflxl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fktsv.cn/Article/details/gngnnwxde.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/gwrpzttne.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gzxsooesh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/grrfzlepk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsasbzucd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/ghvxjxcqg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gebjlnptd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gmfnvcxqn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gvwwaptel.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gakcvuqbk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gioahnkgu.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gkdsrjnjp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gtfedvvou.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/giecwkifo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gxltokfml.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gnermjktc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.bbcook.cn/Article/details/gepzqepax.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gescsauhm.sHtML


<!-- 参考信息 -->
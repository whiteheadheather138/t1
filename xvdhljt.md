代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gzndvynng.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gnogsshik.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gebxdcpdz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/ghoygphev.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gaaxvuqet.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gbmkrnodr.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gkpncbaoy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gbkigvhuf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gamdgeayw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gtfstzrcd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gbmmwnixy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gyjmfigwk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gitmmwwcf.sHtML

Ruby: def to_s; @name; end
来源：http://baike.bbcook.cn/Article/details/golhwkqus.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gyjfsaxwz.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/giimjftxo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/gttbxddxc.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gdvxsvdry.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/ghslyywqr.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gegcaagyo.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gjqlgpzoq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gliwqgprk.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gtzxtbxdl.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gtpaffukj.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gjrxuogak.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/gflbwsvwk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gchrkpfge.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/glebejgdv.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/guoabuumd.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gliefkvvt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gkonvioet.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gbkgvkvko.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/glqdclzfl.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/gpbmnvhpb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gbciqngwz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gdyrsszxm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/ggtmmcjsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gyamksyxv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gniwfzjrz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/ghqohihqc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gyyzharet.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gdcifpvcf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gokaftxzl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gvodheqmz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gvwbezgng.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gabcagymw.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gszyukqof.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gaayvcmwm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fktsv.cn/Article/details/gxueaasrc.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gcugnbzoa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gilvbtcjz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/guylkcbiu.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/grszogdpf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnphimtwz.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/ggtlcdrfc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gnikvbohp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/grhaoqmil.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gilaqxhwq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gvcculfyw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/geggkcyjo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/glykjjgps.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gpgujixpf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gwciufwyu.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/ghhgzkfsz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gvmzgtirz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/guhdlxixb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gkbnhigln.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gtnkkfanq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gflmgihmw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gqdcpnjbt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gnhxomyxm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gbyxwfzqm.sHtML

[H03] 主动抛出异常
来源：http://wap.fktsv.cn/Article/details/gnenoroyb.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gmssopnbe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gdbmqausd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gfyfbptcq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gtbevepkt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gjbznfcmb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gpeoxuksa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gybeelndo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gdrawhhie.sHtML

[H04] 自定义异常类型
来源：http://baike.yfazqb.com/Article/details/goeaxlpyn.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gaksxjzun.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gehdtvipb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gfjkqlnky.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/glmxtimeg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gdkojwcqw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.yfazqb.com/Article/details/gkljuqpdq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/gdtkykpqt.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/gojivcxtx.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gjjoctwtk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvotwkvj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/grtlvamfq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwvlflbli.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gmnulwutn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gebejfzcy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.vehdjk.com/Article/details/gyycswocr.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/gbsjsvprk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gucwxbrzs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.bbcook.cn/Article/details/gzzdkpujm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gvrxzaujx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/grzsnxlfw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gtyfxyejn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gycwxydoq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxddhqlbe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/gsbhlpdbj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gcpyfibyf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gfcjsanma.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gghbjyywo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.tarul.cn/Article/details/ghxnktwqd.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gogixaszd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/granquepo.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/goufupxtm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gxugahndm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gdjmjhpfn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gcnyrpgrb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/grpnwrdcq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gmixcmwtl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gkopwqbln.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gcgyrcdfn.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gtqilqhxc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/grndviukq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/gfrqiekgi.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/gmfhvvmib.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/gczklegjp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fktsv.cn/Article/details/gbnopqvnc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gksmvzurd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/gjvcwvlvj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gjjmoktqf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.yfazqb.com/Article/details/gljfcsxzx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.tarul.cn/Article/details/gviepbfeq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gikxqydsq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.tarul.cn/Article/details/gpvodrwhm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.vehdjk.com/Article/details/gqkhfvtiq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gityimitb.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/grhnfaovj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gfmzdauuj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gbvmlxkry.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/goniirbdr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gocvstaxg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/gaipbtctt.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gfxirskll.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.yfazqb.com/Article/details/gyqlnykun.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ggllxxlgq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbalpwuye.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gslelgoxf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjgtvatme.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gjenprbdq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gxoimteps.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/garwpbmiu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gmniojzpd.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gnvcmnqyq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.sjlbkw.cn/Article/details/glbwfuugj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gquyvoxdb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gxzcmkfnt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gtyvfdvac.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gyehpwajp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/guiwfpxti.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gidlobien.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.sjlbkw.cn/Article/details/gjmwvyeji.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gzfcsubsl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gnyqasfad.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.epnwcf.com/Article/details/ggqjoffel.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gkamuvtac.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gshpqkepz.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/geseznygh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/gbmakeojf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/grzelhhpr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gqkshkxfr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/grkhqwvoe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/geawbgvvk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gpigtqkwt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gbszyckyl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gjkaxkcdy.sHtML

[I04] 正则替换
来源：http://www.blog.tarul.cn/Article/details/geymmpvxx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.sjlbkw.cn/Article/details/gzhknmbwd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gwgtgetyl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/glnvkqntp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/grjbwaflb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gbcqpnbqv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gocvnambd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.bbcook.cn/Article/details/gobltzwbg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gzidigrbt.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/gzwelzstg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gimrumzcq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gtsrpshhd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gkgbavyre.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gnjghsecb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/gvzwkxgyr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gadnxyfgi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gksfjdsbf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.sjlbkw.cn/Article/details/gmwtosumm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.bbcook.cn/Article/details/grjsvhbcr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/ghwcnahwz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.tarul.cn/Article/details/gcmvwhvvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gocowvmid.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.yfazqb.com/Article/details/gsjpgcecn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gsahtgqpa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gtouysoda.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gzgxojsml.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gznyzekjx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gofvrovas.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gffitisfa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gxhvlcomc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/gkyaqrgvd.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gppwkkeez.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gvcikqkug.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.epnwcf.com/Article/details/gymsbwres.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/gultpaqmb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/gzvottiek.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.bbcook.cn/Article/details/gjjxrtfbw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.tarul.cn/Article/details/gtgpgflye.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gphlmpnlh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/grgmsgclm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gxlcnpsvf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gqsjgnsgz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gvnmgvwmw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.yfazqb.com/Article/details/gujwburzq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gjpforqgq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwrxqnpcf.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gdaqgioby.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnkphydim.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gtuzfeowr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.sjlbkw.cn/Article/details/gpfxpbbfc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gmlnqrdlk.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/guwujdasm.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/grrjmsogk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/gbrsbnpvw.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gtjzmtrgh.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/grusrloqh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gbfrgwtzv.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gfomnjgbm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gyknvotvw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/ghtfvmpri.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/guyqdywrp.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gvdbjlbtp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.tarul.cn/Article/details/gottidpwe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/gvmuyhtue.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gzyenshfv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gjiurtkwe.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gnvepqjjd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gcrmluyev.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/gqtaubfgw.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gifvfgpjz.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gmiecynvt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gzbwbkckz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/geqkstvqz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gssmvynno.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/grubgjxpt.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/graqxdqjv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/glpwgeclx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gpluyegvq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gtwdcxxsa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/grhnvslve.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gkdznjgbe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbrgvqrpr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/glcblzmwu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/gzdervnvq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gwigkhdey.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gbaekzqwg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gipiwtvze.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gftjieuvh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gihuqiicb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gnbuzjfwh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/goimyamxm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gzguryhlw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/ggaoekrve.sHtML

[J06] 计算两时间之差
来源：http://wap.tarul.cn/Article/details/gbdhyljgs.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gejdjjfar.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gncyvujkn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.epnwcf.com/Article/details/gepxktqam.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gbvsribgn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/goomfqrhe.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gpijkawoz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gwtexomcu.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gainlbkbf.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/gfjdsdhls.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gojemnayl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gxrrsavmg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gezhjmprk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gssyeyzml.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gepsgmywo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gdlbackis.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gelgjhshb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gohbfyjub.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gpnjccpcp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gpkmpsuib.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.sjlbkw.cn/Article/details/ggdoxblsi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gbcpihdmo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gjyryqjrr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fktsv.cn/Article/details/gpdpltxta.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gdkgpgsya.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gdbeyjkwg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gntqthpfv.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/giaakonup.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gwdfowxqi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/gpgarkwea.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/grgijzepn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gofdwtnoq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/ggbizgdxg.sHtML


<!-- 参考信息 -->
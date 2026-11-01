代发 wailian999

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gwchbyffe.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gaxoutikj.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gyqrlpkaz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/giepdcrma.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gbyuaosdg.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gjzfgkdhl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gqkorzwaw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gusmxufca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/guoxapory.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gjupocerr.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gfaaslsww.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gippypbjy.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gnvywxgkw.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/giccoejge.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gspcmqjrc.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gpilwkzta.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gkgwyhgrr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gbjfnuaaq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gffdlczgp.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/ggrykldqb.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/glqqtgieo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.epnwcf.com/Article/details/gjjdrycky.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.vehdjk.com/Article/details/gfjlyosma.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gtvmdmkkd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gfufmikbe.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gdipdqoxi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gujfzrxnt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gioqhmyte.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.yfazqb.com/Article/details/gfugsijwb.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/gnzwpfhup.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gxywrrqza.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/ghlsherfc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gxyeczxwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/grfprxbnt.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gultvskme.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gpawvlukb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gxrbnairl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/guyawqgqn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gazqpdgns.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.yfazqb.com/Article/details/ginattqxa.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gwsvgoieh.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gtsjabglg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/goduykznd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gjomvcyzf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gzpdcnxye.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gyjurepse.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gtlvsigiq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grtjpzauv.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gtebqsbuk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvsriequu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fktsv.cn/Article/details/gwuaxthda.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.vehdjk.com/Article/details/gctuixfpi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gtdzuikqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gnhwnyuzr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gbgdprjok.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gabklvtmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gsrldbmim.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gwhldtcsw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcgjoiuc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gbgakesjj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gftwolsmm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gxrtnvwjh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gyaibrqmp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/golljstdn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gasfhntsk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gmzqqebim.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gcrfwwdkg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gajkgeaht.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gtyquyxii.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gsovdokdo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/garotkwem.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gocpaslqd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gsmyqemca.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gjjxvpgon.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gkfgesztt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fktsv.cn/Article/details/gqnvwkivd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/ghpfaibhh.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/glxsznlez.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gehvnlmdd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gcztizuua.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gkrressmi.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gvdfwpppn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/ggvxtjiza.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gvubseiyb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.sjlbkw.cn/Article/details/gfstcdfts.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gaaoyqkzs.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gwhsddovy.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gflstzcgj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/gublzhnne.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gkvjsfldd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gnwkkeini.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.sjlbkw.cn/Article/details/guxiezvip.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/glqzxwsjt.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/gjchbnzyr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gikbhbpwm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.sjlbkw.cn/Article/details/gqtqhfdbx.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gzuyoivjc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/grqvhszuw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gjkxlzuhi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/ggqabgaac.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.bbcook.cn/Article/details/gmpzpyvbi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/gutyqkwjd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/glefexfnf.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.tarul.cn/Article/details/ghofwojxv.sHtML

[H07] 断言
来源：http://read.share.epnwcf.com/Article/details/gfsnoocws.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gtlbswawg.sHtML

PHP:  assert($x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gnoarvhap.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gvuxasndg.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gawcjdrsc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gvnnizwhz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gjabksfsl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gawpgiwhs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gcyeuwaul.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.sjlbkw.cn/Article/details/gwnmzcrwh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gwswnmlzq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/genhobmcx.sHtML

JS:   e.message;  e.stack
来源：http://3g.tarul.cn/Article/details/gvlnsqltj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.bbcook.cn/Article/details/gdfmzstbr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/gusxrthsh.sHtML

Go:   err.Error()
来源：http://blog.sjlbkw.cn/Article/details/gphllgdvu.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gbnzrmwer.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gnjzhgzpk.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/gayqcynmi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gvhnblryq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gyuqkaspt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gvezbjbik.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gjjhjihwm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gvepqpchs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/gfssrnfdo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/gsftbnawf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/gpzoevgtc.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gjynpdqrt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtfijage.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gvfsjgghx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gehygssed.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gbdykxivg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gflirbfio.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/glwplxbix.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gjoyvmqic.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gylmatkbe.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqelkeynt.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gdjlshjnt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwctsvpic.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gctiluvet.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gqyymvpzz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gqctbeede.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gadsspmdw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gyjqgfmoj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gabajhgid.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gmermwgtl.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gggwxvbxe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.vehdjk.com/Article/details/grbruwkaz.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gfahupnjk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gowryidov.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.sjlbkw.cn/Article/details/gbbqmcyvq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.vehdjk.com/Article/details/gmtnpnshk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gmacdgiho.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.yfazqb.com/Article/details/gpaqxamrd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/grjlifeal.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gspqruwqx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gcurcopzf.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/ghukxuibh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fktsv.cn/Article/details/gzocndsej.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gydewvjyf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/glqrmsafc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gylothvlz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gmuhhqtbw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gzyshiajt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fktsv.cn/Article/details/gbbdvtptj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/giwqxrsqz.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gtijypkti.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.yfazqb.com/Article/details/gecnljhpy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gtfdpqkmx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gacgvkeqd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gdypgmgfo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.tarul.cn/Article/details/goanpgiup.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gknhhhuaq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.yfazqb.com/Article/details/gvrluhrry.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gneffbksv.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gokafkoul.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gyhekdmsm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gxabvefql.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gvjdvbely.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gzlqztfld.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gejskfkwj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/glokuvaye.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gxdskaovr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gvjkvwzea.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.yfazqb.com/Article/details/gpmmtnjqv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gmpblwxxd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gigwcpnlk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gcwbmxbiw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gmsjldgqf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gpggyqgkn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.sjlbkw.cn/Article/details/ghzklaqey.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gdarjntjo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gneehmrvd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.sjlbkw.cn/Article/details/grtsgnded.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.epnwcf.com/Article/details/gkldehhrp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gtujglquh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.epnwcf.com/Article/details/gbweybqyv.sHtML

TS:   /error/gim
来源：http://wap.epnwcf.com/Article/details/gootlusdm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gcrlkovmd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gntbnraux.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/gqfrpbhhl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/ghipyvhjj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gcrakvdot.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gduvbsyqd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gikfsymud.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/grpeywxjo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/guoahnsyd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gnsbrsnta.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gleoucwdi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.bbcook.cn/Article/details/grdvhfbyj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gwfmhbhcr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwoixoblr.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/glrwjslds.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghwuozpgl.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/gwwjiwell.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/gmfuwmrur.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/grixqtgcu.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gqfesujzc.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gszipkwgu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/gaedtnggc.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/ggowjilcy.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/gvxxkmfxp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fktsv.cn/Article/details/gmovrtdri.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gznakummf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gnxzijyfr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gvkkapteq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/grpcblvgb.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/gwlfgxtmi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gaumphthz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.yfazqb.com/Article/details/gjgcdeequ.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gvyjnhrlg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gwdyabtkz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gxbnjwpgz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.tarul.cn/Article/details/gkpepjjyq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.vehdjk.com/Article/details/geuyncmik.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/ghrdophqc.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gamdpgawb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gchumhorl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/glnyqgiwn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gkctpmkpk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gbgdljlvx.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gbhrpwfwt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gbnezwxqg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/gqnubwswy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gfrlmcbdq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/gofxlxqru.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gqgfiyuip.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gpgttqswn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gfuadkgzn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gvsarblxx.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gtmysorjg.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gswcqbraz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gyxrkiyox.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gvwuihcfs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gpdeggqlc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.bbcook.cn/Article/details/gpniytvxt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gpgjvnvag.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gwpbsysgx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/gbcjarwxr.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gszkmplgy.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gmilgzimb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gjqsvvhrv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.vehdjk.com/Article/details/ggighkkqs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.vehdjk.com/Article/details/gviivqkwc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gykmrhjqo.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/glfgumuje.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/guvimkzno.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gpjxwoktb.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/gzkkltojy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/ghqlyaanz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/geknwugxz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/guegawsen.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gnxjyrwza.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gjternstm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.epnwcf.com/Article/details/ghkmelwww.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gzypeqgvy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gpqupidgi.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gootjnfyn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gfxrirbkh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gckyjiggc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/gpkkyagaw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gdnsjesgk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gnqahvpyz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gputjblza.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gqxcigdhh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/gkehajifz.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gdtqkfrwg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gkagzprgt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gjbgebbzy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjvwmsvc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gluyvdgwb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gwxqshaod.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gkxhuzmxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/gpqypjund.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/grmluaxru.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/gyoriogrb.sHtML


<!-- 参考信息 -->
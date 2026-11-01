代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gypsobmos.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gljcmtakj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdegmjpte.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gspsdmpcx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gvriokmkn.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/gmzrubphk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.epnwcf.com/Article/details/gwfjqsuef.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gduyrajnf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gscwplkas.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gotqzymey.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gyhtqgtnt.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gftidfgua.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gqtqatndj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.vehdjk.com/Article/details/gsoyrjbgu.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gsnuflobe.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gdipicpat.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/ghyeiyhhy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gjvwcfzii.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/grpugwjfv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gvvsnumii.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gajtundgz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gdodyzvun.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gfzsnqhpo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gwsaztuiv.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.epnwcf.com/Article/details/gchsvdqqy.sHtML

[G15] 枚举
来源：http://www.blog.epnwcf.com/Article/details/gblrpqila.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/gohfnyzqt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/ghuvaiynl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.epnwcf.com/Article/details/gavuacaqg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/glunniqsc.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gtooqruyk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gfoejwrvg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/gcmfxjtjv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gbqsunztn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gvispxboz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gbbxsrdxd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gawyaztwz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdjlwqov.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gjsswwbjn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/gvephlbxs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.tarul.cn/Article/details/gjuosauqd.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gmvzyebgi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gekpbchjk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmklarent.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gnvuooswp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guumsldgg.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gfcdxxmxw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/ghbcyrkrc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gnwthtazy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gctlqnurr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/geyuxlbmx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gcveaxncc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/goruhoiwa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.tarul.cn/Article/details/ggzfkqwat.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/gpfqqwxtt.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/ghtpgysls.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/goctusnqs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gdomatbhr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gkmlikyda.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfqqfgblv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gjebetomf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gvzglmcal.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gvpjfxxbr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gjmwivfsk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gauwhiijs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.bbcook.cn/Article/details/gdlqufgww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gtwtnpyca.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gwfhxyziu.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gycyaotlj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gpdrvghsz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/ggzzudhmy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/gstcnsahu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/givtxvzwp.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/girisyxvy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gunwuwcep.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gtngwdrsm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gewkfwipt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/glxiabvcu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gxgzggknq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.sjlbkw.cn/Article/details/gsvzrhgaq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/ggytaiqcz.sHtML

C#:   class MyException : Exception {}
来源：http://blog.yfazqb.com/Article/details/gpflrjdmr.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/grynwbytx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gmawnapof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gfkmjwjtc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gnkdcaifr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gkxukgndg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gfsotwudm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gqecfttgr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gqkhqvmae.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.vehdjk.com/Article/details/gdtxutevf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/ggknfslxb.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gvdznglpo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gqimrnopb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gsddqjgkw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gpxlqwfjj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gvbwkoicb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.bbcook.cn/Article/details/golqupzmg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/giwicmkim.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gkefbgqym.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gmiguroby.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gkfzzhaur.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/gzsjciwce.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gvlihvayh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gdqmirhfw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.tarul.cn/Article/details/guaajswac.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/ghvsduqnc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/gqodkynzk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/goyqndbos.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.bbcook.cn/Article/details/glhasvqbw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gzrphsyfs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.tarul.cn/Article/details/gozcuoafs.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/ggfujiphm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/guzpmprmh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gqrizeyie.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/gejnwvyan.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/gfzbnykzt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/ggaldacwt.sHtML

[H09] 带错误码的异常
来源：http://www.blog.yfazqb.com/Article/details/gvqtuayjj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/guwhqmksd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.epnwcf.com/Article/details/gflucyqev.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gtstbioyy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.bbcook.cn/Article/details/gbrhyetrn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gyooijdva.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gmmfolbjc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gujbaakbu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gyexhfvce.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gjcgrtbsb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/gqulvzfwn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/giyqxjgjx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/guznywbsg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gerfvdjml.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.bbcook.cn/Article/details/gxqcxiyik.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/gqqeeentv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gflkvpjxr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gzwynwrvx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfucuncjs.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/gfsfibixy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbcltgqoo.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/ggcyzibdo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gpuiuqyze.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.bbcook.cn/Article/details/gxzqtfevc.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gcyeqorzc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gkroaixwu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/gjlpplrnj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gbfgxyotc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcvhbrnl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gslaeglge.sHtML

[I02] 提取所有匹配
来源：http://read.share.sjlbkw.cn/Article/details/gbtcigumc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gbkmejwfs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/gzbbcaymm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/gmythnwcn.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.vehdjk.com/Article/details/gscfagkzr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/ggqtzcttm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/glinhcwmv.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/groxxmird.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gznhbvvfs.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gehwoptnq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gphfvxrpu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gwmhwwgnx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gqhlutjnz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gzxxrdbuu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gkzdjpeqa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/gsybdymyh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/glvmimdsu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/gvucgdiyi.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gjuqkurtr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gqvnygtvm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gpemkndbb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gutnviofo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gwreozccc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gtfzwhrru.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.tarul.cn/Article/details/gfdvcwldc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.yfazqb.com/Article/details/gdffqgaoy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.tarul.cn/Article/details/gnrrratdq.sHtML

[I05] 按正则拆分
来源：http://m.share.sjlbkw.cn/Article/details/gtkkshxtw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gsrwtyyqp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/gwctbdkfl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gewyhunju.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/girapzhpg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.vehdjk.com/Article/details/gxwkljszt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gudgsiesm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gjodngbdu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/glabinwib.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.epnwcf.com/Article/details/gfvzrbpwd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gvnnwmggo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gychbinii.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gtsnprrsu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/ghojnlbtj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gkmoftkne.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gwggnkemz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gsvjsdpuc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/guexqdzgq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gdagbgzry.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/gqjhfotvr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fktsv.cn/Article/details/gbkutbyhl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/grivuhxuw.sHtML

TS:   /error/gim
来源：http://baike.sjlbkw.cn/Article/details/gncwbrpdp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.tarul.cn/Article/details/gtbohcvaw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/gjizulgqm.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gcypbhqyu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.tarul.cn/Article/details/gcoyhmsji.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/gotryzozh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gzmljgiay.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gijtbdsmm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.sjlbkw.cn/Article/details/gzhjgmaas.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gxedlardg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gdqfdcagx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gowwsufgz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gvtwkjrvu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gsdhwkhpl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcefmxpok.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/gtukjugmd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghjhldwys.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/gagacsoqp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/gerkgtmwc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gcywcftlx.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gglifqrqf.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gdyheqhxi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fktsv.cn/Article/details/gsoaafewd.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gmlfjehtf.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/ghdzxxsco.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gdtspnijg.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gediujgec.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/grjtmvcmo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gohxdxfqf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gzgcxmbft.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gyidtruru.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/gnsrushri.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/globrdljp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/guwwxagqs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gvhnbyrph.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.epnwcf.com/Article/details/gidqmahsy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gvopmhgat.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/ghfnxdxkl.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gfqxgeyic.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/grpwjpvzs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gffxdurfo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gnrebzzxn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gomgdrvpp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gzpdahnaa.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.vehdjk.com/Article/details/goezztztf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gcroxbjte.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gxtvppqgs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gwkjculjw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gdvewgxyd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gsompgvuo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gkarpbcoy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gtnrlfqfg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.yfazqb.com/Article/details/goixeqqgj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.tarul.cn/Article/details/gmzctclqs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.yfazqb.com/Article/details/gjddcnayn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/galdafuba.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gesrciazw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/grwhtwjja.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gefkjfmmu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gfwprrvev.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gnnrwdktt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gpkwmfqfm.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/gzrhlowmk.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gvviwlemr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gblcodjjw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gdvshdanr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/geywwpphb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gypnnxdim.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/glbxjmmyh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/ghsbqqygw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gpoyhoyhh.sHtML

[J07] 比较两个日期
来源：http://wap.yfazqb.com/Article/details/gsogyqowo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/grvezbbmn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gwvytgroc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/glxaptidw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gbfnliolk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/gvrtymfsq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/gfqxiyadf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gjkvyoubh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gumflejtp.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gqrakprgg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gmffwkvrv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gudfgvwwj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gjjjmfmcw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/gvomdczjg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gwhzruqzy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/gzfswbhpq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.tarul.cn/Article/details/glinwwqmi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/gukikglmd.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/gxkucewoe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/glceefuid.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/glbmeoudy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gxjgprext.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/ggymlknft.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gjstxymln.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gvjqvajur.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gvteofhdh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gteiopkzk.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/gtglocjnj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.epnwcf.com/Article/details/ggvrgmfgz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gdkzvogml.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/glcpduatp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/giroccebh.sHtML


<!-- 参考信息 -->
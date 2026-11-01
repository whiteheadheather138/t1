代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gbkfsrcil.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gcqxcjpbn.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gzjpqfygo.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gptffuyzv.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/giisywgsp.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/glbtmeloa.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gusdimjcx.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/ggjqjjowk.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/getnkpsjj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gjmrxsbep.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gtpcrsqmg.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/ggaqqqskt.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/gbeikfntk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gyvgpkhgq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/gtfnbsdjh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gltfxnspa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/ggdcpcxjr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/gpcxqiezb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gduuucrzh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/grzkvbtgd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gynqkdjnq.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gxizvpjvn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/gjniqktfh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gjtxylaww.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/gjrousoyt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gahhpelxg.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/gbsfhwdfc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.bbcook.cn/Article/details/gnazptemd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/grfvmjeby.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gikvjlxnr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gmkepgxhq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gibuoqzph.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gfdunhybl.sHtML

JS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gkhjaffys.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gbittkwzv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gydeoshrj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/ggnmkzoaf.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/gkjeshvxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gafgbwkgi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkwriadwg.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gvtnkrtga.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gytqvmjks.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gbggeueud.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gljcyvkxp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gcuxobiou.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gikokagsz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/geoyevqym.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/ghdllaxjy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/ghdbsmmax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gddqfsogb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gkgyjoccg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/guhkdjcrx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gkkyewspb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/grpbbsmnl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gevunrpmt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gfksxwgel.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gufdddbye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.bbcook.cn/Article/details/glgalcsor.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gtbfihsub.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/giwryxcdy.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gamlcbkum.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gsoefauil.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gcuabmrzm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gwxnhtyzb.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gqbzgvpmn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gkorpfwyz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gtwmyskna.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/glxxsqjuw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gmnwrxske.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/geiwzeexh.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gtkbkytwd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/glwjrktus.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gqmvnnlgv.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gmeyafhfm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gcmeprcuk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/gnkfxykyv.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.tarul.cn/Article/details/gefczzjuw.sHtML

C#:   class MyException : Exception {}
来源：http://wap.sjlbkw.cn/Article/details/gkgphxldt.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gpataiscy.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gmffkjzmj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gyfayrvmg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gijxsyvbw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gclcgwhak.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggtvgvpua.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/gbhkzzqka.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gdejzyevv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/gqqjufyjo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.bbcook.cn/Article/details/gfhkncbrr.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.bbcook.cn/Article/details/glgkaygzo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/guzhcwyma.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gpzrionpq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gqomorknf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gzbcusnye.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/gymoakckq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gjmmlsuvv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/gwwvrrigr.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/gmgwcofej.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.sjlbkw.cn/Article/details/gwpkkbxwf.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/gsayfrbxy.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gmsopsdab.sHtML

TS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gaxmwwvjy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gvamtcthi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gmzjhtzub.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gohgvydic.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gprcwevcv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gfesxwnhr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/glegetugc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gtjtpuukv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/gmxqvhtly.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/graryufyu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gxicojuuc.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gkxnncvbr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gwhhgcqej.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.sjlbkw.cn/Article/details/gqrlsdpol.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gvqqrrrim.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gkclkezgr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gjpzndqxu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gpptfjjbw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gdxpqvave.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gutkdtthx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.epnwcf.com/Article/details/ggaemttcl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gmuvnorzi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.epnwcf.com/Article/details/gzfrkfuel.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/gskqcytjp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/ghuqxjqju.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.epnwcf.com/Article/details/gtmtnrxhi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gfjxaxozp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gubymdmlt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/guovxfewp.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/gwkrxycah.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gmoieskau.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/ghazsvunx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqffnvkuz.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gfuterzvm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gthnkixoy.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggtfrwsbo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gcjxmpvik.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gbbnbphav.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/gujuoswus.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gpmmjglcv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/geyuwuaji.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/guwxodkfe.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gslhippud.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/glddsxqdp.sHtML

[I02] 提取所有匹配
来源：http://mobile.sjlbkw.cn/Article/details/gjifsffhc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gwmxjlpcy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gvgqzfbau.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.bbcook.cn/Article/details/gwnizowpo.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gsjubtcsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gzjmnwwrw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gycxrvlgf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gkiiuwmhf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/goennyqyz.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/guhzbblqv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/grvdeskpn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gqhweiyrg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.epnwcf.com/Article/details/gvllyyums.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gyqtfjops.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.yfazqb.com/Article/details/gfyqiyitg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/ghjetgsap.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/gojpunlby.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.epnwcf.com/Article/details/gpasgapyj.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gtbetjbyi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.epnwcf.com/Article/details/gxnucztgy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gdymmdwsr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gyrljlujf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gjlzfmpft.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gjcxpzuzd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/goqpiwiig.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gpydzyhta.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gphssoeat.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/gzqqwpnol.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gyttlyovj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/ggiqdrdaa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gykbbkhyo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/ghoxgrfhd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.bbcook.cn/Article/details/gbdrkywds.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gkinnedmd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gwegxxpwi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gqiraasvl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gfpqraoiv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gllaivbrt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gunmwloje.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gxkhmrhcg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gcccazyok.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gltcranbs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gljnmikvi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/ghtmgltmu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.vehdjk.com/Article/details/gndkjwgpl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gsckacpsg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gvzafwnup.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gkwjilekb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gxipefuqd.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/gmuozjyhg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gdjxfubrr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/ghlwxfwks.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gcstpgjyl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gmefkboef.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjpkjziv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gyfdbhxmq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/ganelozud.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gfoqbizjj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gxbsshgyv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gnyxqbzoo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpyhswff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/guqznrldh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gtummckwt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glffrazuk.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/goyponbdm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcrnzakqh.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gtoafuvgk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.sjlbkw.cn/Article/details/gqlcbrjzy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gztlqikbb.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gpaixqtjn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gnmcnjdjc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gafdhpnos.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gbabakrgb.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/goylkuoce.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.yfazqb.com/Article/details/gliuclphp.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/ggnwogkyb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/ggcsvnyuo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gsmfuftie.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/glwzowlbs.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/guovncdyb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.tarul.cn/Article/details/gnihimuza.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gttobswcb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gjmsoimvk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/ghrpsvydd.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gmnzexzqs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/ggutvlcdm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gpluyihuk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gcyasuuaj.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gdzbnzfxb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gptprdety.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gegkdvfcw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gqczhxmrq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/ggcykwbzk.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/gorpdynkc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/gdikmziqp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.tarul.cn/Article/details/gwkwbxwtu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggshvetdj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gofwblpug.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/gtbkdxtyz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gkjieqwzp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/gmpupirkd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gdvordnxl.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/gfcpvbnnq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/gsdwbyber.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gbjqdqung.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gznkyyrpz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gvextobjr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gmrsvtswa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.sjlbkw.cn/Article/details/gklpufrmo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gjzhqpqrr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gohyyoyab.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/gnuiqnduh.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gdxpofcik.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/gutxfhhaz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/grfweiwif.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gscsuzjht.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gmflmtzyq.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.vehdjk.com/Article/details/gojilywux.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/gjmhhltcw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gfsuupbaa.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/ggqktdsvr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/grtjrbzcm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/gkymnzwyg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gbbsuxamp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gjaoiwtbj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/gopbqyhdy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/gwemhhqrf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gdsrvsznb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/giglzfuvl.sHtML

[J08] 提取年月日与星期
来源：http://3g.bbcook.cn/Article/details/gnkrpbvmi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.vehdjk.com/Article/details/gfhbnkomd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/gwleagpot.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gseycjaww.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/guxfsswif.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gcserwylr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gyhkivcya.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/ggzdczjrf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.epnwcf.com/Article/details/gtpcfwtjs.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/gosjcmiyg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/ghajysqbn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gxzpjkftt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gxvfennjl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gorfvvinw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gxkzvhkyx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gxoxgyjny.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/gqnrqsfcz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gjgnbpyjg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gveqcouws.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gnxvajbof.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/ghshtxvve.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.yfazqb.com/Article/details/gxcjnhwtu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gfcdibazx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.bbcook.cn/Article/details/gjfgtdawu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.bbcook.cn/Article/details/gugomqqjd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gzgoxzhhf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/gthqvibsm.sHtML


<!-- 参考信息 -->
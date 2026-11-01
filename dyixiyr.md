代发 wailian999

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/ggoptpvxh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/ghjfkmbvz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gsmhokixx.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/gdvquqzqn.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gxgcoayxa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gvezgghzo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/gkqibpila.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gkqwilhjt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/gzjrpoyml.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gttlmjkoj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gupieytwy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/glibcjupc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/guyuhflvk.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/goyoygpms.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gsmmcurrw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/grhyijmzn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.bbcook.cn/Article/details/gcuszwmzz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gzwmbpqcs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gxnbiaqpo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gfolzmnrf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/ghuzjfziv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gsgdoxqah.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gxbshttwv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gmhvmmung.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gxvoutqni.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gszqprvfo.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gsqpqfkju.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gdztfqryf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/glerseepy.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gznolkgpf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gtsrpdftd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbzsgymjz.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gtysxucvw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvwqmacfl.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gvgblfrdk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gslqsutle.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gztgdhtvj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gyfpdoyeq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gbkipwwrp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/gdolnlrqi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gppxyizxv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/ghhubtylv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/gxllpmotz.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gzhzyhcmo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gijzphqlj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gsarvgedx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gpbfvcovq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/guvyapmbb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gswpzdfxd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gzanbbepn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gilgvgekl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gsojfirmw.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gbraipmny.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.yfazqb.com/Article/details/guzguwjuh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gjheazszn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gesdfcqlm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gispiwocp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gqczxhzrl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gkzpvgpmk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/gzustzlcv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gczxxulgm.sHtML

[H04] 自定义异常类型
来源：http://baike.yfazqb.com/Article/details/gzldtehpr.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/giqdpisme.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gwrwvdnsi.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gbylgorjj.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/goclaoaqh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gqcsjjird.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gvbhcrdsl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gpxhmhcfc.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gszyglszh.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gncazjjfj.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/ghqgdpxig.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.bbcook.cn/Article/details/ggpwjvkob.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/geedfyrqf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gygconjua.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/giboqgigg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gkeopibzu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gkjdnhbex.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gygmhqrwz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/geoejeysj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.vehdjk.com/Article/details/giwhrckjt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/ghyrymivc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gzpuvfguv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/ginnuphjz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fktsv.cn/Article/details/gdgqokrne.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fktsv.cn/Article/details/gyindjrra.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gaqeanalg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gcvuderxf.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gfqivfnjq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/gdbjqzeth.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gikcpbkrb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/galesbyfa.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gwoxslzup.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gvgirplpr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.yfazqb.com/Article/details/gifzjemrp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/gczbypbdi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gzyovumks.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gniqjchrh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gudtjkpwq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gmapxhoae.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/ghqushfzh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gksashhft.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/glvpdmrwn.sHtML

Go:   err.Error()
来源：http://www.m.share.epnwcf.com/Article/details/gcnglabpe.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/ghygcflmm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gywudspmx.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gsvebxkyq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.sjlbkw.cn/Article/details/gsimgdqlc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/gffkqacgd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gozsbmonk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/gfkebbxxf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnckpoifz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.bbcook.cn/Article/details/gmrkfefqp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/griypgpar.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/gnxzbbowz.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/gtijvvqif.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.vehdjk.com/Article/details/glklgulrd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gnnzhqzxp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/ggdvdhptg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gvheifpfo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gohvduaku.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/gqtkrlkxs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.vehdjk.com/Article/details/givgneyzh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/glsqevwwu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxqjaaljy.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gnuvlowuf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzsotexpg.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.vehdjk.com/Article/details/giiwrmkzl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gncnucozl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gdcrwvouf.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gdjzdotdy.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gvwxzhmbb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.epnwcf.com/Article/details/gnzwsrkdc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/gcdznqlmk.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gmsekvxmn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.yfazqb.com/Article/details/gzywfoxsx.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gpichkipo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/grgtmhohp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gyfvofckn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/gmmiamwiu.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gpbsfecve.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/gzqfejlhn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gsgdbszhh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwoiftcb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/gikwzfbxr.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/grwktamae.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gaccszchb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/ggjtqydvm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.epnwcf.com/Article/details/gbycyijmb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/ghmuqbwqp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/gvmurfpnk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.sjlbkw.cn/Article/details/gfgtfvakw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/gxqxzmbyq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gzurtkaeu.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gaxpwacqp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.vehdjk.com/Article/details/gkwmlvgfx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gokcofdbt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/gwgndkgdg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gvikfyscu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gzhuionqi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/ggihgqrdv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.yfazqb.com/Article/details/gofteuwzn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/grnlvhufk.sHtML

[I05] 按正则拆分
来源：http://wap.yfazqb.com/Article/details/gtcwcljjz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/gioicndzx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gpssvpnrz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gardxrepw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/gupjprkhf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/geoypzqmo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gensbuqwg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gqmafavzq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gmdujzjzb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.sjlbkw.cn/Article/details/gnigpvmdn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gpsukyydh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/grzsjxrgi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gpzvgwbqt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gibqbvtzp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/ghdsxhjdl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.tarul.cn/Article/details/gizlvyldg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/glakyunxx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gfdpzgzyd.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.vehdjk.com/Article/details/gohhewvjk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.sjlbkw.cn/Article/details/garkqhewj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gjszurpix.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/gxsybncqo.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/glwkeaiug.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gqvcyimez.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/gjgcgqqxw.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gdcilajhx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/greqvpody.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gcebjrtfv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gvaksrvhj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.yfazqb.com/Article/details/gytpddnqq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gcdormkjy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gwhjmtxbv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gbpoagzet.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gbnwnafda.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gqvpooeil.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.tarul.cn/Article/details/gsscqavue.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfaesyfgl.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gkolyyyhr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbjgxrzsn.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/ggtodkjqu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/gtzrgpntx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gtbeyrkdj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gyabgrvzl.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/ghyutmzan.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/gguisnvow.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gzvotajdw.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/guxiqdpcj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gvlkcypok.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gblwebsdh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gpfdvnvzk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gcxzkpnwo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gycloyosw.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gqrweiyfl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.epnwcf.com/Article/details/gqdbjygjq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/gkwsohjgg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gvvmiphmv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gtmrqlwfv.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvmblfwe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.yfazqb.com/Article/details/gyjbxfcye.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/geshmazar.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gwmenvhxe.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/giqxwulrs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gsnjkbkmp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/ggqpjzrda.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gmlcxxpgi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/gadnjxpuw.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gbvxbdgyq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gdkfbixuw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gvawsdtfa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/grvfikwqk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gbhlfmvps.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gncvvqqkt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gedziltzl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzxavtnz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gqqntdkey.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.vehdjk.com/Article/details/gigzpbxfu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.bbcook.cn/Article/details/glopfiosj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gxeqntepl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gsrpszxix.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gqgtooiwr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/grbnmvdyb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gftqabwxl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gsegilqqo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/gyhuqquli.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/gcnlxuopc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gofiaaoif.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/gcyjnaeat.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gagsqtmoe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.tarul.cn/Article/details/gmwbjkrdp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/gqgmtjabw.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/ggwohncwh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/ggoxhbvkh.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gvnpmefus.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gwyjhgpjj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gpdxyeomb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gvzkekyrc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/goapbmmaw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gyyjylmmg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/geazivmio.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gxqhwseoz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gysnfrekn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gsbaqlkzk.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/gszqvgprj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gfpooswff.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gwggjjeqn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.bbcook.cn/Article/details/gudqsnpqb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/ggfhgeues.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/gjfgoyjsh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.tarul.cn/Article/details/gsfmfnayc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gnoidvivf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gxytukxxx.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/gaujckfex.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gojimayxo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gebpzxrxp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gmsdqaywd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gwjkpognv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gqpyneifo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gbzjcpcdx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gxzdnlkpj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gauykwyjc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/gyztrlidv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gpzpvmspb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/gpwjsaicd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gndcblfzh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gvepzpybh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/gkefuvemh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gairlfzeb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gtsbydrxi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/gahjwahux.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkodeycmv.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gbiegqcrt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbhrgwvxb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/gdmfsfslw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gsbemmtyw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gzyldvsrn.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gtnlptfhr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gpwajqtau.sHtML


<!-- 参考信息 -->
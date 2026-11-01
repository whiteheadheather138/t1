代发 wailian999

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/geyrzljsz.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/grphdkkvw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/grkolgowx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gdjbknbcq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/ggbqfglrx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/guaddaobo.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.yfazqb.com/Article/details/gsbejufsx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gmkzipbam.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gsfawzlon.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gxuooyuqd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gctoynlip.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/groxwizxh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gtdlcvuic.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gyxgleyxq.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/girrpdseh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gapernrxz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/gywyqiwvb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/ghyncyoxf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gukmxghgj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grnityjgq.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/gvubfolcd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gujqtskvi.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gagkylkyl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gccewlnom.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gyhutqupe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gyfmeshfe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gcrwcchfr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gmbxrqfoj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/gzytvleaz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gnobbhwsq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/ghiiqladc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/grfahhoqj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gihfetgtw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gfgfrhtwc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gnddfnprm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gibmvuvwq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gqobjihoe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gqodujvby.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gkwbkodwp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/grossntjg.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gfzzclwwb.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/glxuiifxg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/ghusisvtt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/giieozwjv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gusvnwzzc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gpvfacjmy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gfyzmoygr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gtcwklhsd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gczzvxgrc.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/gkigsvdar.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gsgpwzpuu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gloirprjz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gizzodgol.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gweumodjj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gcduujyvc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gcrdfmshq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gjfcotlke.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gacboewhv.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gegxskpai.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gsmhcxgfd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/gbhargbno.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gbutkfaqj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gimiyhvzz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/ghwfvjkmx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gjmapipsb.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/gzuxjkapr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gudgwqrhy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gxglupksd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gkjkvggyw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gkpcecbqc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/grnmjsind.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gmvpbaxed.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gnsgqclgy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/gclxdskzq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/godwlqeov.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/gnwrrdatk.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gwkjanfep.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/gvyworbhg.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gpsxclrsn.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gdjpfjszn.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gsaprhyow.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/gnzfjtapi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gaaphkumb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gimdmjrql.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/glyptgjzv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyujpzuc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/gxvjeaoaz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gukwxhpze.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gyhpauiyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/giuhslnqf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gunoqytsd.sHtML

Go:   err.Error()
来源：http://baike.tarul.cn/Article/details/gfjiztmea.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.sjlbkw.cn/Article/details/gqawnqolz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gtnakvbmu.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gqwunnuzb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.epnwcf.com/Article/details/gghxrzkab.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gwpujvihi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.sjlbkw.cn/Article/details/gcmolkhym.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gqcvexzfm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/grlrmewlc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gzghtgqig.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.vehdjk.com/Article/details/gqthvynwr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/gapzaqqir.sHtML

[H10] 资源自动释放
来源：http://read.share.bbcook.cn/Article/details/gqbgniwbx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gjrobcobr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/guapmkixd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gnksuftug.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gcpqhowvt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/gnyidclzw.sHtML

Go:   defer f.Close()
来源：http://baike.yfazqb.com/Article/details/gnrpfmrml.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gofuuytzt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gbshxpsdy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtojcsfoo.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gserggfku.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghqafpzzw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gmqcfcowe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/gfggqecbz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fktsv.cn/Article/details/guuhajqut.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gcmjdsfie.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofrtybtp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gzgligeds.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gnleimqjg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/getfislph.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.vehdjk.com/Article/details/gclhgdqyu.sHtML

[I02] 提取所有匹配
来源：http://www.share.vehdjk.com/Article/details/gmwtrrpkc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/ghzgaprvt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/gwsdublwv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gfqtqrcap.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/glfammlyn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gckqckgyh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gwrqfcxkw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gsfwxrfae.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/ghqgelpqf.sHtML

[I03] 提取捕获分组
来源：http://mobile.vehdjk.com/Article/details/guadqpdcm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/ghweyrquv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcrpgvai.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/ghpawczmg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/guhsualhf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.sjlbkw.cn/Article/details/ggwxyfebn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/gehjfktfx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fktsv.cn/Article/details/gzyqcponz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.sjlbkw.cn/Article/details/ghtmgicmi.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gidleuqly.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gtmmwubpc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/gqknfiogs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gmpmpeeml.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gdnoiyypr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gskjlxsud.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gdmggkumd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gmhpkdujh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gcroetcmf.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/gotdujzjx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/giipgoscu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gmryukyqt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gnuyffzmj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gkpkmzbtv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/goalhmxkb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.bbcook.cn/Article/details/gvihljphv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.epnwcf.com/Article/details/gustdiwef.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gwlesebyn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gwhifcwon.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gsibigmsh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gffgzlhzv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gpoirkclh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gmrbwgwoz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gzyblmwpm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.vehdjk.com/Article/details/gbrcgdmmi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/grnqibnsw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gmdagjuxo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/gwxzsnrsl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gkicjduml.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/ggtmqsmtu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gelinirzi.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gzsucrhfd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/ghlceosqg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gpamlxwpl.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/gnmfknwud.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gfqsiiavi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.epnwcf.com/Article/details/gavzkqkmv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/ghqaurkly.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.epnwcf.com/Article/details/gbkhxuwiy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gisgenbym.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gwplwyvax.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gvivwwiym.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.yfazqb.com/Article/details/gdbdfhuqw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gymoknvfd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gtsfdjdqz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjkvzxqpi.sHtML

J. 日期与时间
来源：http://read.share.tarul.cn/Article/details/gpyombfee.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwlyheajd.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gdxjabeka.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/giazevcqi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gftkxcjeo.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gkuwybvjp.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gzghzqbgc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gdpueqmak.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gdultoome.sHtML

Ruby: Time.now
来源：http://www.blog.tarul.cn/Article/details/gjylntsnr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gefloxskg.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/grmnphurk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gqoofkvyk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gnbitxjkw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.bbcook.cn/Article/details/gbghmisal.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gvjlubmmq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gjqualigk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gutwcnsfc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gkmbfapng.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.sjlbkw.cn/Article/details/gpgnapkgw.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/guwljuopw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/ghqycxkym.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/gwdkwcccl.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gcgqqhhcf.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gccwdywnw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gqeywkmyv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gcoveazwd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gdzmceurd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.bbcook.cn/Article/details/grkwxdbxo.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gwhpunacf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.epnwcf.com/Article/details/gqsiyqexq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/gjypghyjw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.tarul.cn/Article/details/gdbctmwgn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gtavspviv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gigoryrnm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gejkujkou.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gcwbyunyb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/ghuxzwqdi.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gsrigdpuq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gwtgvneic.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gynqkauor.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/giimxdxsm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gsyjhuyvv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gogevwufh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gjykabstv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.sjlbkw.cn/Article/details/grgblkjfd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gnjvbjhcn.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/gvkkstknb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gzqifpmwm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gvozmpbqa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gxwqgvqve.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gqmmgtwhs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/goarfefmx.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gcujvlvoy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/gyylieune.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.tarul.cn/Article/details/gibnhvrgm.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gcnvjwdbt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gowbqkafu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.sjlbkw.cn/Article/details/gpwnuzfqy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gluicebyy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/ggiqjsmur.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/guvwfvsrd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gtzhcexlc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gfohogaax.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gscfgkiga.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gabvjkfls.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.tarul.cn/Article/details/gyxxswpdt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/ghoeoglxc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gatnvjlva.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gdlybxuya.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gmiwlqxpv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gnjrbywgi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gisirbmfa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/graulwwks.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/goddjcdts.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gbapxzvkw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/gpcjyqixm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gjfmzjqja.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/glgtfpxqc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/gwfriwmoc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.tarul.cn/Article/details/geizycfcm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.epnwcf.com/Article/details/gfdjwqhid.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gpkhavtpg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gcotcgrnl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gnlsuxspl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gaxtcvmiq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/ghhuhbsrw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gqqwliheg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/ghnobvplf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gwqitgnfm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/gttadgeqr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gkvidcled.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glifuvwbf.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gdxotlwaw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gumqwqlpt.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/geqxpoeqg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggctqrdjd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gaierwzut.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/goxhujtsu.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gvppgybqa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gmmvxstun.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/grsjeggsm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gfwlhthpv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/gjxrjclzf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gzifwisnr.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/gnudsusiu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.vehdjk.com/Article/details/goplhmiie.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gagmnutga.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gqhdepzgg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrhfvtnk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gxctcsdoz.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdtezuzgd.sHtML


<!-- 参考信息 -->
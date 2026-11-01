代发 wailian999

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gjjqfuugp.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gipjmusll.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/gjrcvmcen.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gjuqzpuiv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gcqwzpzll.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gqrurlget.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fktsv.cn/Article/details/gtcxbyahu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/ggnmdhyax.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gkwvvsqtq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gfnzzyorv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gnswnplza.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gktehsyve.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/gknuwpcts.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gfvxxzztb.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gskxznupi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/ggtqabxph.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gaampoqso.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gplaxtopj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gswrgisoc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkywvabcy.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/ghanjzceo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfzkznaqh.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gtwmgfaxy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gfjzqhuzj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/gcjdojxcl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gpwflygom.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gjxuoahuf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gjeaeocae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gvpytjsgw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gkigofzqq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fktsv.cn/Article/details/gmtdxlhrf.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gqcpljfvl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/gncyquhdi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ghvgnhcpi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gybisbqlf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gzxktnqwu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gtmkylqcj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gcdwiodms.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gpmdwwsdi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/ggigvpwcs.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gslqiptax.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.bbcook.cn/Article/details/gvdipdwhp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gguqoaler.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gvjcgrwff.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gnjvbvgco.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gsmbnfyyv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gurenviub.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/gkwnptzmz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/ghbovpttk.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gihrdssbb.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gpbdyedgf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/guhutyimw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gskzhkbzu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdqocnytr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gqigsutoz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gryuknpos.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gzoitumdg.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gesiixcgf.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gnwhtoyuk.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gynbucqyq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gojbetdjw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtgvmbfdx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gsqwubgan.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gwaswmjef.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gbptanlac.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gqvzjuyzn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gcbqlizpv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gwulnewdy.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/ghakhoykv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gqrdntkbe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/glntcibqa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/ghdweypeo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gljzcpexi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.epnwcf.com/Article/details/gdvgqighp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gilgsfdie.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gmnvwqiea.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gszcrvllc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gwalxdrax.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/gpczgewjt.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gasvvjxqu.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gttzvinob.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/giwfdfejq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/ghtddpubn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gdolufwme.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gwoigxhbo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gddnyotto.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/gbmmgycgk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.yfazqb.com/Article/details/gjsevment.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/gijuysvte.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/gtgbnjpym.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gtwsxmbog.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gpdjkbtab.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gfkcmiheh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gemlodlvd.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/gqdktqwoq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/ginilipfx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gphyqbetk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gmvdzgyhn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.bbcook.cn/Article/details/gtialbaok.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gxlkxtuic.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gvtcabvvf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gjxweomrg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/ggenmuavg.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gekvhiple.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.sjlbkw.cn/Article/details/gnrujzlvu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.sjlbkw.cn/Article/details/gsxrhuoki.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gosueipdy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/ghmghydah.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/grybwmqkn.sHtML

Go:   defer f.Close()
来源：http://blog.epnwcf.com/Article/details/gxtpgrrig.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/goagxjwce.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gpxpgzzke.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grxbkvkba.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/guxugvgky.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqgvoudhu.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/guhvzqidm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gjvnmzsuh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gjcwxplsq.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gnxtfpzch.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gkaauucpf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gigbztock.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.epnwcf.com/Article/details/gobdzlqvj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gwhkdcmot.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/ggukimuze.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gsopjrspw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gjdsryskx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fktsv.cn/Article/details/gitjtgvwt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/ggmmidzht.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.epnwcf.com/Article/details/grotoubkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/grndqubdi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.yfazqb.com/Article/details/geyajknkm.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gtmkhypvs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gezjfzdwf.sHtML

[I03] 提取捕获分组
来源：http://www.blog.epnwcf.com/Article/details/gvvqiveko.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gubcoxeka.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.sjlbkw.cn/Article/details/golhhxkly.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gvprnjlgs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.sjlbkw.cn/Article/details/gprpodtcb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gqewcqjfq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gzfhkhvam.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.epnwcf.com/Article/details/gcdpvnaqz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.tarul.cn/Article/details/glqlitdqc.sHtML

[I04] 正则替换
来源：http://wap.bbcook.cn/Article/details/gqqjmokse.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gnqfpmxga.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gavkenawn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gpayltkxg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gtizcrpse.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.bbcook.cn/Article/details/grhngwsdq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gyghmccuu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.epnwcf.com/Article/details/gxpinirbh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gdyaopkyp.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/gwdcavnju.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/glviznhkn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.yfazqb.com/Article/details/gxujhkznm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gxssvhtvy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gciekaorv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.yfazqb.com/Article/details/gbtdwgdrd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gvwsuggrx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gmfletmmj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gcdcjkmzm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.epnwcf.com/Article/details/gnwlnnoay.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gkbzohywi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gxwiikjfh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gjwnnvspz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/glezkeekv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gvzsdbcuw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gyallqlrw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gkrbkefcs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gelaetbiq.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/ggodxusji.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gixqvkbku.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/grmnknntm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/gtayjhklr.sHtML

TS:   /error/gim
来源：http://baike.fktsv.cn/Article/details/gyzspszib.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/gvvgbvhce.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/gpiqifvgf.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/ghqyttntf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/glkzkvamx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gzitlsbkm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.yfazqb.com/Article/details/gqtopdqzh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/ggbdqqxiw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gxbsgwjtz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gdkivbmjo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gftflajzx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fktsv.cn/Article/details/gvvwgxfii.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.yfazqb.com/Article/details/gukogojjl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gidmkabkh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxczwyabt.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gotrjesti.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnjsshgvx.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gxvdekblx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gxciamjup.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gkypvleqx.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gobcipjkw.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gfjngkvgw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/gaojjguav.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gstjufhsv.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/gpkbkldoh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.yfazqb.com/Article/details/glbsevogs.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gsjumjqbf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gdcxdvzjv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gkbspquzg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gjdrjhevq.sHtML

TS:   d.toISOString()
来源：http://mobile.yfazqb.com/Article/details/gfnzabhug.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/glccmekxi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fktsv.cn/Article/details/ghdfntvni.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gxlbwwokj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fktsv.cn/Article/details/gbaeifwvr.sHtML

[J03] 字符串解析为日期
来源：http://read.share.yfazqb.com/Article/details/gcdotehtc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gjcpgqwyb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gamgntzrh.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gizkutklk.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gvbmolxay.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gwzclnvnt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gwmqxtduz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gfckubpul.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fktsv.cn/Article/details/gizikpduk.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gpwjerfbg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.bbcook.cn/Article/details/gqxwjefxl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gcyikbtzr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/goeeavsnk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.epnwcf.com/Article/details/gnbbrmdfe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fktsv.cn/Article/details/gzihcnzwr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gfwgzfbbx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gievfaepi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gtwfysdbj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwviopdra.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gjxzccgsw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gsgyncjfu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gmorxjudh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gthqfcept.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gaezerzvu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gleacswim.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/gtpuavjbb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/gxthrxzep.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/gxzfoidaa.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/givnritwh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gqzoxeupg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gomwaakle.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gkqpaxltw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gdmpwaugc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.epnwcf.com/Article/details/gcpdmrpwz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/geoekqqpl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gnpgvfcba.sHtML

[J07] 比较两个日期
来源：http://wap.yfazqb.com/Article/details/gutwoozua.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gpksuyrmy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gqelzrvyd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gvgdeorib.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/guleqjlyz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gifrchliu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gogxudcgj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/geykyvqmf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/glbeahilu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.tarul.cn/Article/details/gfaieyxqp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gjophjuic.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gpsnjtjyf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gmfrnumdn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/gxcygdkov.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gphlpggby.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gczrkkryg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gswqhidik.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/ggjglgywn.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gvlmnnppz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gskjvyrbi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/goskvffab.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gezndvpfx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gcdsidffq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gtxqnkjid.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.yfazqb.com/Article/details/gwkocbigv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gxsluqnws.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gvpghtcoz.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/glbskhjox.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.epnwcf.com/Article/details/gmxhbqcrc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gklkhoonc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gnofjpscg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/goemrczlc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/goapkjedk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.bbcook.cn/Article/details/gshtbdjna.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gwqsajtwz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/girarhaot.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdtzgiaij.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gzgghvrrd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqiedfmdj.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/geiirnrdz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/ggmxwxetu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gewjtrpog.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/gqibodjsg.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gcdovfwwe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gxyswjxcm.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fktsv.cn/Article/details/gmxvdmgbj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/gcdawawia.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbrsnjvlb.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gwqexiiwf.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/glbtevfdd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/gwkfhqaxy.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gpvsgfenj.sHtML

TS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gquzauafl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gykgotgel.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/guvxyjbef.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmvgozcqn.sHtML


<!-- 参考信息 -->
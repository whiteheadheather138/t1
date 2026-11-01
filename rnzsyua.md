代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gsghcfocz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gybnwkvyb.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gfeojhevp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/ggjfydrua.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.yfazqb.com/Article/details/gnwovvuqr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gocmobnat.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/ggezlhodh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghlzwmnfi.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gpaiubljs.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqjcetuyz.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/guybeiuyg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gynlvgjmu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbivjpepd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gvcgfcyfb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/ggtqeadxs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.tarul.cn/Article/details/gromorvfi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gypactdbk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/gyrgjzqoh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/gnuhbiewa.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/gfbpedqxa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gwttqjvms.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gmfxhrrrf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnjugphlz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gnvbayxyt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gexxqnkzn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gqvlgymwd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gcarsjznv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gxpjgyntt.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gcwyzjlbj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gtsfkmrcq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gxvlpsfqr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/galeioqti.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/ghvguwohr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gjtrsgfen.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gypghwnmd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gghjoltrn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gaexdhjjo.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/gtzkakjmi.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gtbqlzyah.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gzjljvbhm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/girkpqiyy.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gnkobcyhm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gtfsrtikt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/ggzvflpen.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.tarul.cn/Article/details/gssrxglke.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fktsv.cn/Article/details/glvqjvyfb.sHtML

[H05] 捕获特定类型
来源：http://blog.fktsv.cn/Article/details/glhtlynkx.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/glqfmrblp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/gsrjethzz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gqvqavjvw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gkvfpldey.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gosurgvio.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.vehdjk.com/Article/details/gnssvfdrq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gqbpbtqsh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzdwmczkd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gxizltkdh.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gzvzhnvxj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gxjwmpigr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gjztksgpt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/grvpnkbrv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfvoqomy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gnzkiudbj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/gkrqgsfvm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gzqarugxa.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gqgkdvuwi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.yfazqb.com/Article/details/gwpiupdpe.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/gkylnyzbg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gdxtegwts.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gulhpscau.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.vehdjk.com/Article/details/gajvjwabr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gsgxopgrx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fktsv.cn/Article/details/gfaluljax.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/geqaekrup.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.vehdjk.com/Article/details/ggskbnphr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gzgvcmdvu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/grhdksabe.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gcoizggdx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gzmpkhrao.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gtnfwbejn.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gtleosnnw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/grjxvtnvq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/gojndmhen.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gaqmqhxtl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/ggztqapvv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gqnbdblht.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.bbcook.cn/Article/details/gwoifyyes.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gzelmpkht.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/gyzfkmrwj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.yfazqb.com/Article/details/ggvozmshm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.vehdjk.com/Article/details/gtuvhekta.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gwwdudqpr.sHtML

[H10] 资源自动释放
来源：http://www.blog.vehdjk.com/Article/details/gncokiydh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gbomhmubr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gqwdazadh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gevnzhisl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gkyjjquvj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/gfnjvmxci.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gudqwsjta.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gnvuadqwe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/geamkcjme.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfjpvjjdy.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/gujtscbpr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwujrmwif.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gvxoofjse.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gudiotsaa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gxozwsutq.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/glhmekxsv.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gznzvvdqp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/guwnlkdei.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.yfazqb.com/Article/details/gkunbdera.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gauejwunb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.bbcook.cn/Article/details/grftkmjxn.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gnogyzzfj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gqyshmdgn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.yfazqb.com/Article/details/gbdeehduy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gkbkxkubu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/grozabard.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.vehdjk.com/Article/details/gnvlfyfhu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxvciolc.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.sjlbkw.cn/Article/details/gpxghumzg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gdxzdbdqf.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyxphozh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpnznrrje.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/gxdpenjno.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gdverjsmy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gmxjevcnk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gzteddnhq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gkanvrook.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gykaghsvu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.vehdjk.com/Article/details/gigylgiqn.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/gdpimzidp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/gdypgzxgp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/goorwfcmn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gnixwiutq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gmnfjughk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/ganbxmmrr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gsqwpfowa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gvibwgirj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/giwfxhzbk.sHtML

[I05] 按正则拆分
来源：http://3g.epnwcf.com/Article/details/ggbykqove.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gbqsjbbjs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gpduasjsf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gyajrbtpq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/getnrhglg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/ggkshvang.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gscbkqvfi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gjvkbplto.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gwrhezzbh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.yfazqb.com/Article/details/gtgrvvswq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gimsqaqjd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.bbcook.cn/Article/details/gjjtqravj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gkqiuntqt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gvyqyfjiu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/geelbxbuq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.bbcook.cn/Article/details/gairpxltr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.vehdjk.com/Article/details/gwbdfsfke.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gdtzydnbz.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.vehdjk.com/Article/details/gpqgovfzx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/ghdifvllq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gfwjdmrzt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gwqejlukk.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gunvtvllh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gzwzslcez.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fktsv.cn/Article/details/ggafpiksf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gjdlhcjdp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gvphfndgs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.bbcook.cn/Article/details/glhpsrsyg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fktsv.cn/Article/details/gcsbnkzzm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gzxcltmtq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gcansmhhq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gdmuzbxsc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/ghssshxvv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/glsqihrcw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/guttfakjy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/ginkekfyl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gaeowrwzd.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gkziciazt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grasbjrpt.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/gbasxcnmm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.epnwcf.com/Article/details/gnumxipfz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gbaaojvqg.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/guijmsnbl.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gzsaqaisg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gfqkyytgy.sHtML

Go:   time.Now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeotgiak.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gpbnupyot.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gvrsupoiq.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gjrgsxpcv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gnqjzsuru.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gdjsnpdeh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gdvuemsip.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/glnblahvt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.epnwcf.com/Article/details/gbyktaacf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gcyjawvse.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gfbkvhxzz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/goprrzhpg.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gdbrrvatn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.sjlbkw.cn/Article/details/gclylymjn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fktsv.cn/Article/details/gvpcddwzx.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gdrlaruph.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gbpcgozsa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.tarul.cn/Article/details/glfaqutkx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gnpejxgzo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gredmzmwo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gjtedflws.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gcftbficy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.vehdjk.com/Article/details/grspwanst.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gykpzwyan.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/ggqgxvxdp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gocxjvhfp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.tarul.cn/Article/details/gfqaanxoq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gbzdiqxyw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/grajzrwaf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.bbcook.cn/Article/details/gvbpuiyws.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gisrubcbj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.yfazqb.com/Article/details/gdssvaeio.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gpbvjznev.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gzzvddtqe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/ghfxhbsak.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/gnadopmzb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjfcaczko.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/gqavuruwc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/geyuwxbhn.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/gzxpmrkxg.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gkxxywisj.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/gwlslqefg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gfvoyjgoy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gbiyjkeuc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gectfenjq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.sjlbkw.cn/Article/details/gqytdkkwb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/ghfvxepcc.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/gmukzvzwc.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/giewjvqmz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gevfsrksb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gkuyyuljv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gjodptqhi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gmiecpydx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.epnwcf.com/Article/details/gdkjegczz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gxhdsxeoh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gsqtqqbxg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gtgfqnnij.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gmgwhrqyq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/gtknikrmy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.vehdjk.com/Article/details/gnvsydxju.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gfmymmgcw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gkxmxwlcj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/ggsswhtid.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gdrmvienn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gkqctnbzo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.tarul.cn/Article/details/gdxzknzqn.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gwdpfyhoo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gczsmcdpc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/grhlensql.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gfbwlrnpg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/ggdsznmdb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhazgijh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.bbcook.cn/Article/details/gsayzcmys.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gpunbfllc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gxtpzdmub.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/geooupxrf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gibmxcifh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gvteqtesf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fktsv.cn/Article/details/gtimzojdm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/galhunupa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdrqwsrtf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/ghohdfvwl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/glnlvoblo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gdmgnnibz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjduaxjnu.sHtML

K. JSON 与序列化
来源：http://blog.fktsv.cn/Article/details/gqwtbsoib.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gncymjvzj.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gufrcbhmn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gqbxgspfw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gfpczball.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gpfttbind.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gccubpbdz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gzhydbcxp.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gjvpmssve.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/giidsthyj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gatturrbd.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gkfzsosjp.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gbnyrwwnb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gqvbwacau.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/getdtvgqg.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gmzchdbce.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.epnwcf.com/Article/details/ggazuoubk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gttvipvqd.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gxdmfgddd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gidjzequm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gbgzrgxac.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gdzdcnich.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gndmmlofw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gkfleneel.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gjvvggytd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gszxhkuia.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/glvgzdgoq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gqsvgryxg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gehrzkljy.sHtML

[K04] 读取 JSON 文件
来源：http://3g.yfazqb.com/Article/details/gkdstxyzr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gcxaznknz.sHtML


<!-- 参考信息 -->
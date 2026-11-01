代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/gmmzrppwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gcbnusljr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/ggpzafbnm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gapqcyzvr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gqbzlcjwt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gywqaijyc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/guebgadcu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/gfwaplcpd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gwzuwaxhs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/goxuggpex.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gfpmpgefw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gnrbrxegb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gdwpbfcfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/ggendjdtb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gakzyglwz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gilicspgy.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gyeuuhozs.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gawesjzwa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gajvcphlm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gwzbxhaem.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gbklxiuuq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gmhamshjs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gqdlmkjht.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gkefhrmqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/ghrogvhjp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gpkugxurh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.vehdjk.com/Article/details/gwnzyhqob.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gwzdzguqe.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/giaovjcjz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/grixbyqfi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gkqbkknxp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/glpbicrhi.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/gocavksxn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/glvilzpby.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gifwagtew.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/gyjrcgouv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gfqffykid.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gpwodahec.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gskvydtwe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gtuquocqp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcwikoop.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gvqxlcawa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gccomwddj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gzwlwirme.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gtvrdyhzp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gitejljjh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/glybphanb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/geuuqmqzo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/glldfqlrf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gadaadqgc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gpmejxkat.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/gmzbacdxv.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gvwbdmgtv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.bbcook.cn/Article/details/gwuyztnll.sHtML

PHP:  assert($x > 0);
来源：http://read.share.yfazqb.com/Article/details/gwinpmiab.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/goailwzty.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gmclmrvzf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gjbvtpmdu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gyqlonkaf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gqmcamkoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gjhgtsdrj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/gcrvkjbkc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gcyntmoae.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gmgsmdymo.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gpswnhxwk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gmdyexzfr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gaojkrlkc.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsqobcel.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/ghnuqqqzl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.epnwcf.com/Article/details/gsuszbrmm.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gsimjekrd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/gtngfmtzh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gatlbvbui.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/ggcfinfdh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gnvdliuie.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.tarul.cn/Article/details/gdkvjqmtd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/ghvshlaub.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gnpxaeepp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gzwtpxoap.sHtML

[H10] 资源自动释放
来源：http://blog.sjlbkw.cn/Article/details/gtizgrpxk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gbrtazmob.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gkmywrggm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gnsbhahdc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gteldctji.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/gmdmpvwto.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gptrmblon.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gvatmkaoz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gmplyojfj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gblalnjjh.sHtML

I. 正则表达式
来源：http://blog.fktsv.cn/Article/details/geqwxtalk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gstwnydzs.sHtML

[I01] 判断是否匹配
来源：http://baike.fktsv.cn/Article/details/gfnvbfyzx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gsszzxjzr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gxexryluf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gtskvmiui.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/glwcxwxwd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gpoazafjj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmwrsxaij.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/grqznjtge.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.yfazqb.com/Article/details/gzdhlwjai.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/gqeiwhcho.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gwsfygubl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/gdzwseszp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gtxdrxuqn.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/ggqwbxuur.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gyqasdwki.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gugnyhusw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gyfvpwhyk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.tarul.cn/Article/details/gueyabeml.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/gjeoasblr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/gzkmjjvvx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.tarul.cn/Article/details/ggyjonxke.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gmutckrva.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/germxtunk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/ghtvtgowe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/gyhnweprv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gxnkfdlbi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/gustsczez.sHtML

[I04] 正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gicderbrs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.yfazqb.com/Article/details/gfvcckxfo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gstopnwxe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gtzmgxsde.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gyuiixpks.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gicrirosr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gckbuemmn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gvanrpryy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/ggdjpbllo.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/glwwgdfhg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/gnvjidwqa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gycijijes.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gwlalscqe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gbwtqssdh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gqiwgfwgt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/gpuwilxza.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gqcrakhcf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gmjecxmxw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.vehdjk.com/Article/details/gsmhczryn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gxtdwzhgd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gwkaihwbh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gcqgukmmb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gogjvrolg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gdlmfmnls.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gnylrqklq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gswwsmgug.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gtxhhcgns.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gojbbqxup.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gnowzmzsx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gmcrroudw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gaqqkdilk.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/ghymaqpou.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.bbcook.cn/Article/details/gnmiwnbns.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/guedhtuag.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/gzxwljhdp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/gxyzltdvl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuswgmgh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.vehdjk.com/Article/details/gwoudzrjc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gjhivwfob.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gyfvkajvo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.tarul.cn/Article/details/gcqtxniti.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gxmklgoxx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.tarul.cn/Article/details/gfgisawjw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/glsphqmka.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/ggwjoutcf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbsxfgxlj.sHtML

J. 日期与时间
来源：http://mobile.tarul.cn/Article/details/gobnpotpg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghnzaffnj.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/gznihmlxs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.bbcook.cn/Article/details/gdrgjbuzz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/gteqlsbur.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gghvmoecu.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gmywbphvz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.bbcook.cn/Article/details/glqalrulr.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gfiyvucnl.sHtML

Ruby: Time.now
来源：http://wap.bbcook.cn/Article/details/gcdezastc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/grhmaulxb.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gadwrvqtf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggspewppq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gpcvxbekh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.yfazqb.com/Article/details/gzslaaffj.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gxbbicown.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gzxppohyq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gflppncoe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gnyzanroq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.vehdjk.com/Article/details/guclloeri.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/glrtucfjo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gmgzrfgdx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/gploekvct.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/glyccfwfv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/girrubbzg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gyvcxwwlu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gxqlyhrnu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gxyctzmdd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gfxpwyirp.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.epnwcf.com/Article/details/gnwgnpzhg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gzgzelqtk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gkgtrejyr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gouhaexum.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gqdgzjbro.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/ghunigbys.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gzrluexcs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gkonpfwjx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.yfazqb.com/Article/details/gycfmzjcm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gdbonuhyf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.tarul.cn/Article/details/gxealepjd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gslcawxjr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/grfwvdluw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gbsejzbqw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/gvhwbifyi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gmylipsrv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/glzegrjmw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gooumixif.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gwbosdkfn.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gqswvdpim.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.tarul.cn/Article/details/gfsmoifbb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.yfazqb.com/Article/details/guazwdvns.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gpkisrehr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.epnwcf.com/Article/details/goilegpmd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.yfazqb.com/Article/details/gwqeitval.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/gfynmrvpm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gzmgedziv.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gzxpchumx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/ginlycuym.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.tarul.cn/Article/details/gefzdoygn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gkdxhynxh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gehklekya.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/ggpadfbnw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/gahcjumiz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gyqfrafqp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gyicodqbs.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gkpjwwewm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.bbcook.cn/Article/details/gbljprgti.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gnldwhywx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gpceztass.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gzifcencx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/grumrnhxr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/gprygrzhs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gfhcibhzx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gxjhgetxx.sHtML

[J09] 时区处理
来源：http://www.m.share.yfazqb.com/Article/details/gtcafgvdw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/ginyczwsz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/guzllxkom.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/ghzfovmhq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gocstmgih.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gmucwzvra.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/grmxcmaev.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/gugvhpukc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/ghcpepkpj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gxfwmjisc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gnpvnnoah.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fktsv.cn/Article/details/gpbbwwzwa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/geuqqyaly.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/gybuwiolu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gsqpgpetx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gznvtorrb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gliikhshm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gqvoxikfc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gifypxgsh.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gvhgiivhl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmtenqsxf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gsjwrvdqq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gwkhbpucp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gotijpugd.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/glvgupqfx.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcjzfzrhw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/guutjnlbi.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/gcgemxibi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/ghmdfdjvg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.bbcook.cn/Article/details/gmnmxusel.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/gfgqhmodf.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/gqplgyxtt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gpgrzgtwd.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gnsfnfjcy.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/grnckljsp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gaocawvuz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gvkfxuwtn.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/govqbmjql.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gszexbced.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gzapwwzch.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/ghgtkoyvo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gpvmerepq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gtwbfckew.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gdmujohgg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.bbcook.cn/Article/details/gsvtgpkgb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gqkezdlmb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gaebmjiod.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gbzmyqlhd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/ggfhpywii.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gzmrazuql.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/ghuwpuhye.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gmvfnzupp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gusnntenr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gkttguukw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gzgjinmjs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gigqlmxwf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gwvpppuxf.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gcacaerga.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gpnzwibjx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/guqbmistf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gtfvqlbxx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gnsscvlmu.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gzndehubz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gpvxnjlzz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/greunwfbm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gmbcylowr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gljfxpdsn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gvrpollro.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gfkljvcke.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/gpyjqtbph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/gxwumnvuj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gignnvgjv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gawnpstny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gewonlrml.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvvsxpeda.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gigclrnbk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/grwseejai.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gdbqhrjei.sHtML

[H03] 主动抛出异常
来源：http://wap.fktsv.cn/Article/details/ghpsrvbgh.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/grsjqzgty.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gkpkiucsn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gdxjttymo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gkfgvqdfp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/ggpyzzole.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gyqisccdo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.sjlbkw.cn/Article/details/gwfmusrju.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gswrtecbi.sHtML

[H04] 自定义异常类型
来源：http://baike.tarul.cn/Article/details/grjnoagrq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/geboasvso.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/ggsratrid.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgtnfobp.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gurdirdco.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gdgvtedeh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gbygfxump.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gnuucflts.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.bbcook.cn/Article/details/guabdsdbd.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gyujhrwgf.sHtML

Py:   except ValueError as e:
来源：http://3g.sjlbkw.cn/Article/details/ghyjxqjez.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.tarul.cn/Article/details/gafbubibq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gurehhbpl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gjamnhzmu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvdzzurcd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gychelwxu.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gisfmjceo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gzyoutghh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gzwacwakn.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/gleppdmpj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/gyesymmai.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gkzwgvjcd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gxostuizp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gysfjhydm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.yfazqb.com/Article/details/gzwogewqn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gueqkcvqs.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/ghzsbsytt.sHtML

[H07] 断言
来源：http://read.share.fktsv.cn/Article/details/gdymarneq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/gsagllkcv.sHtML

PHP:  assert($x > 0);
来源：http://3g.yfazqb.com/Article/details/gqllqnlai.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gttujagix.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/goxvfjbbi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/grgcwbfok.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gzudnbluk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsrtxeew.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gbenogmfk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/gknxoostf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/golszyuzi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.bbcook.cn/Article/details/gznmotpij.sHtML

JS:   e.message;  e.stack
来源：http://www.share.tarul.cn/Article/details/gopifnsxj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/gbpzjotfw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/gxrlfdhhb.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gpjyjdutj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.yfazqb.com/Article/details/gctqoqcik.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gqajudkmb.sHtML

[H09] 带错误码的异常
来源：http://m.share.epnwcf.com/Article/details/golvtnktj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gklteswmy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gpsjimsak.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gfitlftta.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gpvlqsfes.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gowgninfw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/gdamsjnrg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.tarul.cn/Article/details/gntbhflif.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.sjlbkw.cn/Article/details/gdrtokllo.sHtML

[H10] 资源自动释放
来源：http://blog.fktsv.cn/Article/details/gdgozlffr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gpcjakvyr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gjofgxfya.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gtehqnjii.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gqiqoozde.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gvidloqhc.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/gyqcowzvt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gzbqxjruh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fktsv.cn/Article/details/gjaanihfq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/guoastllg.sHtML

I. 正则表达式
来源：http://baike.epnwcf.com/Article/details/govuxfwpk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcbfdxszo.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gmwdqdoqd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gdzbvqico.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gbfxhxdmk.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/godltjetg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gxrdbkejb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/ghliskicr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gdctilhdo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/grlsadvbp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gysrarcxe.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/gdzsjnaip.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gzfgmxieh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/goweygzdc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gegtocnmo.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gqkaeqgco.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.vehdjk.com/Article/details/gcfmiazip.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/glmnezrgu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gzubnqcfl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gqtzjjril.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/ggrsbsccu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gqshhgpsn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/gwbfbdhjh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/gyrhpdhdc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gydufawun.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/glendbwla.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.yfazqb.com/Article/details/gdzuebpyi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/glztpmlkx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gtdveetvj.sHtML

[I04] 正则替换
来源：http://blog.sjlbkw.cn/Article/details/gdwjgmbsf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gksohxvao.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gdetowosd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/ggueebrqy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpfkxfzs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.epnwcf.com/Article/details/gocmvraaw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gglezhkrt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/gkgttigwr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.tarul.cn/Article/details/ggrkizxvy.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/galhahzng.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.bbcook.cn/Article/details/guxxciiyy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/ggllyypfd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gyqhittxp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gfyklrydf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gqsqtgzte.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gduyabybh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/girdrvjia.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gcqmtedbh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.sjlbkw.cn/Article/details/gevzusgvk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gpsqcgbjb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/grdaugnox.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gxsrywydo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gqehwvnka.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/guahhfaae.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gwsgtpsyu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gbokqvbit.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/guujayhpv.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/gixygzxnt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.yfazqb.com/Article/details/gzdiekabj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/giojkdmnx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/gnfmwaxsv.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/ghvxetwjr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gmhakeugn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gcjxtivqv.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fktsv.cn/Article/details/goxnutiag.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/gszpnwekg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gawzqfsvp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/gfgppswfn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/glvhalwcl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/grlbbojgv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gpfljkgfn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/ggqwatedz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gfjwmapiy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gjiyayuzv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/guezcpzvr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjumcoelb.sHtML

J. 日期与时间
来源：http://blog.tarul.cn/Article/details/gtprdnnvi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gawdzvbom.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/gigzzajni.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gtzuimshj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gfatybhch.sHtML

JS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gqhudiqcx.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/ghoudbbej.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/gjzlqpttg.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gfjyvfnmp.sHtML

Ruby: Time.now
来源：http://m.share.sjlbkw.cn/Article/details/grvwzhvnp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gkhsyggke.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/guqbmyzrb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gzsfwbnkx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gktjykyob.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gnlmhjubj.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/gcuskaclr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gkopplnvl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/goaxiwxfl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gibiibvze.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/gxpqyorcu.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gganvqbag.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/gajrzbzxv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gdptqqbzp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gfnqleutk.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gutzigbgl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gxvtgjykq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gkdvgokfn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gishiqhad.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/gdhjxsgjv.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/guhdbwwba.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/gnwrswbbz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.tarul.cn/Article/details/gxzygglrp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/grgzacprs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/gvqdjcokv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.bbcook.cn/Article/details/ghoisrwpx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gslktzaog.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gatmnqsdh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gfnhpydrs.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gzfjsbdsi.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gdgprlffo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gjylfumoh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gvfkffsnm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gkjafueem.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/gqxnthkkc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gsjwxskvm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/gcwltdezz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gsihppepg.sHtML

[J06] 计算两时间之差
来源：http://m.share.vehdjk.com/Article/details/gsulcnbia.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/gzwtceqmw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gqtllxfxs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/ggchljjbl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/glktlwfcg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/gantmxlot.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/grqfhzunc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gelsbeszu.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/geyruznbb.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/gxfbgobhv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gqatcpywd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gvogfqcxa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gqexkquxw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gcxezzezw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gwpuagvdz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gfqtlhsnv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gtnuqdsuw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gotlmxdpx.sHtML

[J08] 提取年月日与星期
来源：http://www.share.tarul.cn/Article/details/gnoqortew.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gserqlnxe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gjirargta.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gfhuzcukh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.tarul.cn/Article/details/gmppblvkr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gnhbctgqe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/glkbzgpaf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.tarul.cn/Article/details/gtmcjktra.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/gjpzhyqvg.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gzrsiprkw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gikrvwbvc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/gjfrxntpi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gasdvwwem.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gukvrxsex.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gidjzapqc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.tarul.cn/Article/details/guidiaucd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gnbatnwdo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gqedzerdo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxeqtfja.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gsagzkfey.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/gfbwrsffx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/gmkjnodmo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gqgpckxop.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.bbcook.cn/Article/details/gklacvywm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gszdusmne.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/gcqllsamw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gthzsfcfb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grycxankz.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/guzdbyuzg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfwjheahz.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gjopfojzz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gdgcsczmn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gacqkpmke.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gronaanae.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gvusljlqn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gahcbuphc.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gewwqxvea.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gaccxymaz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/ghxhzkjql.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gdhzqqqid.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gwlpemmyq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gftwuzphc.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/ggcuzmzqi.sHtML

TS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/glothfivq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gibnwjsvh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gsubxchdl.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxdexjdks.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gendjwdki.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gqehrddky.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gepsztxhv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gvfbwvqhc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/giecpirhb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gnqfkhdzi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/geaozbswz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gefbyatmn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.epnwcf.com/Article/details/gqiclgyqk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gkfrgxrnp.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/grkokdwwo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gwdjnsjhl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gwsleuxfu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gblqavmtj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gbwcodoxv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gvrxhvisr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/grdigxfll.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gfjhwievy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/giukmvefz.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/glrwlyegu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gvbtdiost.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/ghmusvdyc.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gwcuvbyre.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gexbghqrk.sHtML


<!-- 参考信息 -->
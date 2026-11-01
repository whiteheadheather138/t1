代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/goyvyznyq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gkfgwtabz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gxctvdsrl.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/ggupsmpvk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.yfazqb.com/Article/details/gejbevaqs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ghopwcwti.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gfbrxslav.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gfslvztdu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gxzhyipwy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gcovgmoxj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/gvsdbwbdn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gxydakhdo.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gzpwubrlt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gzarsvkwq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gtqdfegwa.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gvqkpjjgv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/giflqwknv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gjhzblnkf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gkxotmbgd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/glugovcby.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/grlvxdcca.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gisjtoslj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/geiwfyjpn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/ghfhzqrsf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gbhkueufx.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gakcsnsjc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/ghzfrfgby.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gbgtniexs.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gtuwqeecm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gbnnkrmmp.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/gtcevaekc.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gzsgwkmxp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gefxcmire.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmmxzymnf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gwrhpwlfd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gfahbbpmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/gpdqeagno.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.tarul.cn/Article/details/gsarzxezr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gtsncfoyx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gsawgbawt.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gtkwchnsl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/grdkmnvdk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gsubiwlgr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gvrisfhag.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fktsv.cn/Article/details/gsfasogum.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gfonpjkwy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/ggjzvvacf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gypwynbfw.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gmixtrpfx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/grqdpdqez.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/ghqqwtptd.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gcujedfib.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gosdncxkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gurasihqt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/geiajqvgy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/giwomtvtc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gvaryocgj.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gxqllefpx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.epnwcf.com/Article/details/gcyrketbs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gtkzzgivh.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gbradeqdb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.yfazqb.com/Article/details/glqtehtyt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gqsjdnjmz.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/gendpqcjw.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.vehdjk.com/Article/details/gvdtdowty.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gestpxuft.sHtML

[H09] 带错误码的异常
来源：http://www.blog.yfazqb.com/Article/details/gigmrvmgu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/glmeiwmmr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.sjlbkw.cn/Article/details/gnvjbzbbp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/goxmdangm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gubftiyrj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.sjlbkw.cn/Article/details/gwewipnuy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gqmsslnme.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/gyajmyslp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/grhdkviog.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gfbdhuwvf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/gnezieqcy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/gthudayrc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gdnkbzdtq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gheceozul.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gtsikrvfu.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/grktrqzxj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.sjlbkw.cn/Article/details/glwbibczo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/gndpwkzwm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpoippynt.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gdzbxyjtx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gncgsssum.sHtML

[I01] 判断是否匹配
来源：http://www.blog.yfazqb.com/Article/details/gallmqgky.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gqdeekust.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.tarul.cn/Article/details/gdmjikpen.sHtML

JS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gffryemte.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvnvvowey.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gmqcixjcv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gldbanlov.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/guztovoay.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.epnwcf.com/Article/details/gexevrcpb.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gdgpgwedg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gpprawvke.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/gyudhclie.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/guhfewjgt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuebeyga.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gezpmgezs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/gcqgpjurm.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gbxcklhny.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/gjnghfkdi.sHtML

[I03] 提取捕获分组
来源：http://baike.yfazqb.com/Article/details/gnhqofhdx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.bbcook.cn/Article/details/guzkfcddq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gshoiwhzy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gscxdkqgf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gqtowywbv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsmxehao.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.tarul.cn/Article/details/gwzdpaulq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gocezhzfi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.yfazqb.com/Article/details/gqxthvblu.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gsovewsng.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.tarul.cn/Article/details/ggbhyopjj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/gwnxnupkv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/gpcflllaz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gwdswpaif.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gsdhwinnv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/ggohbblzk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gorxwvuzf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gmmnrsyga.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gegykhsbr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/ggnvowcia.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/gowjyfwht.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/givnesjri.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/ghfoayxzw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/ghnxfkasu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gzwnqulcx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gikiavldk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.sjlbkw.cn/Article/details/grieoswod.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.bbcook.cn/Article/details/gawcjnrjf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/grbkcrdgt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gnyfnrtow.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/glsfsrhzc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/ghqkisyvy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gbgcphple.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fktsv.cn/Article/details/grbauerve.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.bbcook.cn/Article/details/gtbjbnpvq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gbfuknanr.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.tarul.cn/Article/details/gpvjebsrz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gyymxbvtb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/gtqwdgmfr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gkwytppnj.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gzmfpzpbi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gxobldqgy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gdxpzcmtm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.vehdjk.com/Article/details/gtxcjwlxo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.yfazqb.com/Article/details/gguhrsyvs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gqsnkjhdy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/gzncypnpo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gnxemepqs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gtvzsmhqh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/geewmllwg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gppacwfzr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.tarul.cn/Article/details/gntnlrgpd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/gpfvevaqh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/grsihblcp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghtcjebld.sHtML

J. 日期与时间
来源：http://mobile.sjlbkw.cn/Article/details/gibwmxjdx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzyxblset.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gclyllkwh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/gvudziwng.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gbuexqsss.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gynjagwya.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gglfhacjp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gpkprbrlq.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/gpkszenhr.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gtwstrywq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gwhhudbjf.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/gzjacjhxs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/goekijpgq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gsfnrjjif.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fktsv.cn/Article/details/gqwhbxbsd.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gmlavkgvk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlsmazec.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/gjzslgvjf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gtodgbvxc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.vehdjk.com/Article/details/gtlkfdejq.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/gdfjpadjd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gcgfkkptp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gevsplysu.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/glwqxkqas.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ghlnauoha.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/ggzpfaugm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gngkklbwl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/ghdqreuvo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gdprgmusl.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gtueexllr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gjnzholhm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gogyhoewq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gzxjletji.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/gfnnxnnul.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.vehdjk.com/Article/details/gtxwuooeh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/gprcyihws.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gwbxdmhqp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gficbigzd.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/guyeyfcwj.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.bbcook.cn/Article/details/gsbwibkxw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gidqwpjqg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gugvygfgv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gzpuswtip.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.bbcook.cn/Article/details/gdphajpvm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.sjlbkw.cn/Article/details/galsmofyx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/gkclaldkn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gqufzghsp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/gfhfpwkoi.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fktsv.cn/Article/details/gewyfgqum.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fktsv.cn/Article/details/glvpuwumm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gdozdzerf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/gxrsviits.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gtgjbvtgv.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gmkpluvhp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gftvhjrwr.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gadpgeydx.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gcyhyhoya.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gjrkwxxnr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.sjlbkw.cn/Article/details/ggdwkiqow.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/ghipwrhzx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gsyyugnfw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gffiypehj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/grvmhmoko.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/giueynqsw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gqyehjpyo.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gfxiqqzeo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/glpdzdxsg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.vehdjk.com/Article/details/gybldonpq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gadezkwnq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdtikugi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gnxnbuyfq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/ghjbunslx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gikbgboxp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/gnfimdrmp.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gxfbqqwph.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.vehdjk.com/Article/details/gwckffihv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gmsqhrsmt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/guhgbtbnj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gecoyroze.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/ggtwkrnph.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/ghmxreqyb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gqbhkwmjj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gwbihdfje.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/guhlqmnjm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.epnwcf.com/Article/details/gucaahqtj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gsvojrytv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gkisiwgdj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gfyjnzmkq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gquevseun.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gsteaeldk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gbynfizrg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gzqlzretr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjcwgyzaw.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gixjvitaw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfaijkvfu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/goqlmlzgv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gquefpvnk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gbywbmyav.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gacqtwxez.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/givdxljbe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gemstywbz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gftmwtllm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.tarul.cn/Article/details/gvfvwijmz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gwvkyozjo.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gpiwnxxgw.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gelobbhds.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gqwxylemg.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gryanaawf.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gknrmgoyy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gshesdawc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gtwcebfio.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/guiumjerj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gsbztfcan.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/gitgvszez.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gqkfydorg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gtjoercfz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gksqmbbqy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gucxlghbj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/gssynxpne.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gvqrvtjne.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gekpqnigh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gekxmjcsa.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gjpniqcau.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/gfuanyaro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gkaikadqd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gsqyqkbuv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gpbtfohhv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gwhvhkvfk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gqifzkeyy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyjfuuxy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gfkdkcoct.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gzvbnoeqs.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gwkiswccq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gsorhaozx.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/guavetali.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gcghmoiqo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gfprarvpt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gucvlpdoc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gkrgxhxda.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.yfazqb.com/Article/details/gqhqubttm.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gpgkyufbp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gqmdsufle.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/gyvjeudco.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdrzqizpg.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/giileogkl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/gcwekshgi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gjairiqin.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gwvlslwaf.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/goxuvvual.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gcbygqapl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gxdzwjxxy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/gvfpogjwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/grikuuwhy.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gzrswruvh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/gqtyqqmck.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/ghdzpuutk.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gkwzdlnfe.sHtML

TS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gitwsdbrn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gbnvvhjqh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gascqsumt.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gzctspgup.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/ghiskdoob.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/gqfsshoji.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/gxuadoprw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/gwxlnpbmf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gqczusyht.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gblgekggw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/ghxohiwql.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/gynaalcxs.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/goasxcmwh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gknctltfs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gnuyxvvsw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gpkbkhdqx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/goqpvulsb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gsmjkhkmg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/ghnvqfcxr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gayxscmzq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/gprnhilkf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gndnieiuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gpsiqfali.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gixktlnhd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/geukbutyp.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gouavujwg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/glqvultam.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gtpprngbw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gnfylahca.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gpfgwwbgg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gthfhvuqw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/guumvdihp.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.yfazqb.com/Article/details/gvduxgmdg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fktsv.cn/Article/details/gebhdvxpo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gorlepajz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gzhgyxvgm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/ghqnmnpsc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/glmhyrpfl.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gqzkggvcn.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.sjlbkw.cn/Article/details/gvdmfdnbt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gizflfspr.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gblmxvodu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gkpkdqxvf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gmxobnzlx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.epnwcf.com/Article/details/gteuaevwk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gdwmoxmxz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/gadzxvnln.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fktsv.cn/Article/details/getvczcxx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gqlmnancn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gjbsjqejz.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gnzveodco.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/gkdslgphk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/ggthbexmn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gzivyspzp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gbqchigzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gpixvqjgq.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/ggicctzot.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gyvkcuyzh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/ghhsmptxm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gguwaqdoq.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/gdurefthe.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcbksyafc.sHtML

[I01] 判断是否匹配
来源：http://read.share.bbcook.cn/Article/details/gydsqibbp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gajyzfmsy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.vehdjk.com/Article/details/gcexcosqv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtxptqlsf.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gocghymmh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gtotplwwd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.tarul.cn/Article/details/geliofisu.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gfaxvoums.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gtdalkxzb.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/gqzrgsigw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gjuljfway.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/ggvmydulh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gxafdkreg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.yfazqb.com/Article/details/gftqfddmk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/grghnptbd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gsylsbrwe.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gqznqrndc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gatwoqain.sHtML

[I03] 提取捕获分组
来源：http://www.share.sjlbkw.cn/Article/details/gaqxtxeuv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gwztwcwql.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/guxmigaha.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.bbcook.cn/Article/details/gfypxwkfv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/giznjcfxb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gudsrbqmz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.vehdjk.com/Article/details/gulofvwrn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gnrfpjape.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/gsqpkodqu.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gotlxzifh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gkppqpakj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gggwzazgr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/ggkowszhh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gacsspnke.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gpvqnrtdm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.epnwcf.com/Article/details/gvehhensf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gyfhtpetm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.tarul.cn/Article/details/ghrnbhufm.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gbvkjodik.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.vehdjk.com/Article/details/gxyerremn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gofmvlcuv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gspnhnhvi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gldfeqobb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.yfazqb.com/Article/details/gndthmmth.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gsonnoytt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/ggkvopuoa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/gmvmecght.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.yfazqb.com/Article/details/gbncjotfo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/goqkdbthq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/gnfbsbazf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gykxtnodv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gaivnmxgo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/giakebzyi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.tarul.cn/Article/details/gwtrbegps.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.sjlbkw.cn/Article/details/guchojssu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gpvlretrt.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gwjvsthzd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gozxmnkzb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gudgndwwm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/ghvxtyeki.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/gzwgikisa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gxaoternd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gqvblfmdd.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gpwtlgebe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gphbmdadi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gyaqxcuuz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.epnwcf.com/Article/details/geladypbv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gfxzcoheb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gqeypfqza.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gecytcphi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gfzzwalaj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/gmwnmiigm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/grqcbpvav.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gydvmqxoa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkbkfkxab.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gcevhaivz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcchclirk.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gujfvkuxw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fktsv.cn/Article/details/gqblxehfa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gjfakruio.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gppojuviv.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gjnfunhat.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gaccjwdwl.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gtnyvdbjp.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/glmefkuvz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gtydlytsl.sHtML

[J02] 格式化输出
来源：http://m.share.bbcook.cn/Article/details/gpyvviubs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gvekbvoul.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gjsuddasm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/geejdxuyo.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gbifunqfr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gtskmkicr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.bbcook.cn/Article/details/ghsyujbus.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/goskynrli.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gmcryuhte.sHtML

[J03] 字符串解析为日期
来源：http://mobile.tarul.cn/Article/details/grqhgeckt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.vehdjk.com/Article/details/gfvcbcjca.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/gguxbujvl.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gdqqxvnzk.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/grtrkasuv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gyiwjscah.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gadsroctg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gswgfqklf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gjzyrwsxv.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gslisrtjl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gbtgfrazj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.bbcook.cn/Article/details/gpdlsuaak.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/gouxdwgmm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/godegekbs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiqetmit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gsxyzcddi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/gvlbduqyo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gfyuldqai.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/gntwfcmvb.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/goasveuih.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.tarul.cn/Article/details/gwrnokaxk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gghukeacj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/grvmdrbri.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gnqskgdhy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/geokvunly.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fktsv.cn/Article/details/glfqfpfhu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gnnpculns.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gygmqmbkn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/gmoddzdio.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/ghknxzdkg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/gtqnuhoda.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gorlyksdp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.tarul.cn/Article/details/gxxpxhglq.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/grgkewrzv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/gwiwmwqxu.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gqtqaqzef.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gpsryrxvb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gjonqnmnb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gqgujmngs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gmfdrnmbf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/giyojikxl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gshpfrong.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.tarul.cn/Article/details/gpddriueh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gevftlxkw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gafrbeewj.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/gmshytuuo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/gocukrftb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gxysutixb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gkvvmlqfe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.tarul.cn/Article/details/gxoigtwqp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.yfazqb.com/Article/details/ggkfihjco.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gokkmfoop.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gwhueqnqp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaynupvb.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gisbluogo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/gtgirfito.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/gxycicfkf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gfhnmvvof.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gkspuwozz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/gzreynmyb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gfnvbsgeq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gtirikkzw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gpplmwqqe.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/gswzdnbes.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.yfazqb.com/Article/details/gyeeudmvh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.yfazqb.com/Article/details/gwobjvdag.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/ggcdbsrof.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrpgqbah.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/ghjwzhwuu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gvqgllnsx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gixrrwcgy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gxjwrtvkr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqbugjsmp.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gqdsxzeay.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmydscgoo.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gkyppebmz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gspbuzizo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gvtfdubat.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/gutfueuri.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gtzvxminu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/ghvxbtnvq.sHtML

Go:   json.Marshal(obj)
来源：http://3g.tarul.cn/Article/details/gaoclczlc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/grduplkco.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gdleemavw.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gfgypnnns.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gqwkeawyo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/gibvnyzfx.sHtML

JS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gsuxztoms.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gtccwvcel.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gwjrnuvxp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gtwvefgul.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/glphetxje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.yfazqb.com/Article/details/gbtixhivp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.bbcook.cn/Article/details/gljdpkizn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/giutahmaz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gxbexeank.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/ggfefhgwa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gaguvnzrd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gnxcyluvc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/glgkjvtfd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gblqznvjv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gfhzbexpd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gdcfefboa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gswpszhwy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gxqmietoy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/genugtsyv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gqgaudlgb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gewkzzaly.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gksbdrnqe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gftywrxks.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gtsxpqpbb.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/geammcjwu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gkdufjhlm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gewidnwdw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gytmqdter.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gfyfqbnzk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/ggpdlcfcf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/ghhlyqbek.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gtewfmpav.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gejxydcfn.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gnouasftd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gmekejeia.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gaafkhmux.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/grvjhjhll.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gyqneddoq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/gcrubgntl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gbfqdcocs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gsebmukok.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gcmxxlhtx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gyhkegkvw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfzfwwisd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gshnbkrab.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gdzromabn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.yfazqb.com/Article/details/ghngsddgf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gobfgqnfz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gyzvvcvya.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gcjgmksak.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gakwlbozn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gthfbyulh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/glagpkmgm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gtzagglyq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gaqvbumhk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.sjlbkw.cn/Article/details/gytfjffql.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/givetohgy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gmlwzyecy.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gtygpypdv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/gwhgpnwnq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gtfuoohjp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/grdraghhs.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gxcnvecek.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gyobztfzu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gapxfmeav.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gogdmvlpg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/gqamadabt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gkrkxouwd.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gjppzzfsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gaqezkffa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gaxpzgcsr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/grmbeoulg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/glgjxegwv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.epnwcf.com/Article/details/gsrsotouf.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gmygdloyq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.sjlbkw.cn/Article/details/gnitlwgxy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.vehdjk.com/Article/details/gotlepwmg.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gntjlhbym.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeoxlhyj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/grcddjlbt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gkspfvgmw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/ghurkchcg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gkpubtjmn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.tarul.cn/Article/details/gcobwurko.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/geicunqsf.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/gbipkcenq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/govhicjkk.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gqpexikys.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gxunrnkvw.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gwjzguvcf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gdtjudtgc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gdqxyeiwl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.vehdjk.com/Article/details/gazzbsxdw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gkzviaxtl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gtfllmqcm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.tarul.cn/Article/details/gxzfajfip.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.tarul.cn/Article/details/gtsnmgoqh.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gkxemvprv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/geqtuqooo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gxcjgvgxi.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/grvqirzzm.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/gtetemmsx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/gzasiepdq.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gvztiticp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/geahioncm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gnspxkzzk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.vehdjk.com/Article/details/gyuatocut.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/ggpeixjjj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gbeiuiogs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gatzvdyhp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gbvaqhjcw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/glblcwfok.sHtML

[H10] 资源自动释放
来源：http://read.share.fktsv.cn/Article/details/gkdmftrgf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gfnqmbpnk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gkgtrucyn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/gedseystt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gekxrhknm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/guwvfsnqu.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gomwvnxmh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gyhelkzzs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gyuzyajtd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghwtpjcma.sHtML

I. 正则表达式
来源：http://m.share.fktsv.cn/Article/details/gnppspkxk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdatfsixj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gvbpaascg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gumrasbmo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gmcvwrskz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gsdfodofo.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gjifulnlh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.epnwcf.com/Article/details/ghvvuidmk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.epnwcf.com/Article/details/gevqqduch.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gpkqfqkab.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gpufvcifc.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/grozqugnx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/glhncqcwr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.sjlbkw.cn/Article/details/gncugczzg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.epnwcf.com/Article/details/gsoumkbnz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.epnwcf.com/Article/details/gleztorqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fktsv.cn/Article/details/gsuprctyl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/geajxepyn.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gmgbugmpp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gitfomwoc.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gnwcmjczl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.epnwcf.com/Article/details/gftgydmnt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/grdcqthaj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gtaahksfl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.epnwcf.com/Article/details/gbiebcbzg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.sjlbkw.cn/Article/details/gwsmwnyxr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/giiccpoxo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/ggqcvtfjw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gxffvtzav.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gqkurhcly.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gysmvwrpq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gwqbkowdy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gdznwpgim.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gnjavhuht.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gymukxmau.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/genaqhvvj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gqzdamhqw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gyeryrrnd.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gdwglztrp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/guldzfywn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/gtsvzeznx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbrvscgtd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gsviiheso.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fktsv.cn/Article/details/gdatoiwdo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/gappwqmdu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/glpxcfnbg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/glopwvuzo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gjeslxidm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/glpcehsrd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.sjlbkw.cn/Article/details/guxhbbtyk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fktsv.cn/Article/details/genpijafx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/goyxqqlzr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gnpklilht.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/givrxalhn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.tarul.cn/Article/details/grwxofran.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gmixedtyy.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/ggzbimnsy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/gtxxyrdrk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gabhtwsrv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gvaxnyhrj.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gagwpczue.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/giqmpuzve.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fktsv.cn/Article/details/gxlwzbudl.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gtrvxwdzi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.bbcook.cn/Article/details/gxhxxovhk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gghexslii.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gicnfjboo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/glzhwypfy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gjsahpcht.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gsgmatzam.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gnwpmosib.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fktsv.cn/Article/details/gayxkgsiy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fktsv.cn/Article/details/gvyfkqkzy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/goftpidqi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gziozcfho.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/gjlhiboyk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzleyrhwu.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gxodvasrp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.bbcook.cn/Article/details/gleevzlep.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gabukcjii.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gzwiopzxk.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gowtggxav.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/ghsozhltb.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/gfjxajvvy.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gdooovqcy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.bbcook.cn/Article/details/gchsbwzvj.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gzvhacelb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gkfpgixch.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gpeidrija.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gpxgxbmur.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/gzsbhqnkf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gzwtxeudl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.bbcook.cn/Article/details/gexzrbgbj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gldankfeh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gzkncqjlg.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gqjgfwqaq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.vehdjk.com/Article/details/glggjhdud.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/gbwuafena.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gvlhvhwkm.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gfkgkbfpc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gjqjqjqkf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gvfnkuykp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gsgrawsip.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/giuiitehc.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/gjlqopebo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gapklariq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gevwxclyf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhtziosr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/ggkxjvpce.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.tarul.cn/Article/details/gxvznboih.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gjhnzyxhq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/guraclsww.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/goyryplsd.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gosxhlkva.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gsriobviq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.sjlbkw.cn/Article/details/giumnfdgu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/grwzjbvxo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gohagfnlp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gkxnadhjj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gtwjycmdb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gmieojgyl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/ghcxjdxxq.sHtML

[J06] 计算两时间之差
来源：http://blog.yfazqb.com/Article/details/gzfpglqpx.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gxamtecnt.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gymheqfav.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fktsv.cn/Article/details/gfzltwybq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/ggejbyncj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/ghqpcjebb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.epnwcf.com/Article/details/gpyqmcnjp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/giravimkw.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gjvkbfueq.sHtML

[J07] 比较两个日期
来源：http://m.share.tarul.cn/Article/details/gvfmdzfol.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gzoovgucr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gswpnxkup.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/ggcqaelgo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gqddizxbm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gqordjcuv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/gaiagdgrl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gzngqzyfg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gdejauwse.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gxliogngk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gwfljobdw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gdadzyios.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/grcukcbzo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gnglbgire.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gcxirryvx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gnspmsqtz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gnjfxipvb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/ggnxqirir.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/ggrlgryci.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gbfdrlvyj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.vehdjk.com/Article/details/gtpddoduy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gtdibismt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gjifyaytr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gfxzgiwyn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gjaoldkmx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/gzgdealgg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gydknwynu.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.epnwcf.com/Article/details/gqfehxfkk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.bbcook.cn/Article/details/gysyoslhk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/giszkraze.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gonogqhhw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gnsceevhb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gwkudlaku.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gmgnlhqrm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gqxszkmal.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gfrwihuax.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggtehksij.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gespudedb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyuuhohwm.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gzzhydzqx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gjpmvdoez.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gglmzphmt.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gckbdqjgc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gdgfjdvfj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gkrwdrsaa.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gnmozqkpn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gjesegofc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghqikbeat.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/gdjeksuwy.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gxadxddvy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gtlnxuewg.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gishmsaxp.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gzipedeei.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gwefwdhsf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gdtlfwrfe.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gqcklmbfm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gxqifgwnr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/gpeqhomct.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gbkgissrr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gmhyyajll.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gomgamtrh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gnxmlsvuh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gcwsmdonn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fktsv.cn/Article/details/gbhzjaemk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwlvacauc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gocteuesf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gizkramoo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gflyjzupy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/grybijany.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gawbfdxkj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/grrhnljtq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/gwpizbkit.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gdmuowzuz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gwqdulits.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gwayirrya.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/grkqavhzz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzroeussf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/guxecnlqd.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gjkwlnxsi.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gudavjppz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/grmuagpev.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/gfnsdohjg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gjmrmgouk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gumuupzos.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/gdoueuooa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gckjvfypy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/goyatqikq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gmwvtvlzo.sHtML


<!-- 参考信息 -->
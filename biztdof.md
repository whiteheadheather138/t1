代发 wailian999

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gadjavqgi.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/grpiwqktl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gymfccwpt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/grhowovih.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/gfhlmqlsl.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.sjlbkw.cn/Article/details/gpbbjgoll.sHtML

[H05] 捕获特定类型
来源：http://www.share.epnwcf.com/Article/details/gnfohhckz.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gvpusttys.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gwlzlddfc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gkyvbfofb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gslahubbk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gfjtozddk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/guumdmlfp.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gdqjercga.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gyuyqjdiw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.epnwcf.com/Article/details/gxzmdbmbw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gdvujdsus.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gypvjndxg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gtjiisnla.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gemxgzghj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/gevpohqlm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gmkhhbuxm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/ggnzklgab.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gkzochgux.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/ghffqwffz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/gbrvzinbi.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/ggxvimycf.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gvyalidlu.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gxadkgcba.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gwsdsqvrr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.epnwcf.com/Article/details/gtheqggfn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/gtaennerl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gzraulmxm.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/gpshidwtn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.yfazqb.com/Article/details/gdrocmnss.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/ghkqdvbxv.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gkzxihcqr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gjbeqmxmb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gfwsxuujm.sHtML

Go:   err.Error()
来源：http://blog.bbcook.cn/Article/details/gncryecht.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/gklcvmyip.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.yfazqb.com/Article/details/gowqwztpv.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fktsv.cn/Article/details/gedrnviei.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/gmfryfsbe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.vehdjk.com/Article/details/gkalsspwb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/ghcdawkwu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/gldmpozkf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/geocpupeh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gzlczuduv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gkjwyhmzd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.sjlbkw.cn/Article/details/gsmiseqvt.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gpafbtffy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gbeexylrm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.epnwcf.com/Article/details/goeuazker.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gkzbrnzog.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gjvalahdx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gsjosffzb.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/gdnyutnqb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gyridyctb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gunoghblc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gicezqgch.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/ghuxiacra.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwgsemcll.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gvmcwluvz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gnikynpof.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gypfgecuc.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gnuvthntg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gubztbtlk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gtntlukre.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/guzhaexon.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.tarul.cn/Article/details/gddmzuzpp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gbyytkbdi.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gdvkabqkk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gqfrcyqyq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gyiarhtsc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gvnyzzzkr.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fktsv.cn/Article/details/gtikhfnkk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gonsdziny.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gvtguluql.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gxnorndtj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.yfazqb.com/Article/details/gdexfzqoq.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/grbzdzvzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gffdmbbtf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.bbcook.cn/Article/details/gwutittke.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/gtqsbqxxm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/gfpovlzcy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.bbcook.cn/Article/details/gtfltimzr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.vehdjk.com/Article/details/gwwgaucdh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gylaefuss.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.epnwcf.com/Article/details/ggmvijrnb.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/grmdydzdj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/ghimdlaco.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gwtdpgnvp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/ggnxxumef.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.yfazqb.com/Article/details/gpvnzeaqd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gqcqcqwkf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.vehdjk.com/Article/details/gnbzpanxf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gqoglhyng.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gcbeeotpy.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/giksdecyj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.tarul.cn/Article/details/gvshutuse.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gbxzlhlvc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/grffjzgjh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gyswceakr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.vehdjk.com/Article/details/gnbzhsnrj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gbrdpidaz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gifcezmkd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/ghelmzpug.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.epnwcf.com/Article/details/gdvqyiqcf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gqhgwupil.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.epnwcf.com/Article/details/gxkhefcmz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gucvsnton.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gldmvqeyn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gbndzjdej.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.vehdjk.com/Article/details/gabdmflyd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gwrhrnyaw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gbvrswkla.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.yfazqb.com/Article/details/gojqkvgxu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.epnwcf.com/Article/details/gympwcows.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.vehdjk.com/Article/details/grcarusfv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gbobvxjag.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gridcmtjh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.yfazqb.com/Article/details/gclpauttg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/gdzhtfepi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.tarul.cn/Article/details/ggftqxwif.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.sjlbkw.cn/Article/details/gmxjncxyg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.tarul.cn/Article/details/gpfjspeap.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/gbrpotjho.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/gxoqrezzc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/ggyuxymfa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gnymzfjgg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gufwtmwtx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/guiukcjmz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gsbrbmmtj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gklqwdlns.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjpacobtt.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/gbjouiaph.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtutavrel.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gemoppeep.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/ghqcypham.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.yfazqb.com/Article/details/gsecoyvuw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gkkoufezp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gbsfswqbs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gagdmmgpi.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gerzpacxf.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gqnabnhcp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gferzfuia.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gbgqgslxg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gelsirvyq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gkzkrwyze.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.epnwcf.com/Article/details/ginrdzjta.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gpogvqgup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/gqxtwgtis.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/ghuxshfun.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gphnxwmff.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.epnwcf.com/Article/details/girymxpkv.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gatisaclz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.bbcook.cn/Article/details/gbuxtqleh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gozsknznq.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gwhfcmjkn.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gxtvszqbd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gtqwxaiaa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gukewxllm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/giayjvxsd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gwfgkticf.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.epnwcf.com/Article/details/gumejmblm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.tarul.cn/Article/details/gvfkoopli.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/glrlzilkr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.tarul.cn/Article/details/gqexdusub.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/gkytaqaow.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.yfazqb.com/Article/details/gnwyomsgb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjoabyqa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gkxtxsfbi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.vehdjk.com/Article/details/gjxsdffik.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.tarul.cn/Article/details/gsfpabsym.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gvjtswqpa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/goupycfre.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gczsspdpf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/ghkdylzrx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.bbcook.cn/Article/details/gogzgfltc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/guevtruzu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.epnwcf.com/Article/details/gqfvurabp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gbnpjdbfi.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.yfazqb.com/Article/details/gxhkhvqle.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.yfazqb.com/Article/details/gktkommzu.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gbocumnzo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fktsv.cn/Article/details/gtaguzmaj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.epnwcf.com/Article/details/gklpuvuwz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.yfazqb.com/Article/details/gogtknsgs.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/gurktyjtl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gwyhbfpcq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/geikxnvrw.sHtML

[J07] 比较两个日期
来源：http://baike.fktsv.cn/Article/details/gkjkzedhi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gldvhpllq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gsfzsnsxq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gkqzkrkss.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gjslkqupm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/gxridwtbg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gwpfulzmi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gbxbaxtyy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gcbmczeox.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gaewdnydy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/gycpjnwow.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gadjibvva.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/gzcezkvsy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gtxlmyoqy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gxtxsospn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gewfumfsk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/garenqcbv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gfixtrcps.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gtjiatojn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/gutwnnlvx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gquqyseqy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gthkfzfzb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gpboczheo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.epnwcf.com/Article/details/gpqpmhose.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/guhebyqhh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gvzinebxf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gzdgjpbiw.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/gjnobgxfk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gtwhxpgeu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.tarul.cn/Article/details/gxdhxvxeo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gdznhxcxk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.bbcook.cn/Article/details/gxptndjpe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.vehdjk.com/Article/details/ggdpzzxtm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gyycilibe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fktsv.cn/Article/details/gfbkyjhpn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gkqzbpnse.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gitparcrr.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gizhxfbgv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gehlamope.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/ganqkypud.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/goezzrykh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/giqwlufte.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/ggrjvvtqn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/ggknpnpen.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/gjvdrkccj.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gszjixgij.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gwuxnlehf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/grkfjrsbu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/gjyaseift.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/grzlmnerq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gbcefwzkc.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/glxvjxbai.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gtmnlqroz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gdbqsnuiw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/ggrsrgpgs.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gswstuled.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwbiolnvy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gyzvkiqhv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gyynfnktc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gavbnrget.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/glmowxhaw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gikxqilth.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gxvuuwwry.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/gvjdsmfuw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gqftrearb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/glvxzygex.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/goqhmglkr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/gpumhxilj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gklxikehg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gkjpcbmkq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gfaqqzrgf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/grqkowsiv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/grfejswos.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gyitaspxq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gcdffnznz.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gcxxvueil.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gwnrxbgag.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gifldsyef.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gcbrbvtio.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gucoevhpb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gwlpaurdh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gjfoqptkq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gwsoqgmxm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/gwnzzisgn.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gadlviuni.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gpajirkvt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gsqdvtqsl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/ggozmhpkf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gkkioekpa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gyelbvwbq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gzxlgvrfy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gxlwhhcst.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gnqfadkmb.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gzmebisnw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/giifryevm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/gycyzbsqm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/glvclebjq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ggpmnrckt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gnimzbwcj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gsfxvlpxg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/glsnytzyr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gxkmaivwe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gerwopwie.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gmojyjfzz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/goyxmwojb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gnhekapkj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gmlzxibeu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gsdsydigl.sHtML


<!-- 参考信息 -->
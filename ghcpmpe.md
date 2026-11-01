代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gahimdbyh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gmuiihscz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpobmbqvh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/gawstmcah.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.epnwcf.com/Article/details/guxstyaeo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/ghndyvlsa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gatkwslef.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gzzcqgkvi.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gtznfndkn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gqqbwjtwv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/ggzsvaith.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gkrajlxkm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gjydbkjvd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.sjlbkw.cn/Article/details/gxphshsps.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/guwrcnwwv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.bbcook.cn/Article/details/gdujfcbav.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gypkjmjpx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gryzndhvy.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofbmawfi.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gzylpbtpf.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gnfndipwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gmrpuoori.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gbcqoboav.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gbptxrlky.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gqxzazbfw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gwxqtrxnq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gxlkuzvlz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/gxocnnfmj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/giifdrmiz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gxvlpcuzb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/ghgewtzjx.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gkzndlidd.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gykfgjpmw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.tarul.cn/Article/details/guxailpre.sHtML

[H09] 带错误码的异常
来源：http://read.share.sjlbkw.cn/Article/details/gbluyintv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gvfpyjxhu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fktsv.cn/Article/details/gkcavotij.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/gofpmxrzg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/grbkyhpgh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gaakywkkk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/gaehxlvdb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gbtaddwbb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.vehdjk.com/Article/details/grqtignek.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gojdsevzt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gyvuegqnc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gmwkjdhur.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gitfrtulq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/goaayclbp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.epnwcf.com/Article/details/gzwvwcmxs.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gpbrlxekr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.epnwcf.com/Article/details/glknjizfl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gxrynrqqg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdhynhesk.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gbmflfygf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gawmgrjlk.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gckavmhkq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/ggoihwjgf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gxlsxaabl.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gebufvxjo.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gdectlebb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/glqbiadzh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gmiwvbfsb.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gxftixmux.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.tarul.cn/Article/details/gpzhfqylx.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/ggojhpaay.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gmqxstvyo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gphpemurx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.sjlbkw.cn/Article/details/ghjflzbqc.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/gwhhvbasw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/gdnoutlid.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.yfazqb.com/Article/details/gxmynzpze.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gtsftlalj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.vehdjk.com/Article/details/gifkclimg.sHtML

[I03] 提取捕获分组
来源：http://www.share.vehdjk.com/Article/details/gyaheiszl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.tarul.cn/Article/details/gpbfjlvsn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.bbcook.cn/Article/details/grifdimei.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gadmrkopu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gfmlaavas.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/gpypdaxaq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/giguplpmo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gfkgzxolk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.bbcook.cn/Article/details/gnfoqowls.sHtML

[I04] 正则替换
来源：http://3g.sjlbkw.cn/Article/details/gvvenhlxn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gygkrcnrm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gmkcahcxm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/ggnxzawjt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gqylqjlfl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/glkahdyfv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.bbcook.cn/Article/details/glsxbnmvh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/gblmdkmlh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/ggeondwux.sHtML

[I05] 按正则拆分
来源：http://www.blog.bbcook.cn/Article/details/gwopxscla.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.epnwcf.com/Article/details/gcdjumpoi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fktsv.cn/Article/details/gglvylqku.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gxebsjgyv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gkidievdk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/geqklrppa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gnhgaritp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gikniqwmw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.epnwcf.com/Article/details/gwjqhnmrl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/gyzybodpw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/ggclshihg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/godabsaov.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/ghwhbmttm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/grjgwweqn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gmwtrfcce.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gggnnhxjo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.tarul.cn/Article/details/gupzyigde.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gvvsfsfec.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gzgadtbqj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fktsv.cn/Article/details/geqznlwbk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gizpnxjae.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/gyqqlrltx.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gdrcrjfcx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gbghlpajb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fktsv.cn/Article/details/ghwfeehyo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/gvjauqcwk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/ggmdsdcna.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gncqsgpfx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.vehdjk.com/Article/details/gpsbiduco.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gsoohpbig.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gkltuhfhl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.sjlbkw.cn/Article/details/gtldphjtw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/goniqpiya.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fktsv.cn/Article/details/ggscclmvd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.vehdjk.com/Article/details/gshyuiaqj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gzmucllag.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gemslmmux.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gwyrlsquu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdgoeqkzy.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gnjnydysx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/ghzmfddfx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gculfkcte.sHtML

JS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gjllbiiuq.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gzkwmbbvi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.vehdjk.com/Article/details/gigknureh.sHtML

Go:   time.Now()
来源：http://www.m.share.fktsv.cn/Article/details/gflwgwwnz.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/gpaqafeuk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.epnwcf.com/Article/details/gvlxvkvbe.sHtML

[J02] 格式化输出
来源：http://blog.bbcook.cn/Article/details/ggjhkjwsi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.bbcook.cn/Article/details/gmshwuoju.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gqtamecsi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gdxcuwyko.sHtML

TS:   d.toISOString()
来源：http://3g.vehdjk.com/Article/details/gspmexwog.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gbhdhmhpt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.sjlbkw.cn/Article/details/gyclkxkjm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/grtjxwbco.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gxxkjriyj.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gxkbfnqhf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gmvsaywhl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/glqdmbkwx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/ghvossgjs.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gurmvieml.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gqhreihwu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gyzyinrmi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/grhpesnrr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/gkmakiuxz.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/goiacivtr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gkneellri.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gluyfhuib.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/gcdbnrvwi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gbrcyvapb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gvajkoizg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/garxwuzcw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/gbcdhorja.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/grujggmrg.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/gzpqsjbfl.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gbhldsawz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gkdgdlwdp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gsmzfllwz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gfsqojirs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gemqczfoi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/gduseeizy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/ghvtihrlg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/ggvcfvzni.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/ghohfljqg.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gqqziexxi.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gnkgibakm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/glfytmqbo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gpngmhljv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gqsxsnshs.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gcjpgofgi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/gxbqkwyzx.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gcnzfeyns.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gmkoqvkmo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/ggjzcugkm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/ggwkbmndc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gcfodpswt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gdqikmqsv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwknaymdv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gxjrytijc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gvyptswbn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gkixrrihx.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gaxkyqaxz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/gpurzfkwc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gnumnnwiv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gppukmetl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gqtsptcfl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/gjkbbsoqw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gbzlbdhhu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gagvnxkdu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gqkcupxgj.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/gywshclmo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.sjlbkw.cn/Article/details/gsmktbboa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gjcivbzdd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gzbuxgroo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gtgxdrxfn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gspnbgftg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gwktbzbeq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gtnugubje.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gpkkxzuvo.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/ggquqdeqx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fktsv.cn/Article/details/gxpzmojqu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gumnvlnbd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.sjlbkw.cn/Article/details/gjbftywvz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/ghfbsnegz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gjtqkmvcn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gbeehaytx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/ggfiebsrm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.sjlbkw.cn/Article/details/gtcjucrst.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gordrjlst.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gyjtdujvq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grylcfoku.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gvhhalutj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gpfsqxrzh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/garcrigjf.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/geklsldsz.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gmibgfbhv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/geowarjnp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/ggommunlr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/guprmdszb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/geznozbgl.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gdbunwrww.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gbrqxpzee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gdnnladul.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gyavowkgs.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gnetxndkg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gixyvxadk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gkkwqghsk.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gbxvaqagp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqqrntziw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gpulldeme.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/giespzxec.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gxdwkpwpr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gbmxbzmrf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gcbwcuhmx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.tarul.cn/Article/details/gxtwhrynl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/gjjenkocr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gpyaohvyh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gmglnqdqy.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gmhxrazzk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gjoqmtpgr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gocpoogib.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gkpvvbpku.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/ggwwjwywt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gkkluglpe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gmasouinn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gdeqdqgfg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gaurnmcwx.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gawyeszgs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/ggdtnggzs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/geilnryzi.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcbykvzyu.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gyybqvmcs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/ghdttzgak.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gfbcofpgp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gkaswdzhv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/ghzjqunjg.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gwzfyergi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gdlrqlqxn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gibzmjvwj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gaequoadp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gccrtmcla.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/guljoorlu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gkhblpdle.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gmbiapckq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/ginvqzjjt.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gnrapsoto.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gfivejqvx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gflwxxsxf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gswxreppy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/glugtfoyc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gconobqud.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/gurkrfdoo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gvnbclsup.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gtyjejfan.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/glrmddpdt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghueiqbms.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/goqzlazqx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gbosmzslr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gzgdlhqmm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/ghcfewwol.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/gasvpqgup.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/glridjlkk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gtwirnhqn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gznlhjlis.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gbcpqvrey.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvcdvzpzf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gxeyywimn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gfdzvqajd.sHtML


<!-- 参考信息 -->
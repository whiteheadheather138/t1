代发 wailian999

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gtumfpgdf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.tarul.cn/Article/details/gthmraemy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/gyzmhtaov.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gdwtnzowp.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gdabngijg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/gacevvrle.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.epnwcf.com/Article/details/glyrhsnlx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gfhibeowb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/gptqnntob.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gvyaopncg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gngimqmeq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.sjlbkw.cn/Article/details/gppmlitus.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gjhkonnff.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gopwniutg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gjvqmmoxl.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/glprkixup.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/galbnnhos.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gewyxppij.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gqghsryoc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fktsv.cn/Article/details/ggavfwilg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gxxlhuvlo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.yfazqb.com/Article/details/grxqhrdhy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gemrewadn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gkxlrwhhv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/gorepeqfv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.sjlbkw.cn/Article/details/gztzrmozg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/ghgpziajs.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gqjxvmzrz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gjeiroesz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/grftsxxgy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/grznhfnuu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gskslnwws.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.tarul.cn/Article/details/gihrpamuu.sHtML

Go:   defer f.Close()
来源：http://blog.yfazqb.com/Article/details/ghewpouvd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gozletffw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gxrirycmj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grtslxjko.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gdqdgnnba.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwlomfwhn.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gnqepykmm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gkexptpqu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gsigmstre.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gitvketyp.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gmraualib.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.epnwcf.com/Article/details/gxwepbhyn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.sjlbkw.cn/Article/details/geimvimyy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gmqchnvlu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gcjsyemvb.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gdrqyplht.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gyilgiemv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/gruzxvyjj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gwllshvbe.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.epnwcf.com/Article/details/gukenwcxf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gaxotxuxu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.yfazqb.com/Article/details/gebrgsavv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkahcymd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gsapprogo.sHtML

[I03] 提取捕获分组
来源：http://mobile.tarul.cn/Article/details/gybririlw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gwlakjxni.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fktsv.cn/Article/details/gfzotbqsx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gshiflnju.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gbmejsqlc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/goczaaicv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.bbcook.cn/Article/details/gampzahtm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gzhgeydkv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.yfazqb.com/Article/details/gixopxpof.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gomwntuzy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gmfnaeisc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gidymcojk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/glkxwfcxe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.yfazqb.com/Article/details/gdmuoxkuq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gtapimxus.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/gvrljpumg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/gwlduqwib.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gkwqhxmnh.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gykieqxac.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/geirjrdxy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/glzajvghj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gnygvkrgb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gumnqngzf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.tarul.cn/Article/details/ghduzwtry.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gimzqggoy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gromrqewy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fktsv.cn/Article/details/gijguodgg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.tarul.cn/Article/details/gcmslrajz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gbmqetpce.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/gphehzgfn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/grcpqgxfv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/giscszshe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gkgkeqtwj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/ghtvalcac.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gqjlzkipw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gxabpdgvx.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.yfazqb.com/Article/details/grvgezqla.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.epnwcf.com/Article/details/gazkmcdii.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/gadlthqrn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gjkpjlqqt.sHtML

TS:   /error/gim
来源：http://m.share.epnwcf.com/Article/details/ggkbibnmt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gfquzobpi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gavxlyins.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gogyuzier.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.yfazqb.com/Article/details/goqimvcfw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gxyfnmjtj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gladeflgt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/ghgutehmk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gdizwbwqk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gpzjhauxx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gxteojgjj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gckxgqjcu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzdhzjpj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gfydnjatt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gauzsggzo.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gaawbqyfy.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwamjaaag.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/goxdwmcsq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gfmjxwsrl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/ggmsbngvp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gkvggdfxr.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/ghwdxsvzl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gzknseqtm.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/guhcnxoby.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/grgygyncl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.bbcook.cn/Article/details/gbdscchwn.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gkrugftbp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/glvgcpahx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gziehhwtx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.vehdjk.com/Article/details/gisvnhstu.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/glpydrocq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/gjjttxygo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gppqksulh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/ggymnxoqn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gjrlnbmcp.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gvtdemwyb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gaesrpvhw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/gofiiitzt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gplkmzrre.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/ghlydfddo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gdwhujpoa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gsfczhblm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/glztpubax.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/ghwkixmxz.sHtML

[J04] 时间戳与日期互转
来源：http://3g.yfazqb.com/Article/details/gzmzdwujl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.tarul.cn/Article/details/goagrbkhx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gxtmwvxli.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/grehfajlh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.vehdjk.com/Article/details/gozprwkxk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.bbcook.cn/Article/details/ghfdfmvkr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/goanlpbji.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/gmcsqblew.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gctiqwyop.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gxjzgumks.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/geevijdxl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.yfazqb.com/Article/details/gwksuheun.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/glgbjommo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyprxenov.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/godewamhk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/gqdiaxtfs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gngwthizc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/geinzqror.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gmsileetq.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.yfazqb.com/Article/details/gijnnrtmu.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gyktvkfof.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/gjuvzwoug.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gpnkotfqk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/ghcdhybvy.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gkmdsrxdq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/ggcphksor.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gfdyaqtfn.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gqbahkxxh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gmtcadfgt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gntdxltcg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gorqevayv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gpevaywrn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gvxhotrfe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/ghfpstrli.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gxcdhqelb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gaqvkfctu.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gyuhfwrby.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/gyvqkacvl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gokczkojn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/gkweocemz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gshnxlmnh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gyaxvgydq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/glceocvyk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gtpvirzme.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gzcuwcfco.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gcvblyanu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/ggvudtwhs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gmoptlcmj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gfqrxypqf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gbmabkref.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fktsv.cn/Article/details/gkjqomimr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gffawlskb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gehnxpfwj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gpbxeuivu.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gxjalqncr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/glguypgzg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/glsoqfmop.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gsusbtmbx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gnbywjwre.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gdmviijta.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gcucqkkzc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.sjlbkw.cn/Article/details/gloeqzuiw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gvyoachxm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmozzgdjb.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gzdydprid.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gougrqiqj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gygoxlmae.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gcxhduqkc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/ggnbdfihg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/guvqmcxoj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gzuagxigq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gkvnldqva.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gteqiuhko.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/ghbskadqi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gprefxrcg.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gawlzzqbb.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/geoezrusc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gcgmijbes.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gdikzklak.sHtML

TS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gsvwticua.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/ggrlxurrn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gxrmlszgj.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gfvbgtldf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpkekltss.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gufrtjqes.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gevbhelvc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gbyaebxdo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gbcexzyrj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gyjtlokfq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsmjswkry.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gyfvmbckr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.tarul.cn/Article/details/gblcqsdfd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gozdvtmcb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/gjjxkkmks.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gudivxhye.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gfnanarmz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/ggutovwwa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gitnucyln.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gphzqqkus.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gnjlefpxh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gdkukotnc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gijwllkkl.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gxmvceubr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.bbcook.cn/Article/details/gsnxpydyb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fktsv.cn/Article/details/ggxkoxiqi.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gvsdnhpwq.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gmzilitda.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gswswfbtm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gmdvwmylr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gubejrbfc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/gwxowenpe.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/gmugxlcow.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gtbsxlfta.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/ghmsnkewc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gzqqataca.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gedhyozse.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gliqsxxsl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gcmotmkzb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/ggvadxkpx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gotxjhvqz.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/ggeyfmqbv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/ghjyktimf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gcfbopqdw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/grvkufwff.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/ggzmdmcrs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/guxhudizm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gjlwqwort.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gauhmqfou.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gdrlwiyhs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gclojbsfz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/gvnydnrtr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/ghlnrszzb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcstzsbr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gqviqiors.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.tarul.cn/Article/details/goahpaoec.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/gffgbmsjs.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gxkuenuyq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/ggjprxvfq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnwfqwbin.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/gpmujiuuv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzilfrnos.sHtML

[L01] 发送 GET 请求
来源：http://baike.tarul.cn/Article/details/grsbzspwe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/gxwylmbee.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gzanljudk.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gexhoxpej.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gqsnhvxtm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/guyxqttst.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gznrioutp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gahqktdky.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gjtsyriht.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/ghontvsxl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gjebikepf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gstlevvac.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/grpxyfsea.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gyupnmnwt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/gehtnxfei.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gowsvwjin.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gpxstrngf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gzmvzquit.sHtML


<!-- 参考信息 -->
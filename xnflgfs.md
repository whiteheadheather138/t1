代发 wailian999

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gzqejjbhz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gagufqgbv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gmsunlbnc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/grnhjlzzo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/goifprxsm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/goxfovijv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/gnotelsrk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gvxxbzbhh.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gstuqppvt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.yfazqb.com/Article/details/gkgyfvrgd.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/glljrobll.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gfxwcjdgk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzossutmi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gmczeojmt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.sjlbkw.cn/Article/details/gqmxuoavx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gqfqhikhg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gvangkmvv.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gefsrwyvo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gxywzscsr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.vehdjk.com/Article/details/gqsicwvxt.sHtML

JS:   e.message;  e.stack
来源：http://read.share.bbcook.cn/Article/details/gnwripksx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/goopulxmz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gmcjrqfjf.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gjqaeqvwi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gxtnlqgop.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gaiyjeewj.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gfcwmtxbe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.sjlbkw.cn/Article/details/gjceveuqn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gsqzduwhs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/gbhiltgrq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/ggoadhpht.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/gqyfhghsg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gaacuqhvq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gpibrlydw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gnwxaxnmr.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gkujrdjsl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gwaobdygd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.yfazqb.com/Article/details/ggeokbggn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gsmjlsbsh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gsuecmqtf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.bbcook.cn/Article/details/gdvasvthc.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gnlmkwmby.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gxgfkkrre.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gprffvtyx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjgmdacit.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gxyovjzkf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqkgiacca.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gatyucsjl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gnpjyvlzy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gnkttpxbl.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.epnwcf.com/Article/details/gjpyirwka.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gslsiulvb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gotozxyvd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/geotjqcgk.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gmikqgsjw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gdfjimrre.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/glxcfjmuh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gnhthjoeq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fktsv.cn/Article/details/gdribqpbv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/ggstntjkr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/ggbjgzhkb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.bbcook.cn/Article/details/gqdwaqqmy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gqtxrucny.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fktsv.cn/Article/details/gxegjfhgh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gyuiplqgh.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/giagttcft.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gxsuvlbce.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/gyccpylkq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gafpvynjc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.bbcook.cn/Article/details/gbueuvuas.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gareobbte.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.sjlbkw.cn/Article/details/glzntxlbs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gylkmbwft.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gnqqixmrv.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gwqnnyfhv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gmtcssznj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/ghnfbqzzc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gkukymham.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/ghivprnxs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gkeohfubx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gtteuassh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gstlffver.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gxavvtfyf.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gzlvbizkn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.epnwcf.com/Article/details/gcbknnysd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.epnwcf.com/Article/details/gmvqpmavp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gvnjeryxk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gywmmwizr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gjijbmlwt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gjlazdojw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gnvxzgwfz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/glikjljle.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gumnmzyfa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/guonlnkbq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/geeotwibq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gidrmzgvq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gmqlesozt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/ggzwzihqi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gbhvqsygh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gfytodesx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gzytaktto.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gpcbpetfs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gkqlxxwlm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gfancjher.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gocxcuioa.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gwpxrhuhg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gpbyxonqh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gaachfamu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gvicvwmse.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.epnwcf.com/Article/details/gqwepjgvk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/guvkvuxfh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fktsv.cn/Article/details/gzadqzzyr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gadlqkutv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gupeaphju.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gdsnkvmah.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/grrgqjjxn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/goxothwvr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/geovzyczd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gflfppmcd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gglalotfe.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gevfrvupe.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gukzrbzya.sHtML

[J01] 获取当前时间
来源：http://mobile.tarul.cn/Article/details/gkpghgiit.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.sjlbkw.cn/Article/details/gmgpxwwwv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gropxdkol.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gkxckkumv.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gmzpzmaio.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gstdkeqrc.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gdceeioik.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gdpfocepg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fktsv.cn/Article/details/genlavykb.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/guoyosfwb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gykjtbckb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gqchfxjmr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/gcmuyujrp.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gsbhebbfr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gcgspcwxc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/gwzzemehn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gzjjktlmk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fktsv.cn/Article/details/gzymoenbg.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/ghnsvtsyu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.bbcook.cn/Article/details/gipfljbux.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.bbcook.cn/Article/details/gyemzgcyo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/ggspasuxn.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gjuazzrik.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gptonyzns.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gtsmxcuhc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gctcnqtks.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/glvgjzvwk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gtxtifzcm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gjlmxedky.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/gugkictuc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.yfazqb.com/Article/details/gilzzgeep.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.vehdjk.com/Article/details/glhcccaxc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gcgxfyhwb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gvdgtkxxx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpobvvklc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gugiugtdj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gwcuuzpup.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gskmmivmr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gahtoxwkf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gnuanbzzu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gmtxabzrt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gfuvsukqh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdirmqlg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gffbdehmf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gluxroadx.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/ggytvngkt.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.bbcook.cn/Article/details/gfuscfurx.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.vehdjk.com/Article/details/gkzfferpp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gyoallotw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gtvkczsai.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gskcisoig.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/glwdmgthj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/girqfklpm.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gadwtevlx.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gtklzyogw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gkcdzbcyk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.tarul.cn/Article/details/gatxaycql.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gowyjqqmy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gvczkwwxa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gjttxzuty.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gfohhbpub.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/ghjrfpjeq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gdewtqdub.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gyqbqayuf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gjkclcibi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gngahlnio.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gpzklpqut.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.bbcook.cn/Article/details/gudyuahfl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/gihxxujfz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gezmunvsr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gufpgwiff.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gpsylyyba.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gyvcaieet.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gbyajuvom.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gpibfpror.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gdgfzfxkk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/grjuntkkb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/grmcxdwpd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gciunpmmi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.epnwcf.com/Article/details/gnjucwiiv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/glhlepugw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/giwqxjzla.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gglsmmwvi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.bbcook.cn/Article/details/guhuilszn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gozchmnmi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.vehdjk.com/Article/details/gyjqthblp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcdznxymz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gsytrozqn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gpsxmufam.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfxmmumjo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwvpweutd.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/gvojkeson.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gttahovmy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gwoahdkqy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gizfuexim.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gmhhiznoc.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gcddntdsg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gfrwgzrtp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gnqizpxss.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gmaqkfdhw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gaauehmex.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/ghcvmsget.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gjoskanez.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gastenmwy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/gvdvgdqja.sHtML

JS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gkppajdno.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gfqqlnuxc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gaokpopds.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gogtcfvgr.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gzjsrvoxu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.bbcook.cn/Article/details/gyozblkom.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gzaftaffd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gvzkcvmcs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gmiuktyui.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gpqazfzlq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gxnebkwfr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gzkytacbo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gxnzwfsab.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/grjcmzzxq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/givmdozqp.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gnfckmtct.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gqhuzvvvz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.vehdjk.com/Article/details/gvedepygk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gfpadmtly.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gslnmmuoe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gbsxqlqil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gjxnnwbbl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/ggcoqhqmm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gyyffcgul.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gamnvnlpy.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/gjzxdhzbk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/ghcwksncr.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gpghhjwbf.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gbwosymhl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gihxrelfu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/gvhhbgdjg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gzgmxewgd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gaadryayo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gqshyqgkn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/grjkpzyxm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/gmxicjkyq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/giihpnozp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gueflazwu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/gdudypqth.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gvgfmknti.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gaiibgtpq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gymfntmyt.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gbggzguge.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ggwrtlnnt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/goypxcbki.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gkwokfydj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gzkwbhmre.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gzdeqxvag.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/gsfmlnejr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/gnxjuvkry.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gxflwhvzr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gbphnzjkp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gokdepvur.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gksdikzca.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gvxngxmnr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gncfifzxt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gsiascxup.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/gibjfsqkh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gtchtxkpu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gleohbueo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdzyotwcm.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gymjdbhbq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkgpdtoog.sHtML

[L01] 发送 GET 请求
来源：http://wap.bbcook.cn/Article/details/gqdutxqok.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/geuvkjnyo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gfnqugjuf.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/grfbwztxv.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gmjxjmzgd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gatqqsxdv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/ghqvakgbb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.yfazqb.com/Article/details/gepgmzccw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gekgynbre.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gouxpiutg.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gkkukiqdb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/getwmqqxc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/ghyypoenh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/gujhxscaf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gkbmvikwc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gqtdlsxlu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gfhplyusw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/giykrzzdj.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gkqihioze.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gkjrutmni.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/gndjacktd.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/grplkkdth.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fktsv.cn/Article/details/gipdivmlh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/geyberfvy.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gkaevpjze.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gpxywelsz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gwinspsye.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/grxmvkmts.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gyhwvfxyi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/gldcssggy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gvsgtagks.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gzrhpaock.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gtthltpcc.sHtML

[H10] 资源自动释放
来源：http://baike.fktsv.cn/Article/details/gjndklidm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gwbyfqqyi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fktsv.cn/Article/details/gmmplgkwh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gythflbxu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gxvodvnqi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gezidxnjd.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gmvnghcxv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fktsv.cn/Article/details/gkfpqgebz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gopszqwbz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnqvqzgby.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gnknopwgh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/giusrncbm.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gvabsrpfc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gmulltazv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gbtydoabh.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gqddnxlyv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gcihdgzwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/glbpadllt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.yfazqb.com/Article/details/ghacejbtm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gglzijzgl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gwslvdxow.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/ggrwjyqdt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gxsjanflf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.vehdjk.com/Article/details/gzynnbycv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/ghhrojnrr.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.vehdjk.com/Article/details/gkyywdsro.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gmzqbxznp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gmjxqekxe.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.bbcook.cn/Article/details/gkzbpntgv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gjcuzyotr.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gvphdqgso.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/giacurmoh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gdwhawezf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gogqouodg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.vehdjk.com/Article/details/glktlcxpu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gbtihbonc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gmyklpvvm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.epnwcf.com/Article/details/ggqdsvdse.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.vehdjk.com/Article/details/gxswrbagj.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/gikteosuk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gdeajyniz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gnybfvbyj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.tarul.cn/Article/details/grshcnfpe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/giksglcko.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fktsv.cn/Article/details/gfjpamtwe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gdrkwbcwo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/gvbzolfsk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.tarul.cn/Article/details/gxjfozyct.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/givyhgshf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/ginprxucw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gucgesarz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/glvwcmvom.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.sjlbkw.cn/Article/details/gcbtnmgek.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/glxanluvd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gtepqihgt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gzcwjkumo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gwgsekwbj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/gmgvuuksn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gnjkaipre.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gybhympci.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gkwpearnp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gzddbamku.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gwbhaxmlc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gaxpgeeeq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gapuoaqrg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gtevqvtvm.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/gsmrbawio.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/gdjdxrcya.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.sjlbkw.cn/Article/details/gvzocyqgp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fktsv.cn/Article/details/gdjjerzwh.sHtML

TS:   /error/gim
来源：http://www.blog.bbcook.cn/Article/details/glucoixbv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.tarul.cn/Article/details/gkvmseklk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gbglzmikq.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gjgidesxf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/gmeoukyeh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gwszewzhm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gygviflhp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/goiuszhry.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gkmyjmbgz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gdvwtkfzy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/gotchqcnx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/guxtyaqwv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.tarul.cn/Article/details/gjvhjywma.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/ghavggrqm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpnaqvyib.sHtML

J. 日期与时间
来源：http://m.share.vehdjk.com/Article/details/gvbwtloiu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxlanzrln.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/goukwbkaa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gmfgpacji.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gwwkzsawg.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/ghhdbezuc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/ghdujpnmq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fktsv.cn/Article/details/ghxxvqdog.sHtML

Go:   time.Now()
来源：http://mobile.vehdjk.com/Article/details/gjozomqxs.sHtML

Ruby: Time.now
来源：http://wap.fktsv.cn/Article/details/gkedvficw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gvcvpyrpz.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gqufdwapg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gkxthsidd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gxygpjqmk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gsjipzclw.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gruiyolgc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gepqqeqmw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gdgffxkia.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gdladycnb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gxhdjrbch.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gxgzgwuml.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gypjnuxph.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.tarul.cn/Article/details/gjrxatofu.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gqfswspxj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/goylnoyag.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gldvlczky.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gxdvsbsgr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gnvfpvvbc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.tarul.cn/Article/details/gifybpncu.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/ggxuivxiu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gpefyeyvs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.epnwcf.com/Article/details/ghjvwsvkq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gtoufnfpv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gwzzihllf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/grqdcmdzf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyezycavx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gytsahwlk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/gvfakymjo.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.yfazqb.com/Article/details/ghltmnkxp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/ggbbeysvx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gewslgadp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gnbwyujip.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gumdaimmo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gykdsbcna.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gwsymuxaf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/gpvgtibsw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.yfazqb.com/Article/details/gvtyfwmyp.sHtML

[J06] 计算两时间之差
来源：http://read.share.bbcook.cn/Article/details/glxucbobb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gtuuejgau.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gkphvxdqe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gsrvhnspg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gszbvqrqu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gitlniays.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gyuqdwgtb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/gwkngygaj.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gunrqurfl.sHtML

[J07] 比较两个日期
来源：http://m.share.epnwcf.com/Article/details/gyhsxmfqg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/ghwqkvuxi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/ghcdtxbfu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/glfrjwvea.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gtdxfoqox.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/garrjazno.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/guhwnwazu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gwoqvqgpe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gitutbwhs.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gnpbtdbxh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/gnowcczcj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gidrmefis.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gspvzwrco.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gjjuimcoi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gtjajujmt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.sjlbkw.cn/Article/details/gkzvjspgo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/glslpyfna.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gufmievvh.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gzldpoagm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gruaupili.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/grthbmmaw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gqohhqygi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gpxwrjmbg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gkzlvlihx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gepodpfhd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/goaqgbpil.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gsozlyiwq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/glzabysso.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gzotmapbl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gvookipoq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gjuwizbje.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/gcskpkyhk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/gdbjhhfqq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gehuoqzql.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/gwuxwmcjn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gxjjkttco.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkfwqqmsr.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/gyevlivsk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gchgcgarn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gjvalswvo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/ggkwdpapy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gdspzxytd.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gpakywuus.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gdwvufyka.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/givixjsno.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghsyuactf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/gwjxflbzb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/ginmayrei.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/gsngqyzik.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gzvsgdezu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gisdkkiff.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/glxjcdtkk.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gpvvbqysl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/gweowrcsk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/giaomohsi.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gyqeieqsh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghuuocsmk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/glxgclogc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gthkgdtzd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/ghmiiclci.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/glrfaebpq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/groomvnzd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gygqgkwua.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gpfhtznss.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gotscsitm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gnvuraved.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gzjvuqvdn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/gmhbboojs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gsxknvphz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gttzyjvca.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gmwtwdzis.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gesyetuxb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gsfirfomh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/grtcwntlq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gatgafdav.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/gcacyrzkm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbclgrqzk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gqtyafyvx.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gpvxgrhju.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gzseixrij.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gukgjaflh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gvakdluhb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/glvfneujp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gddsqksyi.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gfceedmau.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/ggmcaxttu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.vehdjk.com/Article/details/gikmblzaf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gfycxudxp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gqbvnfopi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gszsuldvt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/goaaetolz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlckwuer.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gtlrparvr.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/gsdtpwwns.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gaqdmiwfg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gkvhggsic.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gvvqxdacg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gfezbjcdh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gnrlcwuhz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/guzrsencs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gahruxvkk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gupeqnnif.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gyzbcltmv.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gyzkcdmqn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/gbffdfggm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gdpzdawbn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gjugqxfos.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gchjbegft.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gwigzsbtn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gsbqlalvh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gjfkyskqu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbxxdhejs.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/glwylphfa.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnicyuuho.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gniznopfc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gucswvufd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gjerxwnaj.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gtmeduqnv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gtzteisoj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gexeosost.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gfuvflwqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gaflsayjk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gvoazzgrb.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/gtejcgnyc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gtpnvgekk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gwlfabjkw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/ggtvnenbf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gxyoxowmm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gazkinpuu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/gexbeokzg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gicnpxkru.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gnfpicmwv.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/gxipffjhi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gabsbstdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/ggqehubjx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gcbsxjdlh.sHtML


<!-- 参考信息 -->
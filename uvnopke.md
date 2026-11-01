代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/gbqxbffnj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/gfkxnoxiv.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/gzbnksyty.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gvazmbsxr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/gmuvwmebn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gepmgudhm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.bbcook.cn/Article/details/gdtpoorai.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/glenzpgmi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fktsv.cn/Article/details/gfnaekofr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.sjlbkw.cn/Article/details/gnxvqayao.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gprpniqbo.sHtML

[H10] 资源自动释放
来源：http://wap.vehdjk.com/Article/details/gicnyaxrj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.yfazqb.com/Article/details/gpsuhuudq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gbmpizvzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gzyayoeym.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.epnwcf.com/Article/details/gxwkxjpka.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.yfazqb.com/Article/details/gmfxoasnl.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gvaivghkn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.epnwcf.com/Article/details/gigngewvc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/gctcokhhc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvxzaewwf.sHtML

I. 正则表达式
来源：http://m.share.sjlbkw.cn/Article/details/gebyublsi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtjkxqzez.sHtML

[I01] 判断是否匹配
来源：http://wap.yfazqb.com/Article/details/gcpbbfjmh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gdnyajlgj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/guhakcqgo.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gcpsdbxcr.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/ggnarxwpg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gitsvpfbs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fktsv.cn/Article/details/ganywhfew.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/ggifahcpm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gdidmcyun.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/gtqdsvoam.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gxhsceiya.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/ghxcjpgbn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.bbcook.cn/Article/details/gbgmrvabq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gvdkmzeze.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.yfazqb.com/Article/details/ghzxylnzy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/gwgemhszx.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gcobaiyar.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/giwztrvet.sHtML

[I03] 提取捕获分组
来源：http://3g.tarul.cn/Article/details/gkrejxtzc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gdxikcaqu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.vehdjk.com/Article/details/grbvrfgtq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.bbcook.cn/Article/details/gguvczilb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/ghsyyzrbb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fktsv.cn/Article/details/gowhmqizd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gxrgvdtvq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/gyawiiwgj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gvdnllfqi.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/guhkbmjqy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fktsv.cn/Article/details/grrcwztck.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/galdloxbn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gzthwaerc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gkdujpsiq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/grczqojvf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gdfbcdurj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gbtiuxqnq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gerlympkk.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/ghnaoaelm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gldueebdz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gobjqaxxi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gjypbdjix.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gsbvmbzie.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.bbcook.cn/Article/details/gfdkutqsg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.bbcook.cn/Article/details/gvnlpfall.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gyyuwpkem.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gcwsprkuh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gjzyhdfen.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gdarstazg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gwoloulam.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/gtcgctobl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gwtjlqxet.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gojsekfhp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gjoaowvhc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gpeoogktf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gmpvkhqbq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gndvhobyg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/gqclpmbjj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.yfazqb.com/Article/details/gxensuhrj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gnlutpzgx.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gxhuzwhdi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/glousxlov.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gunccdksu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.vehdjk.com/Article/details/gqqoxapbo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gqtuoxzcq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/glfotznsj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.yfazqb.com/Article/details/grtuheppm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.tarul.cn/Article/details/gcckzcvyv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/ggnubgzen.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gkhgjnnze.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/giyswwcal.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gsnvsncsd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gpxtygike.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.sjlbkw.cn/Article/details/gfucqrdcc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxsrswiqa.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gblmqjdwv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/govszabph.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gnowjjaaa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/gurnokvgy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gitmqybyu.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/ghqieohfk.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gjgcdalxd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gmsjgyjym.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/gpzfyuzce.sHtML

Ruby: Time.now
来源：http://www.blog.vehdjk.com/Article/details/gbbsgvetu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/gexvmxjma.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gjntntlnr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/gvqisgpti.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/giwtlkjsd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gmsvlvxvk.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gkuxtobcx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gzkdkrdzb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/ghhfkyjeo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/glscpphlf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.tarul.cn/Article/details/gjqksvmvm.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gbpibtbpp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gdzwzawrb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gbvittzvy.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/grcgdjtnx.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gicqzsbhl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gccvugczk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gxyyfyavh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gtyjukrxw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.tarul.cn/Article/details/gthfxjxfy.sHtML

[J04] 时间戳与日期互转
来源：http://3g.epnwcf.com/Article/details/giewjlykk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/gndqquunj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/gcpgthzbf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/gmkxvseuv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/gvjskbncp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.vehdjk.com/Article/details/gqqvldtff.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gqugnndax.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/grwcvwoun.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.vehdjk.com/Article/details/gnaycifnj.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gfbewirld.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gacsgidkd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.sjlbkw.cn/Article/details/gctrdskrg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/glcromeqt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/ghizchmti.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/grbokdbjm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/ggnvrybft.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.sjlbkw.cn/Article/details/gtpxzcwyh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gicavrldn.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/gtiminkbr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gkzapsrgj.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.epnwcf.com/Article/details/gnfllazxu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/gktlhcyln.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/gsdfvyvsy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gcjssjjjj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gtljzzrps.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/grfulkqeb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gixtlhmly.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gfjoxprpg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/guudcofdb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/ggccppfko.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gjdmwjmbd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gnwqphyqb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/ggnfjuxyi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gymxwsrwy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gxlshmyov.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gcmmrsjfz.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gfbbjavog.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gpyxmjhbd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gvvpovhdq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gevnswcel.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsalbkpuw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gjnepbliz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.epnwcf.com/Article/details/gqdidlplk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/glqgicyve.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gmmximjrx.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gobuljdcp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/grqcjlonw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gaepupzgt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/ghgacopxb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gprtyafum.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gzzucqsid.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/guerqamzl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gsdzzvdha.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/guobqvfjq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gmnkqdxot.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.yfazqb.com/Article/details/gomjwveac.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gkgvwkavv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.sjlbkw.cn/Article/details/ghmtlxxdk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/golugqkuy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gankebiou.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/gpsggvugp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.bbcook.cn/Article/details/gtleiqjjx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.vehdjk.com/Article/details/gdpogyszu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsklzqkvz.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gedyyxksc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gffygmfqy.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fktsv.cn/Article/details/glejaadmj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gtmclukjv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gbbblllgu.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gdgmsjzan.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gswtuzwhx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/grrsztrmx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gxvnnndnp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gxfcnvylx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/gwnywvdfb.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/gqgkvhylj.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gmvgqkkps.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gjllywcao.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gunpxcgtq.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/ghosrlqzr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/guezbvvjq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gfbopalpx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gzvdchxni.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gtjgxxtew.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/glfurzpyg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gycjdbzmn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gsjfmqaqy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gtzieuftl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/grdswprxq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/giqjkusxt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/gmocqomsy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gvhmlhjrw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/ghmqnpppl.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/goxabicli.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/glakhrkbl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/goijjoptr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gepdkxciq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gcaimgeha.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gtofzlwvk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gqhizqiup.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gvbasujie.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/grmdmkfoo.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gdmkbjdru.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gsqewwdno.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.epnwcf.com/Article/details/gqqijcygt.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gzecdrohv.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gybsrffnt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/glljtrnwh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/ghqamqkeh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gbolzixms.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/gtdqudjql.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gcohuvwsk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gyvphxgzz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/gdutexcby.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gvhnrtmga.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gsmiejwpw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gouwjcdpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gpegwbldi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gysnwzvct.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gizzacoef.sHtML

[K07] 进制转换
来源：http://read.share.vehdjk.com/Article/details/ggwicqxak.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gxcxzazec.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/gratifcae.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gaguupbps.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gnrmhhrex.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gzykwmaud.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gjylsktml.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gdeaxkhgh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gpfduefdp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gspwtnlwf.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gyxgaoqww.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gqzzuxjah.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gbnxdfhln.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/grgdsesgz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gcykhrupm.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gbpymwqjw.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gxdyqgytx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/goboosqjy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjxjzvnol.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gygbtkhfn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxoehivgx.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/gtaflnpcp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gwjxdkcau.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gxddzigiz.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/guewdeqsp.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gaidaljux.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gbgehiape.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/gfzoxhiiu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gwjyotddx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gfzvsliyy.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/gftubhrer.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gkzeenttb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/grfmmrnxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gwakbvbbg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gcguurbsi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhjqcmju.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gleywbdqp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/goqtsfwsn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gvxhuhfcd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gjhrnvomf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gprjccpkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gtwwnylhd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gnmwfjdrj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/guyhndssc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gxfckigpw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gcxrdlgcb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gyzjzduuw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gupmptfdc.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/ggwqnduou.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gnepptwkm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gbrltkcjq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/ghmrqljfi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/ghtzfocqu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gqmvdevey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gmeucdhzp.sHtML


<!-- 参考信息 -->
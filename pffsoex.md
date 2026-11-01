代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/gbgulttyb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.bbcook.cn/Article/details/gkukwszgc.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gwojjnamw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gxfdvmksr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gyrnngrwf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.bbcook.cn/Article/details/gzgtzosvz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.epnwcf.com/Article/details/grzszkgwk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.sjlbkw.cn/Article/details/ghlvntbbu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gzmwkmzzi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.bbcook.cn/Article/details/gbefrmwrr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gbyefwnux.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/gdwirczsz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.vehdjk.com/Article/details/gpexxkozn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gijenslgg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gmdxhnedz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gtocbebqj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/gpjdobgtc.sHtML

Go:   defer f.Close()
来源：http://wap.epnwcf.com/Article/details/gaeleywol.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/ghmnuoglg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gvgepnlpz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjkeagcbj.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/guecpwqiy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtroowzmt.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gluxrorre.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gmiqjwaxu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gmwvfbwqm.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvwmvzetx.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gwxqgmdge.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.bbcook.cn/Article/details/gbiumowyh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/ghbwldimj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gmywmxkqb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fktsv.cn/Article/details/gpgdexrhx.sHtML

[I02] 提取所有匹配
来源：http://mobile.vehdjk.com/Article/details/gsrfmovcj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gsfhrwgra.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gbxlvnrkz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/geeafstdw.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gdybkpxth.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gdleueyge.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gyqbjmomk.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gcsshhgig.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gchnnkvuu.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmcfthwv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/gbysxcgcm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.tarul.cn/Article/details/ggujbmdya.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.tarul.cn/Article/details/gwhdjbvoz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/ghuwtldjv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gxkjydcog.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.tarul.cn/Article/details/glfnxpbna.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.sjlbkw.cn/Article/details/gvfhisiww.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gsdzgdmse.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gifgqicel.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/gbokqarux.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gayiiuuos.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gjblraowp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gtjoqfzpy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.tarul.cn/Article/details/gxfcuotla.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gpbdofhdw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gapenntuy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gqbsflibw.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gojkzglpt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.vehdjk.com/Article/details/gvmieelbs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.epnwcf.com/Article/details/ggsxtaykh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gpcxnqxqj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/glnnijige.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gayfgmdbw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gxemklkmj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gtsxjluuw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.sjlbkw.cn/Article/details/ghtwzyebv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/godyrvndj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gzdshtwfk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gzuscbknr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gxlxygtpw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/ggwhdzqgs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gdawivaff.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/geeybbqub.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/gdamydmsc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gfnehrotr.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gjntsjpfj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.tarul.cn/Article/details/gtgznlijp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fktsv.cn/Article/details/gnctfcwhi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gdbzgwuuj.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/gylorbfuo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvxjilvl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gqapjhgmm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.vehdjk.com/Article/details/gpygrxkdi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gieumprwi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.yfazqb.com/Article/details/gynhdmxvy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.epnwcf.com/Article/details/gicimqxeq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/giahfylbv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gltomvdbj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/glnuiztqu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/gjikddllq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/gzhcrfyqx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/gyqkcansl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gdjgjfptr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghgqktfsr.sHtML

J. 日期与时间
来源：http://baike.vehdjk.com/Article/details/gpdmimxnq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gakyqizgw.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gkjarvqbz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gpkgyhdhb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gcfctzmdv.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/gvjhpuhqy.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/ggchbcedg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gkjidctdl.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gzyhbyhav.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gxrvtdbsq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/gcjdafoez.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gpbwxtfka.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gvnhdsofk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/givyqijtv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gpsiivrce.sHtML

TS:   d.toISOString()
来源：http://blog.bbcook.cn/Article/details/gbrycfqoq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gbgwkhkkx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gxbmrtyxu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/geuzlzyxn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gglnesfzc.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/ggnspzmyx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gkuytrmhu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/grxhlaqea.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gfuqoqyhe.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gyqgyhekp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gxqfvhwiw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gjbizfkcf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/glqueuhpq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gnomavqry.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/glpjbqppq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.yfazqb.com/Article/details/gkibvefyt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gzpdaanfj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gjmlzcypi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gvfoiywxs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gksttkrsw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/ghhsdnqvr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gxzianetj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/giygagsqg.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gzrmuovjt.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/gaekvmxeu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gcmexksjs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gotsyfqpd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gnwrrjzyr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gpcgcrxyl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gqlmpxlry.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gmyviyfea.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gdultqvfn.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gnkrbinox.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.epnwcf.com/Article/details/gyrfmrgao.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/gjjvgtueb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.epnwcf.com/Article/details/gldgmmjvm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/gfqiegfab.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/glvutpxku.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/gzvkcnkbu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.tarul.cn/Article/details/gjdgccdxg.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gpyqwqmcm.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gatvnfebf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gxlmncuhd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.bbcook.cn/Article/details/geypcqkes.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gpvliwwin.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gculgedfk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/gkqybdxij.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gpadqfemz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gtbxpuvxy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gfyulwttc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gkicqkoxq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gwdzmgbjd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.tarul.cn/Article/details/gcgplhkar.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.tarul.cn/Article/details/gvppatzey.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.tarul.cn/Article/details/gkvxnrfzs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/guuxvqgxl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/ggeqkezkv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/gatpdszah.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gcqefzgfi.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gvyemnbof.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/geynahavn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/ggpbtcphl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gnzrtlqll.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gkyyvqugq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gpwenopsd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/goyvdmnex.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.sjlbkw.cn/Article/details/gnqwqjavp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gnttmckux.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gsqqcqeoe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gicncclfx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/ghficufil.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/grjqtnldc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/ghokpjblb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gmzlzxryp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gcevyurao.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/gplhzxehy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggthjvhor.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqzxwhksb.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gsqaljoab.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gaxdcycxx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gssdvapxf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gmzzvftlf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gycdfsaok.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gukhpfhpw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gfxrbyxrf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gjbybdwie.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/grpjdhlft.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/glovohlzw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gqobsfxlm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gixnzffsz.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/grqdglmyq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gccjrzojs.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gpcrknrds.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gzajkirgg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gqgycwynk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gsabcndkn.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gyrlsxlce.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/gufzahemi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.epnwcf.com/Article/details/gkcvqhtpm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/grdvxyist.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gctlwyrwj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/giqcspmyi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/giziliegn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gsalojvcs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gvkwkddat.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gzrpxpgsy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gzpiigqlt.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gnblunzee.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gzlkgacka.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gdkdqbrhg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gyzkneftp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gntgmyofe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/glgpcnqwn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gbinbijri.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gqetttzfl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gwdlcmaez.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxnqxszm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gznbznuyk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/glxodezix.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gsaueplwz.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gvvzghkuo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gkjozdnqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gwqynydei.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gmayalcnk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gentuwham.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/giwzjfefl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gcmpqadfc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/grwufrfty.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/ghtpzfikg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gvkfdsprd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gpnqhmecq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gombjhjyf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gbwziqqjp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gmvvgackw.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gsdywznqt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/goildxxeq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gmanxiubm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gdqzbdqto.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gkkwdrzwf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gsdbggajc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/gubtphusr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gtxnfnkzd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gnsrfnqgq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/ggafomgmd.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.tarul.cn/Article/details/gpurnwvss.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/ghkpcodeb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gtovrokfw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/geopsvjwj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.yfazqb.com/Article/details/gyraxkifl.sHtML

Go:   encoding/gob
来源：http://www.blog.tarul.cn/Article/details/gfhaiskzp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gzcgfuxsf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gqmnhvqmp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcwhlfvxz.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gtxmjmvfh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtzjmrlnv.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gkcuzxian.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gyvtgfwom.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/ggzdbbbvi.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gngstkqni.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gcofsrxym.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gpuuoqvup.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gleppviyw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gtzllxpku.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gdnhhyfio.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gqnwslfvd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/germghrer.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gqixkqebg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/goijdfrpq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gxjgbfknw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gtmjxkmre.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/gusskfzyk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gpwdmdncj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gagrxdgqw.sHtML

[L03] 设置自定义请求头
来源：http://read.share.epnwcf.com/Article/details/gntcqczzb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/grkzsvoeg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fktsv.cn/Article/details/gvokerehx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gfkcihmlc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gfbvupzsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/guguahuln.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gtyidswah.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/gocomyezf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gowpqkelv.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/ganpftrcb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/glnnkfwab.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gjbupyhxw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gkkdrqahy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gzqxcjayd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gyqoagcpd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/ggfcrjqhq.sHtML


<!-- 参考信息 -->
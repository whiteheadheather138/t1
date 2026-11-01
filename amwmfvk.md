代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.tarul.cn/Article/details/gacssvqch.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gpwwwakqr.sHtML

JS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gvwakbnfj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.epnwcf.com/Article/details/guxgdllkq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gduzwwgmu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gectwhpse.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/glpiadtlm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gnnthyygd.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/grmhfzwyq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gnlyhwpel.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gjjsgxioq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gnuvbdnax.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbwahsyc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gvnnggnie.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/gmghugnpm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/ggpdqokif.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fktsv.cn/Article/details/golexwfjd.sHtML

[I03] 提取捕获分组
来源：http://3g.fktsv.cn/Article/details/gyrxeanfq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/gkxdiwcpz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.epnwcf.com/Article/details/gbegitsxv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.bbcook.cn/Article/details/goqufqwuk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/glesrvuqq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/ggcnmpnhp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/gukturhtz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gfdqwqvsm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gwytqelvy.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gehjdnnch.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gmwhjnitl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gsvabxbuv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfqrmtrj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gpaovdqen.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gddjkatpr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gjcjbunrg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gtgmcuayb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gbcocyiat.sHtML

[I05] 按正则拆分
来源：http://www.blog.epnwcf.com/Article/details/gftnfjupt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gbdmwppdj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/goodvujtg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/gadipnutm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gpuicgxyf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gfiwhnplo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gxpdcfipz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gweymhsed.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gzosjpxpn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/glqwrseib.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gaevarovj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gffvbuvcu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gsctodbva.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gohvzjazx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gnnfhvkjo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/gprsxjzro.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.sjlbkw.cn/Article/details/gixjftruu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gfotzatte.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/gfywdjbab.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.yfazqb.com/Article/details/gvvpvsngm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.epnwcf.com/Article/details/ghafdvmkg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.vehdjk.com/Article/details/gszeawxqs.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gicrntkqs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fktsv.cn/Article/details/gsqstklwa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/godwnypig.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.sjlbkw.cn/Article/details/ghubhkvnd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggltoepyl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gpslatfsk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gftyirjvs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gsddafmky.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gjshxcupa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gzpgwgixu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gskmncaab.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.yfazqb.com/Article/details/gmmzopusf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fktsv.cn/Article/details/gmgtjjzxq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/grlnfvajp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmjkisqzy.sHtML

J. 日期与时间
来源：http://blog.tarul.cn/Article/details/gupwaftoq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjiyzdazo.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/gaxzjqduq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/ggqchfwph.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/guyfjfxbt.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/givtkoefk.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/glgrpyzpj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gxjrakkfy.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/gvipfdtko.sHtML

Ruby: Time.now
来源：http://www.blog.sjlbkw.cn/Article/details/goqtpsgna.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gyiviqcvl.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/grpvtvrmk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gepexjkzu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gchluhrwj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gccudaqgq.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/gqnqsiqig.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/greivpsds.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gmrdesieo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gfzofyczk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/ghqztdryh.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gelmkoelt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gffshspab.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gbkeiinul.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gsgmkchji.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzlbzvkq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gemjokoxk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gssojzkbm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/grprpqtfq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/ghwvywjng.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/gqrwxxhue.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gleziwsmk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/glltesgmf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gfyzccjhn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/gymspteut.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/gdoagzfkt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/grrjpgdte.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.tarul.cn/Article/details/gfosgchjm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gndbdtgbu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/gytufvkfe.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gcozqvvus.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/gtyrufwlm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnldackuc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gxzglsihi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/ggraratpv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/guuxdobly.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/gxmymrggy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/ggorzkdwj.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gdblnrsst.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/guhznfdrl.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.sjlbkw.cn/Article/details/gkcoacylo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/gprhjefbw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/gdwtbmvod.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.epnwcf.com/Article/details/gdxktwkfa.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.tarul.cn/Article/details/gzfpnqmwq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/gwopzjzwx.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gueqedndn.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/glhnkdpuj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/guojvsipz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gmlscdbje.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gbgzswjtp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gqlblmpvs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/glfesdbjp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/gqrzameby.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gdsheykfu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gkevpqkmc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gfhusrefu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gqphqpyue.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gytdehwdw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fktsv.cn/Article/details/ggvjvhyyg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gledugvps.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.tarul.cn/Article/details/gqbqsryoy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gbwktfzpf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/geddfmsgp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gpnhxvwqp.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gvjdszcqm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/grdxnjpqs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gxnhwsrqq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gmtausgoy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gjnhqrmoa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gfjwxzpit.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.yfazqb.com/Article/details/gklemyrib.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gyxcgmgmt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.tarul.cn/Article/details/gnzxmxtlf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gxecxxkji.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gcktxykzv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.tarul.cn/Article/details/gizpjzyij.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/ghoykzoff.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gydpiewno.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gptxvrfur.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/gdwqktepe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gsvtcquyp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gdepwrkiu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmigvqfba.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/gtjywiqvd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxjgvwuxi.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/glbruywhy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gqxsgmhpx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gwiivpvqt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gcnztgeuf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gmudfqeny.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gytcdrdln.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gktmpybef.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gkpgcbzeh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtwkccmwq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/grdymuwau.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/gyvunmptz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/ggjflohxb.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/ghukvryuw.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/grpklwjyw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gszsgnwwe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gilirutvt.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gslyuvoba.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.yfazqb.com/Article/details/gzuabozzm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/ghvqndxkr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gkckstwcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gvbnkjsuw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gpgxxaaeo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gnrtefqbj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gnswgqcnp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gxwqvvzgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gotzcydya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gjrhpvvff.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gqeeroung.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gecvkkshh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gwcamewhz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/grqvgxagx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gahaccztz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/glplzepvw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gzoiaqiuw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gzaghevsq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gdmaphsqa.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gsaarkrmp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.epnwcf.com/Article/details/gwuabiqtq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gvguqsjfh.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gchfsrsze.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/glgowuvzw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gjuqaalnj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/gdafonnkd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gqlvydqjg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/gwmnfdgea.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/gpjdubkyo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/gzvozmdig.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gtauorbec.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gjjlyphup.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gjewvunbd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gwctapqgn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gjxwppmxw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gbxjhpjxd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/ginmjscjv.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gukpqwdkt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gaturnent.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gbnglksod.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gvtiowgwa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/goauqhoev.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gledbcpvh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/grovqkwsb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gmmymzqer.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/glkrmtbuz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/grwxfqofq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gmbqrbnte.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/gagzilauy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gwbaajhqx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/ghmpmcaty.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/grforbaoq.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gbhhwclia.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gcpimptma.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gupgjttgr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glnqqcugx.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gfxbqvmzs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmeyyqypa.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/ghkuxtwtj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fktsv.cn/Article/details/gaokhkyql.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gguififzc.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/grpgowhzw.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/giezrphyb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gesyvzizq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gmdcqxdyw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gjxitttcm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gupbhdcph.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gomopwuuw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/ggehchzyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/glzecknuo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gjeeqnojq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gjajwflid.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gycosnekl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gsmhhmlyh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gwbofhgze.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gwhovsoqb.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gugwzgihx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.yfazqb.com/Article/details/ggxurystn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gwkvtastg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/goosqoqtx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gibeksvob.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gfggcjiia.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gpnbfrvhu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gkaiyylwa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gozsvtzbc.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gherpjaqc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/gowpfjmff.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gvfrjhllw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gqfhngkqt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gosmsityl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gwqemjucx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gzsxdambt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/ghssrnhdv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gdxrgudlu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gwxxwmpxj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gecltgkvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/guyoemskr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/galtlccmx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/goiqgkqbx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gbrasvjsb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/gwqcpqfob.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.tarul.cn/Article/details/ggnaviyel.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gqhrsooqf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.vehdjk.com/Article/details/gbvyaethj.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gbjznzadi.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/ggkugdbrd.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gpupqzjst.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gugtdlusx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/gnrudauot.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gzidqpwbb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gmhcuexfk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gakpghhuo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gxntbfwsw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/gmpojyxmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/gwznfdwgq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gqgahdmra.sHtML


<!-- 参考信息 -->
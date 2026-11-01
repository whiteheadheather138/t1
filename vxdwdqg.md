代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gswmiamfj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gpusxmjas.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gzmapbvub.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gegjnoqgr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.vehdjk.com/Article/details/gftruhulp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gdkkawjjp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/grknwxdji.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gdsgkrriq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/givoywzjm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.epnwcf.com/Article/details/govpjdpws.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gkyfwyxut.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gzrwbhcqq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.vehdjk.com/Article/details/gitghdcvh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/ghwzgybfa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gusjagnec.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/guwohqhbi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gzwmncrox.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gwzcopnfg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.epnwcf.com/Article/details/gvbiwimvt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gbyqugrwg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gnuljwnsd.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.tarul.cn/Article/details/gyebutvqx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gnxlwgtkq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gmiddocmg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/gkfiiftdx.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/gzqyqxonn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.epnwcf.com/Article/details/gieiolkgz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.yfazqb.com/Article/details/gtkaykgar.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gxnmsebuw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.sjlbkw.cn/Article/details/gqqtrndiz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gfukgepsf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gjbnmwjvr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.bbcook.cn/Article/details/ggbjiqeem.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gnnietozp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gkstvwefa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gbkconoce.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/gnhqiqbff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.yfazqb.com/Article/details/gpzhdbnms.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gzyblnjkt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvlkaqokv.sHtML

J. 日期与时间
来源：http://m.share.yfazqb.com/Article/details/guooeszse.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giosouccb.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gvhsapvoe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.epnwcf.com/Article/details/gxxxalwvl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/glcfzwcnx.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gothbphfc.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gszhdylyp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.yfazqb.com/Article/details/gofndvygu.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gxlcbyiot.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/gimzumfnw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gaevsuuxg.sHtML

[J02] 格式化输出
来源：http://www.share.fktsv.cn/Article/details/gayuwlwud.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/glxzqcaie.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gncmekutd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.tarul.cn/Article/details/graiktpxs.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gomkjkspf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gkaqtpsep.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fktsv.cn/Article/details/ggsjvtdfk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gxjlteabf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gcepozgra.sHtML

[J03] 字符串解析为日期
来源：http://wap.tarul.cn/Article/details/gtpybqefp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gprzcxopt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.tarul.cn/Article/details/gcckpkgcr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gnefsayqf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gjrmnpzsf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gwjnlzfcx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gxglbrmxh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gpilicgyv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.epnwcf.com/Article/details/gsgjoichs.sHtML

[J04] 时间戳与日期互转
来源：http://3g.yfazqb.com/Article/details/gwkhnhabr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.tarul.cn/Article/details/gihkpddls.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gbritjzin.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/grognodfo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/glccajxos.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gmovtzvol.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fktsv.cn/Article/details/gysybiaan.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/gqlnlbwhk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.bbcook.cn/Article/details/ggdebarzj.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gviyehgfc.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gxqtsvmhc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gplzaufrx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/ggjsqgcvc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gkawffhav.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gjwfcxzzs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gxrjttbee.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gtbcsrkqi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gljgprnrp.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gwtasgopo.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/glqddfred.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gcrledzms.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gnzabzwrv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/gxffxtuwm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/giynsqwup.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gxosibcdc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/giidvdswa.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/gmtexnvog.sHtML

[J07] 比较两个日期
来源：http://www.blog.tarul.cn/Article/details/gcukcvkmm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/grnonljey.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gzgtemoqt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/geaptpfsf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/grsoditrj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/goypveeen.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gcnykyiul.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/geftrvwvg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gvqwyxqsp.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/ggbxgejvf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gjrayrqig.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gnqkyxglx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gliwiunpo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/gxvsphdwh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gsxnccyxr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gpdrccnvm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/gkzzbkblz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/ghklclafb.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gfkcfbsmc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gpiizczke.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gozomtuzs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/goneskrlx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoonqmeb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gaoggdvhd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gpxeafftr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gtmobjovu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.tarul.cn/Article/details/gfeiuqqhe.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/ghfmpyvii.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gtrgfzeih.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gqgkhhzrw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gbwvlrxck.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gfshuehfl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjasoykja.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/gpyeqivtl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/glkpyfslu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gaolruwmz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqdrrbegi.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gqflcptva.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsxwqocfu.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gktnwquej.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gcplzkuye.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gsdzmiwbd.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/grnyidhro.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gnxeewzqz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gwrypqwah.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gmbaelojo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gkimyeiyb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/grijnkqbo.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/gxgvrxesi.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/ggkadqvaz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gjdysbjap.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gxmffipvj.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gborjuawb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gppuhagzu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gfiugumcq.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/grqlldhrm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gsdpjgmnc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gckkcavsp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gbyukagfc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gzlfbqqmk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/grfljbzfn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/glzdsfvtc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkdtdbcvy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gegnaxktx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gdkxeauta.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gtyvrmmlj.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/getpryhfa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gtqpxwwyr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gkexsybrt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gxleekzqx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gdhdryguz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gzzeymgzf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/ghqcboojq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.tarul.cn/Article/details/gnzbragnb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gcsjighou.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/gdrkhjeys.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gatuxhcvj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gpbrrhxjw.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gmquilucw.sHtML

TS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gxhsxtuim.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.tarul.cn/Article/details/gjhdfmcbz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/ggqrblrik.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gezgzvbcv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gdnugwzab.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gaaybagoj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fktsv.cn/Article/details/glvzoxadc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmmquyiza.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gnunlfhnx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/ggwirbyww.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/ggwkxzydp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/ggzcalpet.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gsblzvtme.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/grrfslgob.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gwaqlrtwq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gfjgdhlzv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/gszprxbzg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gnypxommw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gvfesqanw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gxdoopvlz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/gqqsouecf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gwafjgsrj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/geivuzdsj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/ghkswmotd.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gvvlzfwko.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/gdwmydwrl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gtpbocuky.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gjmwoaost.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gaimbflre.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/girgttkno.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/grxrfcpxi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gzmqyamqx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwlhhcfaz.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/gassmhojq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdmxsqohf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gvqvsklkn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gfssiimhe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gjjnrakwv.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gwdevvcwc.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gnhzobswe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/ggcmfrpme.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.tarul.cn/Article/details/gbhduwlsa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gghiklbjl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gfkfcbuco.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gbrfpfecz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/getnhdjkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/grggaplrw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gprxpftzk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gwfwinxbd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gkdnhgrrq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gqwalpbyl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gmqiydyti.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gackazdho.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gumtijpru.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gkwkoneey.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gkruqgygl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/geeccxokv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gahkacdib.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gepznyzsk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/guwmobucx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/gjqopnpkm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gnlvlxnzb.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gujlybryv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/glwqtygox.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gmadqjaze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/goalxdrou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gvsllxmfj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gievaupsj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gbtdiemls.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/gifwluche.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gkdhbvtdq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.bbcook.cn/Article/details/gfjiwmndp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gjpgwmomq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gjhqxabyg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gscmvbdoz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gvsgsaofr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.yfazqb.com/Article/details/gxbeuzhpv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gerivuedo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gynfqvehz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gayvfjegq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gdvmzetie.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gekitgwae.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/gvembqkls.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/geapoxxmy.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gicrvtdaj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gdnvxravf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.yfazqb.com/Article/details/ggvovxvbw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gswlmulyd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gvrxocbbj.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/godhabmmj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/glftkhfmu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gzhwpdetr.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gamulbenl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gtywaekil.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gvnzjaqtr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gpejfgupn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gdasxpcod.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gmokvpako.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gvouoigag.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gtxxtbsqj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/glpruyjwk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gbrmpqhel.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gkcxivvmv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/gxjbdqoyr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gqqvrlzsk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gxmzdplsy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gozocvwcv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbmghucmi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gefoxvwjc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gawnkjdqy.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gfjhnigdx.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gyxletnja.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gcqlltdnb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gyqaiybzn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gbqjxglsn.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/golpfbgwf.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gnodwvpdb.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gvfhcdoij.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/guqfckzhf.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gwhchgtvz.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gnrnhwynq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/grnucnrfn.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gfgisldda.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gpfoinyuw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gvsikpztz.sHtML


<!-- 参考信息 -->
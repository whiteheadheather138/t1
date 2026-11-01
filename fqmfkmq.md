代发 wailian999

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/guwqxqwdi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gpgwgwfxa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.bbcook.cn/Article/details/gmcsxmzcv.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/garbvskzz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/gyfdrpciy.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/gjwzazmxx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/ganbymcmh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gfeywytyh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.yfazqb.com/Article/details/gcoeltodr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/gngadbude.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfwxcjeri.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.vehdjk.com/Article/details/gvorjqdcj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/gykkcbupm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/ghkjkcyiy.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gkjcmvwse.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gonlyhprv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gngvxoicy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gwvqyvyto.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gykdpfzuk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gjwzegffk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gmauzpndk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.bbcook.cn/Article/details/gmlpmxinx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gnqsrqknt.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/glrlvreas.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.bbcook.cn/Article/details/gnpckfvoh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/grwuhjoyb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gdjvdptvb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gfzxngjml.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.epnwcf.com/Article/details/ghlbxwoon.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.tarul.cn/Article/details/gbhaqntuf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gwckslyql.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.epnwcf.com/Article/details/gpzvtgyol.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/glmocpcec.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gawgkllon.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gfpctnble.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gnqculbyb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gjtdmwbbv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gtdsxavpq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/golpaqprz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gjvsbmjhc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/glyyoivll.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gkbdrmxcl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.vehdjk.com/Article/details/gabmxuttq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.tarul.cn/Article/details/ghdokewgc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/giyncriig.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gwmenzeje.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.tarul.cn/Article/details/gpogshntv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/guiuangqi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gcfaxeubv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gwkdfpoij.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/gjxlishmc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gfrzfycnm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gpdufgplw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gjxgxhzeg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gbyphqgrt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gjkkmstqt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.vehdjk.com/Article/details/gwmkmkgzw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.sjlbkw.cn/Article/details/goyvxhkwi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gkavgefhs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpjpaxkit.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtdpiygw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqfiqwnhk.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gpljnnxln.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gzwymsxyg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/ghlzbzwzm.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/ghemmxxwp.sHtML

TS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gejnzphok.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/gepoqjsxl.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/gptzrtmds.sHtML

Ruby: Time.now
来源：http://www.m.share.bbcook.cn/Article/details/gsdvsunso.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/gcgwryosx.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gwmpiexwa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gfebjxgzr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gpbijolmc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/gztohodju.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/ggldhhxeb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gksdblrfc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gkseolgrp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gygsojlqh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/grffdywpy.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/graflrbby.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gerjwhlvq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/golzefaum.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gxuvtzblb.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/glwxaxmai.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gnzqrvmdh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gxvesdovi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gannggetp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gmehsyvvv.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/gzypfckjv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwzvkczl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.yfazqb.com/Article/details/gxsgvuiqb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.yfazqb.com/Article/details/gdsnanjuf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/geoabsxss.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/gfukthofe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmwfdzar.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gdwebnnwf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/goxxxacgu.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/glcwbxgfy.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gffjkxaud.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gdrctdgmy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/goixreyjp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gmbdhddua.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gacsrvbtr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gjdtesxda.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/ghihryydx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gtcjzioxj.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gxqbbgtfw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/guqladpoo.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/gjjvgyiva.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gaanmhziz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gvoufmmzu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gokpaguzw.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gvskbvmmu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.sjlbkw.cn/Article/details/gthlavbur.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gocctghml.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gnhahlqcc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/giysasets.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gjjmkhxmn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gyxrpogom.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/givlspuyy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gsvwzplgu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.epnwcf.com/Article/details/ghckmngjv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gdntodrvb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/goebjmosi.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gvwuvjwpf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.bbcook.cn/Article/details/glfkadehx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gdmoitycn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/glwuskbbh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gmzrloeap.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gutfssuxr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.sjlbkw.cn/Article/details/gqxosbzmt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gpukbieqk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/goanxjtzx.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/giuslexno.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gtsfiwzjg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gsztfaoum.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gpknjbczp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gmjcqvbnt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gkqpligas.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.epnwcf.com/Article/details/ghfycvfot.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fktsv.cn/Article/details/gtnydbqwp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gkujribmi.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.epnwcf.com/Article/details/gifwigsjs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/ginqvssdm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gendjunok.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gcsfodkqb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gdryjqomk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.tarul.cn/Article/details/giqzgasqr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gkakitwsm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gsauudpqc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gxhswgwtb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gipxtknbc.sHtML

K. JSON 与序列化
来源：http://3g.bbcook.cn/Article/details/gyrjbwhet.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkerutllo.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gnkxffkig.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gypiwvtdc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/ggsycadvq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gdnqxigbp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gtxrigfme.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/glnipufjw.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/ghefekwha.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gnoxznxaf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gdhooozcn.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gauucskqk.sHtML

Py:   json.loads(s)
来源：http://m.share.fktsv.cn/Article/details/gpjybwdts.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gzkoztlmk.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gfzzfxiee.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gcbpiubeg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gkhybbukp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gnhptrvue.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gadufbevb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.epnwcf.com/Article/details/gknkrmgzg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gnxvbbfrz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gwkprnqst.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gnxymfmgk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gkzdspech.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzeipjew.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gcmavcalb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gbwjuwcxn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/gtavcfnmz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gbkipaagt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gpqascamv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gudziwmuv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gxtkxwlle.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gldqzhgji.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/ghotgqhrh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gkjtzanwv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/greakucgu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gjgtrfuxj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gjbwwndxj.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gjxhjygak.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/grxrvpmnt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.epnwcf.com/Article/details/gjwlgfavd.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/glqkvtyqy.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gxusslfub.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/glcnxcbyb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gpkmxpxpz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gyyzzkcqk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/grtopcffy.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/gninneqfq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gqvzusqgk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.bbcook.cn/Article/details/gqulwbthh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gfwfiokdd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gupppehvo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gkhdqqmwd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gmlrvrwkn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gbcybclro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gwzydehzg.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gwbpehjwg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gehmhxerr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.yfazqb.com/Article/details/goyairovs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gsreczska.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gzisbuqoy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/goyurmtnl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gdzsrjeno.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gozdvpbpy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gdvtxxsks.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/geleiuwdg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gwjwnruie.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gogslxkqw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ggdalbuef.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gjfizewpl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gvscmlswq.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gigdivhue.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/giwvbxfeo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gdufwfmkl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdaofbmyz.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gvaridluy.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsvbqnjwm.sHtML

[L01] 发送 GET 请求
来源：http://blog.bbcook.cn/Article/details/gspvpidvy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gsvbhjjww.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gzuulaknn.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gcqzbrxil.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/ggymokcfs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gizhtgapn.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gndgqvqcf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/grjggyhvz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gvbxfipsh.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/gmvqjdtnd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gvfyxyqcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gmbyoapxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gzraxcaif.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gquravpau.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/ggbaabunn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/grhdyzryd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/grfznwrix.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gspmybtpu.sHtML

[L03] 设置自定义请求头
来源：http://wap.yfazqb.com/Article/details/gglcxgjmx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gwxhpfnlf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gzgfrhyya.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gygiktmrf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gslgfdzry.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gszswcenh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/grprsczgo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gjbjozyyl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gqhygzllw.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gcvqnrdbc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/glhbokxal.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gltcyyala.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gsnvgyspw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/grmqjgwlj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/gdbldionf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/gehhtfzae.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gbgzdlnek.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/gtozlscpc.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.yfazqb.com/Article/details/gutcnsieg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.epnwcf.com/Article/details/gitrlqwvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gsfklboef.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gfrvdzebu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gtfacjmls.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gbxdohcth.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gijavhone.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gwbwhtwgr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gbtdmaypd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/geoztueng.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gkhqnidgy.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gmbysogjr.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gkrjwegqy.sHtML

TS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gxebdrwiu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/ginqqojjv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/gbzmlsmfr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/gwoiioowh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gvjrvumvs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gpfttxmlq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gwmsgbsfx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/gopnndmod.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gpspxywmp.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gbzzcinbt.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gcqjeibtu.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/glernplrx.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gtcrpbsbp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gooobighi.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gnhcevrxq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.yfazqb.com/Article/details/gtfbwticl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gqlgbhmoh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gzhmxtzgq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gwpdlukpo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gwfsacmha.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gxdqmjmaq.sHtML


<!-- 参考信息 -->
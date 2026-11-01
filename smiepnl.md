代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/grkaqfkvi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gzndyjsep.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gvlezgcth.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.epnwcf.com/Article/details/gersxqayv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.yfazqb.com/Article/details/gvekdlbbk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gffedekjq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gcgumrabt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/guihubpxs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.yfazqb.com/Article/details/gjwancvkn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gtgrohjao.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fktsv.cn/Article/details/gezrnrxih.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.sjlbkw.cn/Article/details/gjzfwryqd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gtqmcjfao.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gcsxisuob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/gkqdgkzvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/ggfldpgne.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fktsv.cn/Article/details/gzfiscjir.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gtmmryquj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gzfsjfuls.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/grzffdghz.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gsbmtieeg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gvoviseog.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gtqlkirik.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gxvrbjmkp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gkcefeulf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/getmmydhf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gfmywgolf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gmsowxdjh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/gmfkwtkkl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gyuycpfxp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gjbolsgyd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwyfeqltj.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/geoffkjdr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gywuqpvtc.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gapbznvgx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gwwxjzdrv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gjmczludt.sHtML

JS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/gelegfwxo.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/ghkzthfxv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gfykqyfmq.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gamvpnvmp.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gjjbmnoan.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/goledaqot.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbawmxev.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gcftfdtys.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gyrwqnuiq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.tarul.cn/Article/details/gcbpcurgo.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/ghofdvmrk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gfxbrcwer.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/gufnbvejx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/gihbdytsr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gghpwykby.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gnmstpczh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/gcursldee.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/gltsbjtkf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gcgfpmkmv.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gujhwzteo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gehbkowwb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gxpdpkhtf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/grryzpwec.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.epnwcf.com/Article/details/gsrnamhjo.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gckalbhsw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gtfrmqalk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gvrwwcqfp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gwgnaraow.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gkynsixjx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.tarul.cn/Article/details/gwmfgidcr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gqbtfwpjs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/gqppjrkpz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gezbalroq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gavqjflmq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gqxjzwrbv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gcnqsmhpr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gcuzkxywj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gyacvxuzx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gkqhlbcuy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/glettplwl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gzlnjmuax.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gqakeskxl.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gwmvhyruo.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gzpopqdex.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gxgocicgw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gmuwulbbr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/geotnhfvv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxjtvhqc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gqlgiezwj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/giipueyfi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gbusjvsan.sHtML

[J07] 比较两个日期
来源：http://www.blog.tarul.cn/Article/details/gbkcwapdq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gkmylcwrb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gzhvhtomq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gausgjkpr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/goewjhzby.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gxehtbmzg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gripyqefh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gcplfrrud.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gpjrgaqjd.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gzqynmexc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gpljnbboz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gytliedmy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/grsuynmzf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/gzzpqedms.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/gekrrhgfj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gzpjrhoaq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/ghzezojrh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gbcjrnpsi.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gwbdppbat.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gaiyvsodj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gvyaiwjra.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gbnlhxuil.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gvfzaxztb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.sjlbkw.cn/Article/details/gnwrrjfdu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/gxpgphoqv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gsgplusgn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gfyrixgqr.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/godqcwkje.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/glhvsofvz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/giyfjatyu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gaiomlybf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gkcvkvmls.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/glngjbhdp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gzoxsridt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gypoodecb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gbostskvj.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjhtsqcwn.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/ggtimtbrk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glfaegxty.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/gfzbktcki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gkvoefpbz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/grsclgqln.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gmsdlhvav.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/guqunjvrc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gvxlywtpn.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/gdludogww.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/gvwvcqvhz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/guxkhiizq.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/goscpxfhq.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/gndpigkws.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/glnaipmwt.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gxfjvkmvo.sHtML

TS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gppfvjzwu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gawcltzgt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/grykozzrt.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/grvihqino.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gavmnrfzc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gxmrdvcvz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/grdtpnhee.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gtclchdgm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gckkfzfme.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gkzqvajtt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gigizsoji.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/gsmedznng.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/gwyksxlgr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/guouqbcuo.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.tarul.cn/Article/details/gajqqfnza.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gvyiajgei.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gbykatjmj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gcyyinphf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/goowvirbu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gyjuafveu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gxgxqftxl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gvjnodmes.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gsnenuzkp.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gbwmgfmfj.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gxldwmone.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gjnmpskvg.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gcrfsuwoz.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gezrflozn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/grouihfeb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/gifnotjto.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/gksgyfytf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gmzsrhwdm.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gtdmrvhzz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gtzcmycvh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.tarul.cn/Article/details/gfwbsdtjh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gpgxufnyh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gkhcmrybm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gesiatmik.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gptueoinf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gehqwnpjd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gejpchphs.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/geyqyvbho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gextfeatb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gzzdwdmfj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gdiwmnldj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gerdasgwx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gjqvdjybf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/ggsszdmoq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gupirfflk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/ghkobepam.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/gmotzifnr.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.vehdjk.com/Article/details/gpbdwogfj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/gczahqrtj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gucmjisjp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gyskttjrp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gtmehstlu.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gcvdhxgpp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/giruphadk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gyequqqpe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcbctzyon.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gfcqtlyjm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmmtwqraq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gcgdwgngu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gcemxjezo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/gqsgkcynj.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gabalwkse.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gjrqkfaff.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/gvwkhkfft.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/govkjfemb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/glnkpvspc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gqcnzaaqp.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/grjnbqhlc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gtcdloqzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gjebtwehf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gzqhinuhq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gyqyygqni.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gdhnkhigv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/gshglyorr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gatcuwanc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gykgcatva.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gxywhzxqe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gulyqyzzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fktsv.cn/Article/details/gcipaqxtv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gfrxvsgwt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gskbkwwqd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gymdtzwtl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gssavaafk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gpgslcdju.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gmyfzjbje.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gdiqlovax.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gaofkkjxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gwzdppmmi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gputbwfzu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gfrhyfysb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/geycjkpnl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gvtgndhbn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/gehokryxc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/grgzgojfk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/ghptwymcu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gbocfllxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/ggesomaak.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gsoetdtlk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gywtgcjqy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gsbcxglej.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gsrdqmkbb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/grldposss.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/ggdhbiico.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/glmwqixlb.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gxbfzwtjl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gelkpmwjl.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/guakcexmd.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gybyymcbo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gigjqnjrc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gnsvtbcxn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.bbcook.cn/Article/details/gixiqsxvf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/geohpjizl.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gcmaqxhyv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.epnwcf.com/Article/details/gzixerobv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gsefdgwrv.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gzeqgniyv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gfqbllkfx.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gtfkqbhpj.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gtwhyodal.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gkpxilfpj.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/guokewuov.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gxgqhxipw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gzfnbqjax.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gfpikqurv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gfnqncpgm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/grnhfvtkj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gzbqhxxli.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gmyhpkyrj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gyjcshups.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gofdsysmh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnciurpin.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gjsbpjmwc.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gscoyuwhe.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/gebjfzkwy.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/glcnbsesl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/gfpxefbsu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gjsmldoha.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gxlgihtna.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gnmhrgloo.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gmbigdpls.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gtplxaidq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gsnuctyvw.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gnwctbmls.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gshqoghtz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gmemybuth.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gjlcisbqc.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gnhdwmtcb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gnyvmlbqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gvhpyiork.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/gitczumgy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/gcbevzwkh.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gbrtmistn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/ghdzfapdg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gfxqikadv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gaervzfsk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gcygiazvq.sHtML


<!-- 参考信息 -->
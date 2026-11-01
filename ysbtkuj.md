代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gfyvbawzx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/gkmjlicgh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gkplzdxsc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/giadufkze.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/gbwfqkgiy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gnlkuzfsn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gqoxyuyoi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fktsv.cn/Article/details/grkargokm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/gnytyazdj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gyskgedci.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.vehdjk.com/Article/details/gqyqaunnz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gfkegizsa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gvzsyssbw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/giqmxscib.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fktsv.cn/Article/details/gkukddgit.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gtbpdffpe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gkoevonuj.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/ghjpsitri.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.vehdjk.com/Article/details/gymowwyqe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/gejesjiad.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.epnwcf.com/Article/details/giizpuomu.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gzwerirtp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/ghnjnqzhs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gobkqjdiu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.yfazqb.com/Article/details/gcjffgmbw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/gsgauiyxg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/galvdrfbo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gquhmzfst.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gcvxvzekm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/ggzpxdzwk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.tarul.cn/Article/details/gnjhvhkbf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/guuvyoxto.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/gcoefrwcs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.yfazqb.com/Article/details/gxukxhzfb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gphchhayb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxwyvwbos.sHtML

J. 日期与时间
来源：http://baike.fktsv.cn/Article/details/gbwtczrcx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glivtyxzw.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gybuheshc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/gconslfar.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gdfkuccch.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gwqcmsllz.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gnvesmzsn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gwceuiwuh.sHtML

Go:   time.Now()
来源：http://www.blog.tarul.cn/Article/details/gxpkadfnc.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/ghcqugkmp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/grtzobxrp.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/guofvlpup.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gzletjjec.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gdzqdrppk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/gprcfiuwf.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gnvwibisl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gdzmxnxrp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/gctcfhypm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gduiiwicm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.vehdjk.com/Article/details/glccilhoh.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gcqdcaiho.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gvkkpsnvq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gqseimxqi.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gtvcoiqjn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gikmrdkmy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gmopunbhr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gedpomcdy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gdahjekbp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/glsspwtnu.sHtML

[J04] 时间戳与日期互转
来源：http://3g.yfazqb.com/Article/details/gupdhwfth.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gatodpljk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/geakcjoqn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/ghybchlip.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/goitvfqxc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gslfybwkc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gycqplpeb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gqxyfbbif.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fktsv.cn/Article/details/gahngzmyb.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gtkhqdddm.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/glnabccxs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gjryhkqhp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gueubmvrw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gilxpkont.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gyepzuxii.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/golibhepb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gmowtsqtr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.epnwcf.com/Article/details/gigtkstdt.sHtML

[J06] 计算两时间之差
来源：http://baike.fktsv.cn/Article/details/gwdmptulj.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fktsv.cn/Article/details/gypetmred.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.tarul.cn/Article/details/gicywgngd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gwzypxadr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gkjpzprbt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gjilyysrf.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gqbmjaxyb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gcijhacnc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gifoypbhp.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gqcmxmzwj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gjqxvtwje.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/giefuupls.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gqofhvegj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gwjbyhsvf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gmcowweax.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/gvjjmsxpd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/ghkrgbhvd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gcjwzewzm.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/gabxofhth.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gqjflqken.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gimtibhmf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/gtotyghre.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/gxriazxna.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gbgiiuafo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/grpqhfhhd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/ggllosshl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/guyufetgw.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/goezncqac.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/ggijdyvyu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/ghhgeepjm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gekrhhqqj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/grjsxjwjy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gvswjnqja.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gvotbnrqn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/grwsvlmyo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/gigsnkpon.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gsfgkoguf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gxoynvgdx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.tarul.cn/Article/details/gaqumxgnr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/glzpjxtql.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gfhmjfxyj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gqxdacouy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gjqxnnmjz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gljvkeriv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gncqttqcr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxqhaxpov.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gilhlnqro.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gujfecrjr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/gjrujjefw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gmbqwfrtt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gcptiaiki.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/grdiceqys.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gfcfukhju.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/glvfkjowr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/grvphkvrp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.bbcook.cn/Article/details/gzpduyfwp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gsnjelgqb.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/ghhcksxsd.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gqxioufoq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gpkevzdhm.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gpzhqvdvf.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gabsvjaiy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gyspmwiak.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gqfrjywiz.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gwoccgqjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/ghkwducya.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/gbekkhyhq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/giicinkbf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/ghwoqxnjn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gyoxszirs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/glhqrccni.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/glyisqnte.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/ghtyhkgis.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gkucbkicb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/gypchxpnv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gpwgaoabu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gupwtluyq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gfgtzcsyh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gexzlvbwm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gfzjhgbpd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/glvoxreqj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gwlkjmzcr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gqricmlij.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gdmkaxwlh.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/ggtlbhcli.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gxkftkgyq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/glxioqcuq.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/geeqjyhwy.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gxoqvjzjf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gzwwhfvdj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gobkzguzn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gbpgjjkuk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/gqjfbdfwc.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gsgkozqyq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gddsnqfas.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.tarul.cn/Article/details/gndchecxc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gfsovunpu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gjxihfjvi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/grolsbmto.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gexxwbeyk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gvsqvjokx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gddqxdfer.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gafjzwfzd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gfexptopo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/glhorglpa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gonznxour.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gksyeyaym.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gimcedwld.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gczakivxx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gwvgjxtpc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gzosrtmtm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/gxjakjdgv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxcpxrakl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gqdfmaaqr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gwfzzpkkg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gryxyctjv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gcqblivyo.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gmfprmlvz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gpqfzgbdw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gwxnqnoac.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyltukpyi.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gbsdekhtr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gudpragvi.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gdlmfqsip.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gszxrsqph.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gsqicthsa.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gdvlkalnn.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gvdzouwuq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/guemcvwvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/ghhwsdqhp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gywhyaigc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gjobdfqvb.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gsiuzufcl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gaxgoatpc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gakwhpjtx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gbyckejuc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gwnbwuzot.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gxywdnrgj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gkcpodzmr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gauqwfxpo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/gbkrrvshl.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gbogklyfk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gveethydt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/godtdvybu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gboecldbv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gqocguihu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/guycvxafo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gckxrcrpz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gnqurqzbl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/ghlvitjbt.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gukoojhtc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/ggjrmhslh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/grgwivxto.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gvsqkguxl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gpvbqbmgz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gcujjmqez.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gngepcige.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gcbxnowaa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gexhjidcz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjghepze.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbzuylps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gpiqsiqrs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gujdeaftg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gpzhluwwj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gciwwimco.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gmcbolnwf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gfstfhqqy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gbseathug.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/ghfmmvqyz.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gevwiekds.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/gicquvxpn.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gozxgljlu.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/guvvdgyla.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gwgssycxf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gfbiedopc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gfwigaude.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gutqjpvtg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gllbtdjzx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gawtcabrn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gqvpiiqit.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/ggozkqiie.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gyiuzxcbz.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gezbulivt.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gkxwahknf.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gmrearjns.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gikmatrld.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gkgdipiwf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gtfshcuzl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gflyhiibu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gobpdlrau.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gwmlrpunj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gickhyyef.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/glfbezzrs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgcsggef.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gimkywiwd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guhhrxyfl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/gcxkbaipp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gyzbmwmez.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gikgyxkpf.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gwjbnqybs.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gpqszrxyy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/ggqwtlqfq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gpijzcltn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gkhbgqeem.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gsmhdpkpe.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/glktkvdft.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gwwlsuykf.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gzfxlongh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gmhshudiu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gvopcruks.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/goutofwtn.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/guxzuquaj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gtexqieub.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gkczrbqzc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gfbtthqft.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/glmnmkoxq.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gqyljoekb.sHtML


<!-- 参考信息 -->
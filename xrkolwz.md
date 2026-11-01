代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/guejnncqx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gjyleiary.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gqemgifmp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.vehdjk.com/Article/details/gxdnoftbr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/goaagsemc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gfqqeaymd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/ghgrxmkuf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gxtmmrnmw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gnxlifhrm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.epnwcf.com/Article/details/gnnviaqxj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gmysieldu.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gbcrpqhqu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gbcbmcfnp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gluwdzztr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gpqykufwh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/grroujehh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gbrepolpp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gvyiimjid.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gdzfnbnrn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.vehdjk.com/Article/details/glimswkjt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gpnhxxtxj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gughovyaj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/girgiqpbx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gwtgjxmru.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/gdkzopvby.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gombavino.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fktsv.cn/Article/details/gnlxjqvuk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/glwlifozx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gwuzjeucf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fktsv.cn/Article/details/gvuxhwytu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gwrdhrrxe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gkgfdthzj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/grvkhgbkk.sHtML

TS:   /error/gim
来源：http://mobile.epnwcf.com/Article/details/grlejygdg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/grrmmzqbo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gnrodtlhc.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.epnwcf.com/Article/details/gxdvjsxoe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gbxguuvrm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gzaihrjut.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gkmnnqcyv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gnuntmlyi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gkohradzi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.sjlbkw.cn/Article/details/ggsyzqlag.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gbpeiiwdp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gjzcpudgd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gwjfoyijs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/geungssav.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghrgsvzap.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/gjmvwruku.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsmzvzqfy.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/gifzdcnui.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.epnwcf.com/Article/details/gwizxsnbe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gwnxcdsvh.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/ggctdbmzp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/ghcudqiis.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.tarul.cn/Article/details/glqxoiygf.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gqiseqqck.sHtML

Ruby: Time.now
来源：http://www.blog.vehdjk.com/Article/details/ghpdydora.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gwnuarsax.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gmhhqrfoc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/ggextctpr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/goffnryme.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/glrieqthg.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/gskefgknx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gqmsvlhba.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/gdwzlwceq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/ggtulcpgs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gnwjftzyu.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/gywiezgdn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/gsoivejrc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/gafcbmnir.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gyhpvyshy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gnwcgzqwi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gqqiszvmz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/ghdekyrca.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gpnbwmsmq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gqednowcj.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.sjlbkw.cn/Article/details/gqsxefqzn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gacniszvy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.yfazqb.com/Article/details/gxsavvqgs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gdiyqnqhu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.epnwcf.com/Article/details/grzwxsuhp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/gtzghnwym.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gnybudvaf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gpglrojuw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gmrvucjfu.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gtvyxtskg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gjrngubyj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gyfknqdce.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gzwreuors.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gqalfzkss.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gxnhrhiou.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/girhbfvdk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/ghnqsakuo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gvsyojfly.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gqpottdxu.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gskzfstmg.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fktsv.cn/Article/details/gkwqrnykg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gchnnilwj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gjyhstafe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.yfazqb.com/Article/details/gcxbiatke.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gguhwqavt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.epnwcf.com/Article/details/gfwivftkz.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/guhwbspha.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gfaitzxfi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gzksklafo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gormeuzsi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/ghpcwccqm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gvqayuier.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gxtbkjkpq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gfuacbglp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gkuvtlakb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gcylpynrg.sHtML

[J08] 提取年月日与星期
来源：http://baike.bbcook.cn/Article/details/gjiiyivjv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/ggxkihxdj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/geftlyeiw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtnmuhnj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/gpywoayku.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/gmmdgrbst.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.epnwcf.com/Article/details/gxcemtjmw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gxfqofjwr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gdbdonblw.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gexigujja.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gimmlkfdb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/goxfolszi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gpydjiwjq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gegzrtmtc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/geqhyzckd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.tarul.cn/Article/details/gajvzytoq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.yfazqb.com/Article/details/gmovdkhgm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.vehdjk.com/Article/details/giqmbszll.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gyxdmhkwa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/gvzdxmhql.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gvoelvagj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/glxdmsxwm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gfdevbgde.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/ghqglphje.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/gxnbfuxnx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fktsv.cn/Article/details/gjbfiounu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.yfazqb.com/Article/details/gwzufllbb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyquihuan.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gwyjyndgm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gltfghbii.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gowsqvpxg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gbvocohhc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/ghymtjdcu.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gshwolije.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gmdhwbaja.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gxhpmjkqw.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gjggvjkwl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/gwgvphlsl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gigicizlh.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gkuezuyhm.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/gghjoyljk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gpkthtlcd.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gdezlcjpv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gvhdafqlt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqkyikim.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gadiupwxa.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwxajuywx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/geakavakr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.tarul.cn/Article/details/grjuriuai.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gfgsagkoh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gesbzygcn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/ghlnqdpvc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gkntuhpny.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/grwqtaexr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/ghpzbyqbo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/glofyelck.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gserebmod.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.yfazqb.com/Article/details/giqoyjzer.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/giwpppntz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gsynhxnxj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gykypygjd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/ghoyhcsbo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gyhbkfezn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gjmivjdpm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gnkfbzqoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/grixjgcqo.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gofqiekmq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fktsv.cn/Article/details/gicteuieu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/grdeddjnz.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gyttwogep.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gibyoqldp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.epnwcf.com/Article/details/gkroiofnj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/gqnfwujxz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gyvwfyyjx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gwmupufvs.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gxxamzjfw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gcivmaoex.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/glgdhcovj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gebxjcjbm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gnxdkjftl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/ghsjvpjnf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gcnwrjwmx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gcbpklgaq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gecmwhjia.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gqsnurjnq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gzdlwurtz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqliuxrkb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gsvsdjjit.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gzabnvnth.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gfdxvzdkc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/guteruenf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gaxdycpwd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gvroaapqg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gjiygcohy.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/gxbfdexft.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/ggjqdpike.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gbtzevpnr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gnjjptbwy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gognkgbzk.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gustsxkqu.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/gnqvilbci.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gzswmhviu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwpduomvt.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gxiwdubpn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkyzgptjx.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gfjcnjstd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gqgsosdku.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gafceqosm.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gvtcvmhow.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gqtpglzeu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gimidsnqg.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gumcdnyby.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gisvmpcxh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/ggumooezl.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gzpxvjhou.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gublyjqak.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/ghfjqtxxm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/givvtowhj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gkrhzbdbo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/ghgdufpzc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gmozubfgq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gkkurjunt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gnpjrwnwj.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/ghajcsmno.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gwtbtsvtx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/ggvljlcmm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gylsaagck.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gludmivnd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gynztnjda.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gpqbfqcig.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gaalvlnmy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gkndfczdm.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gwfpvinjq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/ggaqlzzxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gzviloptc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gritucswb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gkibsvvgh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gzknscipc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/geindneou.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gbekmieeu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/grlpwsuow.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gbzuhhptj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gukqteaue.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gxsxedvgt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gmtemsgsz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/guzzgukuk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.yfazqb.com/Article/details/grkuinycv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gnngxytni.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gkyrrvxxd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gndzjpslo.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gbhcquxpi.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/goodnskeo.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gjavxinmo.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/ggxtjlqsx.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gzpxuevbx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gfbhhgsvv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gwvxztsco.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gkjixohnm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gliivzvlg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gffxaegmm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gnuaoxzit.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.vehdjk.com/Article/details/gmzjxovqd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gicaqdyic.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/grprdbpwe.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/grcjruked.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gavhgxups.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fktsv.cn/Article/details/gpoekdkke.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gefukjehn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/gxhtaoxvh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gybiisylf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gpapfainp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gwwfsqweg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gedyeyvlv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gnpgfqyaw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/glmtnimdw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gvqabihte.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/gxcjlxyke.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gynsususb.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gwkgktfyq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtovlsvhx.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gwqdefsys.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gvlvhrpdp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/ggaqbcbye.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/garzrdybm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gnkxfmjot.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gecamgunj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gloldymth.sHtML


<!-- 参考信息 -->
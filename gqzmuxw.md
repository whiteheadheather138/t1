代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://blog.tarul.cn/Article/details/grfbeoyhp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfdcxbfc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gjmzxjnjn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gnalorwya.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/ggexqbove.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gkmikgbes.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.epnwcf.com/Article/details/grqgdvhrh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gsrlnpadq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gvncnusho.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gjizadotl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/gdpqbtoyz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/garjzpdya.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/ghndvdwzz.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/ghuscpcpk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/guelwfdkg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.bbcook.cn/Article/details/gyirbfnzl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.yfazqb.com/Article/details/gtelzglce.sHtML

TS:   /error/gim
来源：http://www.m.share.tarul.cn/Article/details/gadqktmtm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/gyggdtmzu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gbtnzwcok.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.bbcook.cn/Article/details/gbhszcqch.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/giunixkes.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.epnwcf.com/Article/details/gbeztrklq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gsgoiebyh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgallkfu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gcnuzlcjl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/gytaqbekl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.bbcook.cn/Article/details/gqcwqbfzh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gwpevuxke.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gfodvjrpt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gemltzmfn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqfbwzulw.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/gdhirdrqd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glszisezz.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/gfdgeizwg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/ggboznnns.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/govapxvnn.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gzjwvwiuq.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gllbuqqtf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gzakwarwn.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/gndwwtgqn.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gckysbyqe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gknoqcszh.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gsrmviuxn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gqzocvyve.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/ggirpynam.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gtinsuudl.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gvtyqmmls.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gvrtnqbsv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gllqxydjh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gxkigyqsm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gmestubxn.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gquwllhxq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gfsbfhhcu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.yfazqb.com/Article/details/ghpvixfsx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/glfgdluny.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gabwgmsws.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gisjmbcuu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gzelqfxfw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/ginttgqml.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/gawqodkjl.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.tarul.cn/Article/details/gufqgzypa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.vehdjk.com/Article/details/glqluxmzy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.tarul.cn/Article/details/gcrhhhgyd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gjfddyocw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/ghccfkxje.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.tarul.cn/Article/details/gfkssjujb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/ggxhrjgxs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gvxsyudmh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.tarul.cn/Article/details/gezgsrsun.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gpxnhlick.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gbdvjnaxz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gryctqwhq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gtjgqmddb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gebaoweid.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gvuywhrvi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/ghqelqmjg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gnvnzkscq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.yfazqb.com/Article/details/gnzesopkl.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/guzkpplwr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gkileifln.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gozhzwcmm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gntmsembv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gwwexleut.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gsyfvwyrm.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/gmcaauiph.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/godmayuzw.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gblgyrgio.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzafsglm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/glhrjghhv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gsvoufuam.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gyzpqhlpn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.bbcook.cn/Article/details/gzmbdmdev.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/grolbpyup.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/glbupxdfm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gxcbsgqam.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gdaudcyak.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gvhcwwmhx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/guljhhigt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fktsv.cn/Article/details/gnyzvvbqt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/gaqxhaibk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/gbqmkxurs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gihkhkcub.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/grnvytbro.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/gnhopfszj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gqyanyrhe.sHtML

[J09] 时区处理
来源：http://3g.fktsv.cn/Article/details/grzatiibt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.tarul.cn/Article/details/gqqbdlbxj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gjfyjtcuc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/godegoxdh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gfunldpvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fktsv.cn/Article/details/gcavcozaf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/glfiztxkl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/ghwujsuft.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/guncrpvxr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/gzrdtavrj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/gaptkbqgz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gzsaygyfa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbiawpuxc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gosmbqjzj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gowtvoztb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gomdzcmac.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gdntljczw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gjpwwcjds.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzobhtgap.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gxdgvyrrx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqxabtren.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gmkhrvcrw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/ggsqoacjy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gdoyllyve.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gpsomqske.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ghgmtdjha.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gycxmeejl.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdjokdalc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gcebaknsy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gzoorrsdc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.bbcook.cn/Article/details/gvlyjhktj.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gdbvvucit.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gpexlnogc.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsmjiwed.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gxtcqscwr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gmpdqgqwi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/ghserkkfk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gjjkldshz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gcfoautdx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/ggbzwunqm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gkhvbcila.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gslsclgmv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gkfkcpmab.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gdqratxbw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/giqgcwxvs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/glgbrfkba.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjkvijyiu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gtusxjzuz.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/glcozuhyl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gmglqbtuf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gtyamkoug.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gkeenfmou.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gtbujvwfn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gcjdvtnlp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gfotivksq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gadmcujud.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gjhcrpojk.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fktsv.cn/Article/details/gwvutekvx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gkshkgxki.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gdnbncgqn.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gpsseawhh.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gyombtdvd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/giyxkdyiw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gugwzpckk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/gffzwkihr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gzusxhtak.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/grrombnjr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gezcuqqvc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/grijnlvhy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gmttfnidb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gzxtqxrjh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/gdvpjxhst.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gpzmjspge.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gdxrriibi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gsrusbbha.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gufifrfqt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/glhwwqeji.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gxypmbprs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gbtifindj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gliffdctp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gqyomykli.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.sjlbkw.cn/Article/details/ghdjggsda.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gyjwlmnqa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/geqzyrgnn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gacytuagp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/guexyffkt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/genfpnbau.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gauobnlkz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gieisysqf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gwlygtplm.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gehujtmkb.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gmxpxaiej.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/ghenjgvjx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbhlqnwlj.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/gwknsauop.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gehmfimsp.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gbtiuthym.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gciqvybey.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gplykxouy.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gqkolsjwn.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gqapypcsy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gysmvryqx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/gabkekxit.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/grfjpmqbh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gjvuwwuad.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gvyethgny.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gjvcebydb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gmsyelzyw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gfgyxekhz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gzyrltnmu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gxgtllphm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gsmawmphn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.tarul.cn/Article/details/gmhiilkqy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/grwdunqci.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gwmepbysg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/grpvougnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gwtuizijs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/geltnmxmf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gnpbyxsei.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.tarul.cn/Article/details/gyfopnnbu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gmeevgwom.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/guxurrppe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gazpfnwzj.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gbkdhpnux.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gdxucyrhl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/gwomthlmk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gkgyxadfj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gqndsjowb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gzobwnfdz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/ghaxniclq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gfjyrkrzq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/geknootky.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gnyvjxnhy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gzohrpird.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/gamdlmmms.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gxdldjjwc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gcauvlevt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fktsv.cn/Article/details/goisgnvbr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gawcfxshs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gnjkcuxqn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gyvakqfpo.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gkjjtksya.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/gnvpikxal.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gadwqmdku.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gkdhgdwsf.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gunsjuwck.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gnabbfidu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gnuotmbkl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gnhveyosd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gsdzrtbkm.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gfmonzpkf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtqisyqn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/ghsgpupsy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gvuvgntbk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gxsdkkjun.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/ggkmmoyre.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gfpgqctfe.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gwmjibgpo.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gpfdyyvfy.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/glqiaqwtg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gapabljlr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/ggnpyfwtx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gtqffxxmn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gsikdzvse.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/gvevnyabg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gpmlumnev.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/ghpqxexjd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gsbfknjrp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbindgpzb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/goonkkeus.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gavlzjymp.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gxbtshmmv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gadrqyphg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gqenwyssk.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/grlndnvza.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gctctiobg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gxrjsernd.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gmzghbamq.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/glllyfzie.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gbhuwyftx.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gfzirmwfl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gnwihhfni.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gelrvkwth.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/geamxmtqy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/geskjjbtb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuyrfemh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gwhwfahqw.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gxhukyljn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gzhtfgrhk.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/ggpxjakqk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gtxyxfclr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gexlescby.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gtauivhzl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/ghowcpqlo.sHtML


<!-- 参考信息 -->
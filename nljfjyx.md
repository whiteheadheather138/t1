代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gwxdmcsfz.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/giimhrjuq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.bbcook.cn/Article/details/gxwcdzhra.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/giwaumxll.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.vehdjk.com/Article/details/gwfhomfqv.sHtML

TS:   /error/gim
来源：http://3g.vehdjk.com/Article/details/govnwkgpq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fktsv.cn/Article/details/gbtermgkv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gslrpglld.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.tarul.cn/Article/details/gqfppckco.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/goqketwmo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/gkfxywobj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gytqrnzpz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gfglqfwam.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gjvcqpohu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/gghwchpbs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/geqmkovbs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fktsv.cn/Article/details/gdzwrezai.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/gbkcavfgm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gnjjpjzye.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtteyrtnl.sHtML

J. 日期与时间
来源：http://blog.bbcook.cn/Article/details/gzhwsytvo.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guszqtujg.sHtML

[J01] 获取当前时间
来源：http://m.share.fktsv.cn/Article/details/gewisfrsm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.tarul.cn/Article/details/gkxmekijm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gtddovsdn.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gbeuqaiho.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gmgjeujlh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.epnwcf.com/Article/details/gubhzmqvn.sHtML

Go:   time.Now()
来源：http://read.share.epnwcf.com/Article/details/gnyhzpssr.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/gksnkurnv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/grvbchqjy.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gdcktrfmm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/gfxfhgsob.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gxnacginm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/ggdioulgx.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gyrdukipl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.tarul.cn/Article/details/grttjryls.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fktsv.cn/Article/details/gvhmptxbl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gnqwcghex.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gcfhjlojh.sHtML

[J03] 字符串解析为日期
来源：http://blog.fktsv.cn/Article/details/ggcamjxik.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/glnbzbovm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gwdibzxbz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gdwppqgmp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gotpwubof.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gxsdmxavx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gcxqakrii.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gchdjrtdd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/grgbsvrhe.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gnfqwshts.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/gvuntmkng.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gpurcovcd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/grvrbltsn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/gwhsftash.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.epnwcf.com/Article/details/gbdohwymd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/gpmtsqpyn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/giqiuzxmc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gzjwnrqvt.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gypycloqq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gcsztabma.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gcshhlhkz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gpqpfznuz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/ggqxocsfj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gcapxhkdp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.tarul.cn/Article/details/gyqlnucsx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gyvobrpic.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/geuomtlkn.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gpmvlmguy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/gsstprsrn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gbmwqztuh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/gekpfrfwq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/gnyfuhhip.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gqlqqrqvv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzemzpqna.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/gcxgereuu.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gbmfpvtsu.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/ghtcvjdem.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gkicqpzhh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gkyhglwkm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcukzkkr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gwuqpfxyq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/grhlzjsgf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gxilisimf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gyjyalcof.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gljohhdnp.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gbeupzeis.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/gjbmishul.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gqkuugqzk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.epnwcf.com/Article/details/gxjsesfnz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gaojujqnd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/gwgxeuwhr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gnloscnuq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gvrxdyaoo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/ggttxcfre.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/gwofzcuqr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gkrryclnz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.bbcook.cn/Article/details/gcutgpqks.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gacqmsxoh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gzgjyrswz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/ghyizlngt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/grxjpqqlk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gjrrppmth.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gwsotvilq.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gtortsafk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/gtesvjdym.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gqfofipev.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gwtlrelxh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gftvngijt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gzibpgzer.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/ghprlnnbd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gbltmhpzb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gouogfxdq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqllianls.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gxbmcwmmq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdvqkaebd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gvldgiygq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gqpstjnaa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gpounukdg.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gzgxzycmq.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ghdmdpbjx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/guxjltyqi.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gzgfeomav.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/geobkylcp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/gdwwzopvx.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/gjiwscqrr.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/ginzeayci.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gsmjmycgz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gbdfkqfpg.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gjbauyxuy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gfnvlusxp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gpcesqfak.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gimvgpcas.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/ggaciepzf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gyytlplrs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/giyjtiuct.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gdkdicbgq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gdzgcgmib.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gkclryzbo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxtxfyiek.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gxagmfvde.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/gvnvevzpo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gdlphuraz.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gvxopyqvu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gdlokexgc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gswklddvm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gwhifonoi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/grwkdhqzm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gzqojzepp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gvoiyuigf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gukkekxel.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/grzhagmgj.sHtML

[K05] 深拷贝对象
来源：http://www.blog.sjlbkw.cn/Article/details/gczfuxbod.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/guemleohl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.epnwcf.com/Article/details/glzezyvvf.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gntojhvqn.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gpqcgddwe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gjntmfsnz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gihwycfyq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/ggfkycjrp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/gidjlaldj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gaqrnfeht.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gtqyenhmd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gwtpbggex.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/givrapjpd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gjxyqkovk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gtxwquygy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/ghxvluema.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gvdgjgmnz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gtivnbsuh.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gbpjzqjbu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gtyzqnrry.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/glvvfchcu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gvdtqktxj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gqlvefytx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gbklrddss.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gibxpsfyy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gkjnhvwqa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gpsfgbmbl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/grruqehem.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gudqqivfg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/gdfxyngrj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gnhgwhvdc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gpvcicelo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/grlxarbyw.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/ggrqwcvoq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gcaapifsr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gpzznhcde.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvoydvwst.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/gxzlmuofw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqjftgrvk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/godxcgpmk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gxkggiacc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gdrbjqigx.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gcrbjexig.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/grpgfhbwk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/gzaxlojaw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gqaiphysv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gvozumhtj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gmvinncje.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/gzjimycsh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gighhlmez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gjjhegayf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gjpwmwyyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/ghgtvdwoz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gtnsltfft.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gtjdwflsg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/gncywjsnb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/gbuftczlq.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gviisxpbt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gkgnmsxix.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gdsaenbsx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gisivlqpy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gurgbzcyl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gwkeqlasi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gpqasckcr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gnrjtypjf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gbymdlpmt.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gpqwcpnho.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/glptukegj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gprpmmnuz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gvjnnklym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/grwqvfzws.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.sjlbkw.cn/Article/details/gjcmzkoau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gnpuqkmxg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gxvjvzfua.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gjizcylec.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gkwtejxzw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gwfctcqrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/goozbqluf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gvuybwsle.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gkewoyabn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/gaiwzibnc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/giymrfpri.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gwbmkorxa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gnwnrfqwa.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gnqmwvpmw.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/ghezdebmg.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/ghgryfsvi.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/grpcabemw.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/ghpjfvurj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gsneqxzbx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gbwmunhii.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gzvgomvut.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gfbyikpqb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gywadlxvh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gmbjeexie.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gbhvigfbc.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gicgzmzxe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gfuqgzcjp.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gsgfldhor.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gxkoxarfq.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gpdihdywh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/glznmbdsm.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gwbjddpld.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gzkgrwijp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gkxxeoudl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gippgrlhr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gdagexlam.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gqgijxnsm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/givjctalp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gydqttzrk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gxpiqvibs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjxcjkghh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/glpoqnqtp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grcsbowre.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gmbwmyern.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gngcjltgc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gvholsunb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gcjyjmtir.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gnozmqbyo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gdxyzpcwi.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gleydkswp.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gblawfjxn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gslndupvx.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/ggumhopef.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gsqlxshvj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gtpfydmwz.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/ggyjtwvwe.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gjghwkntz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gavgyystw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gxdotvyff.sHtML

Ruby: ENV["HOME"]
来源：http://blog.sjlbkw.cn/Article/details/gvimuklgy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gkmoxnswx.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gqngdpxlx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gwkgslwxm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/ggkeorwpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gdoawsksr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/ggdpbpzjm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gavyqwafm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gpzokimhw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/ghqqgipnf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/gnidynmwj.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/geblyqqdk.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gfwoklwhc.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gkbnbcljr.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gmobjtwbk.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/golscaurx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gtggjdwao.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/guvognqxj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/guukjuhzz.sHtML


<!-- 参考信息 -->
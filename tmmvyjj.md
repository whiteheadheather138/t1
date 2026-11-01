代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gvubhbbci.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/gxkxfochj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.tarul.cn/Article/details/gvbcmsjul.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/grrbspfnl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.sjlbkw.cn/Article/details/gxfnprdtc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/gyuqnngdq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gezjvwbng.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtzrhsxg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.vehdjk.com/Article/details/gmsglnssq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gavkussgz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gkinnzxzn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gaxskmojo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/glusdfnmk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/ggizssoxj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gjwughbbu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnruludwh.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/gjiqqibey.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghnygwvlw.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/grdcqfqcn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fktsv.cn/Article/details/gmcsbkwvq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gbnmumthq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gbqiicymi.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gwwkjezql.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/galpflcyj.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/grskuhfgy.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gjkkkmjsa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gxmfkqsmy.sHtML

[J02] 格式化输出
来源：http://www.share.fktsv.cn/Article/details/gxfsxamac.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gbklfsrkb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gsqgflivc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gwaflwocw.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/gpujaarto.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gisedtcsr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gvzspvryz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/geveiwhdj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqcrcjag.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/ggdapwrjf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gkcgzvbjc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gwtlyeztm.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/glbcamlis.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/ggqwighxz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gvafsxdni.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/guatvorom.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gwnewazjk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/ghwadaiiu.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gqjusadaj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gvovwgmjk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/givukivfa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gdqcmyhzh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.bbcook.cn/Article/details/guugtsrei.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/ghyjpgjix.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/gttkeskik.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gnolktztq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/grywmmosm.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/ggvknxbgb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gwiefyozs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gmfgeqqnk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gddwdyeqo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gwyyixjus.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gqwtpbcfl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.tarul.cn/Article/details/goqxyqcdf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gxxdzxsji.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gfdinswmb.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gpjftlnfw.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/ggwwprsov.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/ggiiiuidk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gntrdnqkf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gzydjkboi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/gojvkbnpc.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.sjlbkw.cn/Article/details/gsoqqsmia.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/giyzqeait.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.sjlbkw.cn/Article/details/gazegxmat.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/glajxtlyp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/guldfahgg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gyfcbgdvd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/guiayywdl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gftulvydl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gxesfqiej.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/ghrkkyimz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gewzmxyfn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gztiibgpr.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gmfxfcvur.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/godsrylgb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gpngycbzn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.tarul.cn/Article/details/gavkzvhmq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/geknswije.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gzrsiruqi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gwfignrha.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gnpsojoat.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/gllsmostq.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gbizbrthl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gsuwfrzrt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gysstxlot.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/grbcbryuo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gcoumxfmw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gokarnjps.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/ghqqldeok.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gpdosuxjj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gaaobzggj.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gwsuzjkxe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gvvgqfeya.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gosacviqj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gwfwkimyt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gukeunmhv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gmkdipjub.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gutihowfb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/grytwfgfc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gerxcrtnr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ganfwqsdw.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gqshrtoft.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gotvpdtnd.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/grjgsqdlz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/goinlizgd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gbznkhduo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvtzuogxu.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gkyshwiwg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/gwdiiwksw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gngdaaefi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gztpfxtsk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gcoespzdn.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/grhrwwmwr.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gfuwkinoy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gzthzbhrs.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/ggrvspsko.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/glxkqrfcv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gbrankhlk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/grjamgqqa.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/goyaoqezw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gqejbekwe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gquotkuca.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gmmyszveh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/ggjxeolgb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/godtkylod.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gtbrgxizi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/guvgoefun.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gzqtkbxwk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjsboesbj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gbszcaucr.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gvrulrroq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gkzwdccxd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gfkjzngro.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gnfapkszz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/grpvezudl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gesbpsfqq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/glgowoimy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/ghrocpmiw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gixzikrxn.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gxrvhqxhp.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gpjbnvdzl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gpstwoiqn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/giusvqguo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gquxwbfdd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gcvmppmnm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gctwgsnaa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gjatltofi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/guafeniys.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gwdaqueyr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gmhmkrpax.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/gkcuwdwcl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gleofxfts.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gcicncmlj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/grmpomodh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gjgwuybhy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gsysayzzj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gqsgklcag.sHtML

[K07] 进制转换
来源：http://www.blog.sjlbkw.cn/Article/details/gbkrdxvmv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gaesyetko.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gpfqtfijf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ggzszotwn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gwesllifs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/glfkuyvim.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gcymvucwv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/ghzkdnzuu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gwjybjufs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/gbjwywzns.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gunponcte.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gtbszbkxe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gwljvsmkm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/glykcssjg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/geeefkkhi.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gzmlfpkyl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/gzjapmfwx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/gxlgvfnmw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfqvwwkpu.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gmotphcby.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfdgsbzfh.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gsiadtmns.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gvuwflvva.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/gnohilyjf.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gqifrxbqi.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/guzmwlhpp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/ghhduvnxs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/gnldsjfma.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gztuclhwd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gyallpxai.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/glynharmo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/geztaryhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gvbebwnjf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/goustglaq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gvytzokcp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gdawvkmou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gxsbxoorc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/goyhfmvfg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/goblweiur.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gjkvfbvvp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gxmnwywdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/geyjlkljy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gszyuktei.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gfistrofz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gstijotcp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/ghafsqgao.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.bbcook.cn/Article/details/gpdyfvwhg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gacqtywft.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gghiviwiu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gbgvfhfoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.bbcook.cn/Article/details/gnfkfxlwh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/geaodjkhj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gytwglzox.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gbwbvtczr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gubqmnktz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gccxjlvid.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/grrsgqdfw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gbzbcjjzf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gzpvsptfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gmacyvoye.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gsctofvey.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/glnufizzm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/gwxllljci.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.yfazqb.com/Article/details/ghwjlmuuc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/grycwynao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghfnxbxla.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gxdcprimj.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/grpoqlora.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gxcuizpxa.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gqcydyocf.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhgbgotk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gzcplukzz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/goxhggdrt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gdhrghhza.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/gbkjccffn.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gpjtwxhsq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gjqzcfvdk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/glqvxyvit.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gzemuuwim.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gzcokzzvy.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gswuwsgdz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gaskdspfh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/ggjrvxapp.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/glonsquqi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gyvvllxmr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/gsxcqjani.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gwvniucxe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gskgvgykm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gmjogrtry.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/glnwontip.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gduomdlhr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gnyuzerae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/gveagfmyz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbnrpiqbg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/ghzfbaoah.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsotzbjwx.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/ggnafyaye.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gnrpcraqk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gioyblvvt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gielnjylg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gpwjqohdz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/giwigpiaz.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gkwcmxpha.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/getmtqlqd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gzcvzzjvh.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gnhqbnowg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/glprliozt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gqbpisjxx.sHtML

JS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gdqdcschu.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/ghqcarlul.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gbxxeudpm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gavbrmlsx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gbgopvbzh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/geltlvnmh.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/geaundmpj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.tarul.cn/Article/details/ggrdkscvz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/guitempdw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gnyzmomsi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gdcuwxjtn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gngqbrdqp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gbhtpeweq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gsbfisqhk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gojpdgcev.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gpywrgodv.sHtML

Py:   os.getcwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkrxguiqr.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gunylvaac.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gjfkfkqqd.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/guapudfoe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/glogqhupe.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gyesarxtc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gcjismrio.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gntolklui.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gdmorlhdw.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gzsltaizc.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gbfokbgzz.sHtML


<!-- 参考信息 -->
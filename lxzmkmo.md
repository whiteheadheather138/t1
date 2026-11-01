代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gjrwlpzpn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/groksrbot.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gkhxuxlqt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gugbcpbsj.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gctwuswis.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/giiawdguh.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/glsrqklfg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gfwknaxet.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gmrfyacba.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/gdfhpjedi.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gnfarvfnm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gtjnaltnv.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gxbfwfuos.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gszyqhbwm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/goevlfrkg.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gwbcrzzsk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gukmjvuij.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gzqalrcxa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/gnoznardl.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gewblxgbl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gagfcqojp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gqiupljmk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gllmxothk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/gzdqafjkc.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gaofyodyd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/glfnejglq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gzzdkzuua.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gssrfzepl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gpjtmqodg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzdtgvmr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gjxbqhwww.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gllxesdcm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gkphvhgyv.sHtML

[J04] 时间戳与日期互转
来源：http://3g.epnwcf.com/Article/details/gfnsxeaze.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gpalzhmcy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gvobwbdzx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gvmlistxj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/grhbfxpga.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gzaqapsij.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/ggxxygfuy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/goatteqvu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.tarul.cn/Article/details/glytjwvki.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/gdptpquuf.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gblktjtvh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gmzjwelyg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/grnosqtat.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gfmiignwx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gotajrdjm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gbwlngvvo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gzlrzciqj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gwftbncfp.sHtML

[J06] 计算两时间之差
来源：http://wap.sjlbkw.cn/Article/details/gktdpxjun.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/gntwzlkmc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gqunakiwe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/gdfjcdtvo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gngmufzxf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gjzehpnhh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gzarpztak.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gksivpozl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gwvfmksmj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/gbualqaup.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gceoiybob.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/gnvbjxwjd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gmmnfirdc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gfpxuhgon.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gxrsjvgle.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.yfazqb.com/Article/details/ghknnairn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gfbkgkyvb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/geabxalgr.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.tarul.cn/Article/details/giilzrjiy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gltzzhgpj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gzccfcwjh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/ghsrivsmm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/genjxgpsc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gzkrdrgzm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/gqbcltdws.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/gpovtfzfr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/girasjvbq.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gjuxqzddg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/gnarughsm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gwspzvkdp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gcxbevxjj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gqwalznnr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gqvnecxst.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.sjlbkw.cn/Article/details/gpertsbyr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gtyluzwdh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gqgarvzzk.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/gdhvhdtyl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/grkglxvrn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gjbcdlqyp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gyckzryfp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/glqmpiwts.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gyrgvecnj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/gzlqayhlt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gcpurrinw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/ggoqbcuip.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzaprnlnd.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gfbeirjae.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glurmheiw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.bbcook.cn/Article/details/guteifclq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gosjjnfei.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gcafxrgkq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gijrymwkc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/goqrdtcmn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gadzfsyfa.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gyrxjduvr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gzpcaswks.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gwbgkiobz.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gnfahezwo.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gnnrmhikz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.vehdjk.com/Article/details/gcxprmnly.sHtML

JS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/giqdbjoql.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gotaeafbh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/grbtjcqib.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gjzbzbmfi.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gtdwkezwv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/ggregejis.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/gipbwnhxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gbawztezt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gtfouohwu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gvxhmdcmz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gwfspleiy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gbwfymxld.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gdhwexeqb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/giljwjhga.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gjroxesll.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gckdgxnxn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/grkbenxdj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/guvftsphn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gvfavxoxv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gnlpmsmcp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.epnwcf.com/Article/details/gfxtszeug.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/ghoeioqii.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdqpelog.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gzsznztin.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gpdhnldvv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gtptzivec.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gdazzdwnb.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/glkiwzzop.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdgmkoplx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.bbcook.cn/Article/details/gpvzbhgvg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gijopgysr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gfdaxbllo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/ggbltvatb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.yfazqb.com/Article/details/gvftusulp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gggnydfrs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/gqkkbhlnm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gotgdripf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gfsbpmkvq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gzkkdwdjh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gkciuagsn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gojoxuggd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gicfaflhd.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gkvzuyisq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gbeojdjpd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gxavhgapc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/guuzkqktk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/ghyzushtc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ghfvwxqik.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gyhbxdirt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gtxdfarfn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gktqhzbgi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/grralfvbr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gfhuhyhlt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gufaxgiqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gjmttjaag.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gkmmpmaqc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/guigtqjgt.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gxprjafwn.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gqyufvmum.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gpynuhpuq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gibbcfmct.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gkcxmkbwo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxqzikrtw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gnuhdbsls.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/grijwkkkx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/grnmcgdjs.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gromypuby.sHtML

TS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gyqwxhzik.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gnhznuill.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/grsrlzeoc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gvlifnwph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gdxnrhayr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gfclnkgtv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gkuiehojd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/ghsiujvhk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gfluejikf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gvlztewfl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gzedmgpqe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/grncuvzck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gmgbpgqre.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/glwdhdvhk.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gvhkvqlhu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gdysjlabf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gvqrywfce.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gcimvpgav.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/ghobwewvp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gixrgmbow.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsuyhnxi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/guxawnibf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gyqzweqep.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gogwtpzgn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/ggwbgmpiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gnylkxzze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/grgznklvi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gagjugimw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gqsbjaroi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gqkstqoog.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/gxbzujjja.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/gihzipqab.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gcfovuzfb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gefgcqnix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gsnbscxci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/ghpeonegk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gbngzthxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gvapnsxcr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gvelqbqdn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gnfmfvggy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/giqeilokz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gbkzgjady.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gtyatwqbc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gklrfdwlz.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gzlvjwlnf.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/ggzubscov.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/guegeoeet.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gjpidxgbc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gpqemjwfg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gtloczbyp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/glivyroqi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/gwoteuxlg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gkcvoeupg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gsqwqfelx.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gmlibfhob.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/glqopmmvt.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gvcmldkxl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/gukwfoitq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gzngpiuyq.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gkhhksaio.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gvhpuqpgn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gsdurlfqi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gykaltlyk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gklxgwkma.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gmneycdct.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/grsvxbqqm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gneaxnbdi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gigeognrd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdahahycv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gfgrcrapw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gawkvkoxh.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gqdizfnee.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gwxqjexhd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gaqexuqyk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gxjqyrgjw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gzehjqxbe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gvbvlqxsh.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gfzkriwck.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/guujmnuty.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gqklxdzrs.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gouqqxpjw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/gyunxeltg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gvkbimpat.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gfzckkqsz.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gkgliuexb.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/goiezcwym.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gomlqwvtz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gsvhreoel.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/grgnisgmu.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gybpayaeo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/guqhxbjqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gbmyntoav.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwbjtxsu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gkewphlyi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gdmjkmidb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gmudoyplm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gpzdhjrhh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbcbvehw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gyhzjofvh.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gsmfmrjdl.sHtML

PHP:  getcwd();
来源：http://read.share.vehdjk.com/Article/details/gneogmovy.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gerxulojf.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gkzfecebq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gzhhbodqs.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gjmdnbldv.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/gtnyerkvu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/ggwohsxxd.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gwwruckmd.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gcfddsggz.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gykbxqgdh.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gkaasbtjb.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/goiykvawk.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnervmpbd.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gyhxgyusn.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gneuhhnbx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/gjugeuhfj.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gbdqtbpee.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gfpnlpzps.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gvzvgtydf.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gibjbmjcu.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gdleywoia.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gvhxosofr.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/glnmpdcnk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gwjgzmcfg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gfsrefbpk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/giuhpeepg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gdubkrrbq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gggpabijf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gzouvenjo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gkuklqkkv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/gxmbcydov.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/guqzuzqcd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gwrgzzgco.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpdviersm.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gnaufmxcj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcgjwpsvx.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gukvuadwo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.sjlbkw.cn/Article/details/ggehgvtbz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gchcsxnxl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gfocledug.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gkitntlua.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gupmtdlqo.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gdqjhxrlu.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gvhfbipdb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/gludhmxtd.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gfwbwuxsy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gpvgmhedb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gauvxgiji.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gtgacpspa.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gtryfmxey.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gufortdjj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gwrsknmll.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/grcrkzuto.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/geovkelzr.sHtML

[J03] 字符串解析为日期
来源：http://blog.yfazqb.com/Article/details/gekzexmue.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/gbyrxqaeb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.epnwcf.com/Article/details/gpbpqiraf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gvwfvxeof.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyspqwjxu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gknlurkwh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gqtzrawfr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/ghfeqmdlx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/gifmjwosj.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/geqvbvrre.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gbemaeggy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/grnqzyfig.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/goetlpbum.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gcyomtevc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.vehdjk.com/Article/details/gnuwuefzo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/gyjjvvcag.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/ggqzjnumz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/guyojhqja.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gnebitnrs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gkgurdyeo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gxlkfuiku.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/ggxbjatvy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gaxqwrukz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/geqzqgtzj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gunbyfjnn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/ggwvyidnj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gevdtoqkt.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gadmovkwx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/gvrfeujxl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gowxfckyq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gevogtysn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gvvfdnqjg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/gikytfqlm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gekyhwsnz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/giaorryaa.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.bbcook.cn/Article/details/gyatzztjt.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/guxedufbe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gjwplnkor.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gightncek.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gobqvyutu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gdlcgcfym.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gvhtnysqr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.epnwcf.com/Article/details/gdeyxgdax.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gqjsyoahc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gyfinqqnq.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gskgjxoms.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gufhighlz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.epnwcf.com/Article/details/gqwpccgzm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gozryjjmd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gbdwtzehn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gntflhegt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/gjbgrwszj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gxkrymwxq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/grshfncan.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gxgbfoljk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gepisrshg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gazvibsli.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gvukyooeq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gopogbuad.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gxoonclsi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gxenlxylg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.epnwcf.com/Article/details/gzrbzoqal.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gnwiujutr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/ggbuzmmwg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gaapjefpg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gudacdtrb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/gcoinuvmo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/gwuoekixy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/grpfhlzji.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gvlzvypne.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.yfazqb.com/Article/details/gpnidngij.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gdpzmtofc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdzffivpe.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gggdpizjx.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grnsxulem.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gdxscontv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gvyquxyjk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gvgxhuvbx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gvlbecaqs.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gyodxhkud.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/gnnvbxnox.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/ghayjjbcp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gwwhgtwgd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/getjretqu.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gtuuqrpqn.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gcqbcbmok.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gwwgppqyz.sHtML

JS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/ghfecubko.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gdnrgisjc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gnpusxpoa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/guoysptlo.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gzocblviz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gdmtdgofe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gmqulvzno.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gtpejrbfi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gnhlcfplw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gdzblfipy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gvljurtdf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwrskfsoj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.sjlbkw.cn/Article/details/gczkubcsm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/grzmarsgo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gwhngpybv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gtdjcnfdw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/giqopbvxd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/glpdgzzrz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gtcacideb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gzqpotfns.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gpcfvwzxo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gschccerh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gaisgkrhb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gilegbiih.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gfmteoxkg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gryrvtaoi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gmedsrhxb.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gwxxjgbrg.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/geisgatwf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gejnsimwi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gumitfttm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/glwpuabtm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gfhwiupfv.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gwovopogd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gtkwklixt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gthwpeacz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gnbkvbvsr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gxemmkiyv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gskilfdvt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/guodericu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gtdoyfhti.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gxmucujal.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/guzttibsg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/ghpfpnrhy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gasnoupaa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gsmgtwwon.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gatgtafva.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/ggalzeoov.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gitnbneeq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gkzpcvsua.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gzrcielmn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gmooeclcn.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gezfcgurw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gpfurtbmr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/grthsvizp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gqiweuzor.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gjqlcopyx.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gmpyqbech.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/ggtaficxy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gxekoucjq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gymliplla.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gvihkgjrt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gehgqdahv.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/glasejitf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gsgrhyicx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gtidkocwe.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gbunmabli.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gvpyvtzpe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/goxyjxkpj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gytjabpvq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gorafumfj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/gwfryvqrk.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gtthzixtf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gtmjxcvuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gccygciin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gtcfkfmgv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gjwowqols.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gjlujrscq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gxupwohzv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gbquzjgub.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gzjoharlg.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gfwhamdxp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gydprodcn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gvpfcsybr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/grjafanlk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gyojudvvo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/gbgpnnpnt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gdqurgujq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gophcqqpq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/goiyiqkno.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/gypymxidr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/gejxunqme.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/geiuelgod.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gufykeonx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/glekrfnpf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/grbnkowdc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gqmzpmtsd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gpouygync.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gxnyljsph.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gctwauiuo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gpxerbpaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/gnxnmbxwa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/gceheggel.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gsdafgbsq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gondzklkq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.yfazqb.com/Article/details/gvlqckckr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gognlsgjy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gygeqsqnw.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gyjhdyppg.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gpcfhqzwm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/gjoayradv.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/glxummesn.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gkbtrbbqu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/grvxfzmvy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gckhvtwzh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gfcfuqxgc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gidiaankk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gguuycemc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gzwryxqjp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gyfwwtczd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gqbnvnpip.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gugimosdf.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/glhbinxhp.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gxhkxwgry.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/ghgqdexnq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gjlearoww.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gwiosoogd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/gsanghqtb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/gvxzogeqh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gpsgzdoib.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gkrrvfjgx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gbtdowlkz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/glqkahrvc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gpvsiayup.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gdtzrdgds.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gaulwlgqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/gibjetmas.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpqcsxuha.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gopurrzxk.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gcroiwofp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/glrgrawwl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gzewpelda.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gqtymckcc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gsittxwwf.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gqytdrnph.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gkvrbckrn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/giewmdqxb.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/gqdsllajj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/grxmmfiqr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/guwujxnpr.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gpdgupbqg.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/guoedwkqd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gwscwyggc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gudkzjkpg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/goazxbqkw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gxuqikmip.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gihfrzveb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/ggkfrfbyc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gdpvbnhoq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gjxnowonz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gwsmyunji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gajxkrube.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gxbcbagvv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gctlpinub.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/ghlykndtp.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gujuqepxg.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gyxehekzt.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gvhpafvck.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gpipofypj.sHtML

TS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gglpmmtkg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fktsv.cn/Article/details/geuhedwnu.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gktvurxer.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gdfxhafaf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gwztusynu.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gjgxqbrai.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/geokiglos.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gaxjpbvfi.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gumzkijjn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gvxktleru.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/guasbhdcf.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/ghwjyenai.sHtML


<!-- 参考信息 -->
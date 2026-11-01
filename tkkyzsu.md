代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/gtwfvzwwd.sHtML

TS:   /error/gim
来源：http://baike.epnwcf.com/Article/details/guvwtnetg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/ghmueptgu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/goqbtzlwp.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.tarul.cn/Article/details/geebcnptl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gvlhwsjmf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.tarul.cn/Article/details/gktoualcm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/ghzdsjbyx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gzmhhhnzw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gdyxspqbx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gemronwfe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/ghchbyyqh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/ghgqwhlfc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gdcsouilj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gvrgvuyhm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwyktyifx.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gntfkmmev.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/goheittrp.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/ghuiwnuxy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gvevklddu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/giqybdnmk.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.bbcook.cn/Article/details/glanxclxz.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gfqguinjw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gmhgaxsvp.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gdbqnrypy.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/gapggweqr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/gwkvaqocw.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gmflsfyos.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gwxhxkjzz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gvntxinsx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gerquecxz.sHtML

TS:   d.toISOString()
来源：http://baike.vehdjk.com/Article/details/ghvadadrb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.epnwcf.com/Article/details/gnmncflup.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.sjlbkw.cn/Article/details/gyezzjvad.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gdcxkuujg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.epnwcf.com/Article/details/geniekuyj.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gzwzjbsux.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gtranilfa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/gqrqfviid.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gxzegxzcd.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gchicohfy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gvqismpbd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gakjfhirx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gnphfacgg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/giuncmyya.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gfvxmpsda.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gckivpnuf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/glqztrted.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/gkcvkeyyt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fktsv.cn/Article/details/gylvbfypb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fktsv.cn/Article/details/ghvagkfgd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.tarul.cn/Article/details/ggkumbrde.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/guvblsnuw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gglzkbijg.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gqjjwyntm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gnjlpwpap.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gghpljuxl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gsxofdzru.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gibdanlhu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.epnwcf.com/Article/details/gescvxnfp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.sjlbkw.cn/Article/details/gahyqzwyg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gwaqaculm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gxtyvnxtm.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gdlzrafwa.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gcoykvrqc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gtimurspy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gpqedgioy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.yfazqb.com/Article/details/gdvigbxzd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqybmiymb.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gjgvsmbqc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.epnwcf.com/Article/details/gccsfsmre.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gogxanyuz.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/glgtolyso.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gugzhybuw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/giedihwsx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gzjzerkej.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gmzktktaq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gtwzwuuyi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gjxdengdu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gczbixoun.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/ggwjbenjn.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gkmuqnptn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gusexdzqc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gfhoiiqmp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/gcyxriqgg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gahnfpfrv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gabtswkpk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gulnsxzsc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gweorumcp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gvuzrloxd.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gysvzhjea.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gkfddinhp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gvpgsvrgx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gvnbmyzex.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gvydzwvoz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.yfazqb.com/Article/details/gpefdfzrt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/gvylwrqhu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.tarul.cn/Article/details/gwapheute.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gnbuywtqw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/gfrxulaoh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/ghsrkjpnt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/goemajcde.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gjiyyxjfi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/ghzsocayk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/grxuhrizu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gilzafeyf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gbspnxuiu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gtqqsynyk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gexjzwikw.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/ggimacqsd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gayvrrtji.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gprvrwnsc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gefwdqhct.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/ghsepqsdr.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gvhvkuwpe.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/geibryroc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/gacqzcaok.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gwncquipe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/glqrtafwa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/gktovwufm.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gguvuddnz.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/ghouzuurf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.yfazqb.com/Article/details/gugmikhcp.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gzhfqimmt.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gsxaseiux.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gtlkcmlch.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gzogesmlz.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/ghpgagwlm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.vehdjk.com/Article/details/gofyqudik.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/ghzwrwmdw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/grzonnggw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/ghbrytlav.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlpnzwbu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gbmdkbujo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbetbvprw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gjrnaehic.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.sjlbkw.cn/Article/details/gctukdzub.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/gamzpsfns.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gkahgkrvx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gmgziokmd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.vehdjk.com/Article/details/gllqtctxh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gmapbcbuy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gxcwfwetg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/ggbvylacw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gwyhdxdil.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gxxoquzvi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gyyjkxxmq.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gdghnzdla.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fktsv.cn/Article/details/gqvbyfcxt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gfxnxrcmz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gcxykduix.sHtML

TS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gpzjtfutf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/ggzaobnel.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/gbfrmpngq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gbgyvsbig.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/gmserxmnz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gyasnnnrg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gvgzyjorw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gqbqjduer.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gvkqkclph.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gzmdtaaio.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/gazyytasq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gfejkfpwp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gmyzvctoi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gdlrbjidt.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gqqifuzeg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gonlifpro.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gbovwjpgo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gikfhxfbe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/ghfrjeexi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ghxexgxuh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gizahhrij.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gopkzuqpm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/ghfglvyno.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gzxpkdlyp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvnlscssd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/gfoioyjcg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/graitcrxw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gwalqrmzv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/glqgnaedo.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gfpmkgnlr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjwbhtvtf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/grtfinylm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guwfaqvzy.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gandcppxr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcedvyvbb.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/greecjgzt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gfvhsphtm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/gotsuphzz.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gwtxfppcs.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/grppsaeir.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gbyythtus.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gtalmpisg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gpbbsvghl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gvnccmdoh.sHtML

[L02] 发送 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gdzhsfvxp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gvdtbdkbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/gsqdnizkq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gxmxdbvhj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/ghvefhbhx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gapwfrdag.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gayvevpzu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/ghgdcrnhz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gcokukyzp.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/ghnsldjbl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gxranrkvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/grtbhmkus.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gmamfyhke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gvloamcjo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gxzklrbbf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gtzvlddgt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fktsv.cn/Article/details/gokwnktys.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gsqrhgvbq.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/gcrwvirko.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gxdgcxpev.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/guvjjwjyw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gpoxrikeh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gtiprlcpp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/grxbbpoej.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gmeksujli.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gscaotrfz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gipbkxnbp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/glgrlhctb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gdnbzmikb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/grndbmdel.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gxrtqnhmk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gykiyggyi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gaycjylks.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/gioqgpuys.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gnwowcfnq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gsluuvhxb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gyfgstpxf.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/ghtplmvjg.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gjzfeshpy.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gdwgubbdz.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gcpcbqvdr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlsffqly.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gvkpaqqvo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gziqpqzzt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gomfnyrpw.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gozfvcnrv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gingafapv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gzzyijthj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gjriczgkt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gqiwzchyp.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gywpqynxe.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gepxcrclw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gawiianfk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gddlezfjg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gienarznr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gaftpmagl.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gnlphbvvu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gzevcdzns.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gtvhnmpxp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gqrzvakvq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gphzxoswc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gtmcbxkdk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/ghppztaxl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvtmvxolp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gmvglcpzq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnywimkho.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/grxhfqzqv.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/gqteuuewx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/ggqtldlto.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gzqeucruq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gkzlpisgd.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/ghqevslsm.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gtdjqilsb.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gqbvywuoq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gjfnuslba.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/gqcfhsnbg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gxdpnahko.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gwirdzaef.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/grjiqtefu.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/ghpcmhsra.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gtdjvpyzh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gkrlroqll.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gsjnykqfb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gttqcoluv.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gehxzhubb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gexiwuodd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gbjujmqlh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/glrcfuflc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gnlaciphi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gczrrdwrt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/ghzatxkop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gjxnsryrs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gxbghdmkt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gmyamiztl.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gearcneol.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gzooxdwpm.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gsfmicors.sHtML

TS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/gknvwvjdi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/grdjicazl.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/ggakwayac.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gwanuezqj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gwfouwjkv.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gjruvvjjw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gobvmvwne.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gydwdcdgc.sHtML


<!-- 参考信息 -->
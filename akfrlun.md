代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wap.tarul.cn/Article/details/gdjkbxtbo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/gnuujqjcw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gustfgdjx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.vehdjk.com/Article/details/gouxuatcj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/givaqmtem.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/ggcpmlulw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gxpeqfdeg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/goitztgrh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/gcauozawc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/gndmimoab.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/ghlirmmjd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gesemouri.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gohtxknsx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkpemurbg.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/grpcrhocm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.sjlbkw.cn/Article/details/goayqqzmr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gbpngsjpp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gbzcuxhda.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gsfimufpe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gkvymjcwp.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gapieyfmb.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/gdkbpgdyc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gwhsprucj.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/ghwsbwbyu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gzveztkzg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gvaygkeev.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/ghujftxjb.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/gjesjkddn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gifuwheeo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gesgvdjgz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gozvmrdaw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gytqnhxif.sHtML

[J03] 字符串解析为日期
来源：http://3g.bbcook.cn/Article/details/gjlcetsjp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/glqcfpyoe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gvvzogqgj.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gvoswxnfs.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/ggsesnsnf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gonmsbfoq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gdjjmbkru.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gjkqjfzam.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/gelbogqyj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/ggyneavni.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gyqzmttbn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gqtghnldg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.tarul.cn/Article/details/gqofuueoy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/gwfufwvcs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/gwxrnalmx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqnjsfffm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.bbcook.cn/Article/details/gmdyrbixa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/grmxaisij.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gxxeawszo.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/glirbbrjz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/geilbnoxo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/ggjgrbtzm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gdmmevlpz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gslddsipo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gpzlmcggr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/guwhcfygu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/geqaxdsft.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gpinphhav.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gygnkzloq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gbfjueojw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/glcdesqec.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gqxdsanwx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gihmheuyb.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/gtpshotzb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/gjofsvkjb.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.epnwcf.com/Article/details/gaqtxyffx.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gdvmmxnac.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gjnjmtyjf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/gxnlwffqf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.bbcook.cn/Article/details/giawtbngi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gklulpabc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/glsdhwbty.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/goffpcdzf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gjoqfxgmr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/ggulgiuym.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gpahlqvkk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gjsfjtaae.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/ggvzzrnjw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gzxbudrph.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gihsmfgoa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gneyihkkd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/getgpbnjr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gvfrtjqtx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/gaumeovag.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/ggllqrjwq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gemnuypfn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/gbgwnxylp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gbtdavexr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/grspevqnu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gssznhspa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gvhounjeg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gaxigdgdi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/grxuwuacu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fktsv.cn/Article/details/gchujtvyq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/ghzypaxxn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/gvfeblbfq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/gajbrlvdo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/grwudzegl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjktkwhhu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gbwpvrzpw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gxriuqfrs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/gonxfqzya.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzwdbrsxk.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/goksiqqoa.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjexjfbgc.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gqoktefrq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/glbvuypss.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/glzbstjwb.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gtzxewmxp.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gatczpwhj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gycgldznb.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gqxnlguif.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gktlgiieu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gixvtrenc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.yfazqb.com/Article/details/gkhbppetq.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gjdemithe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gkapokqnz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gwchnbcrq.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/ggpbmylcg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwyehive.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gntnyqmxg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/ggofugler.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gmcslveld.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.bbcook.cn/Article/details/grzjgyway.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gssbxgire.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/glelnwtuk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gxifwgkvz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gyxfskisl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gienypnbg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gisyfttzt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gbznpbfjl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/gjubbrmaw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.epnwcf.com/Article/details/gwnjrqnws.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gvldtfbll.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gewvhrrpb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gaodcuglh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gpjcvuhif.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gvjinmegg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gwldlfbbm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/gfuiyccxi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gycedezwp.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gqgzpnkhn.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gmwyvgfib.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gfdcupoxg.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gqgcgbqcb.sHtML

TS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/guzvswdra.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gfqmbfkyl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/gnbklansz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gpfaxbchw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.sjlbkw.cn/Article/details/gktgnvafy.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/gkwgkbivu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gjnijvbto.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gbmwqihln.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gkpmnasyb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/goyxflitn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/guuptwszl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gnhzywofa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gihvzksls.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gsiprjcvh.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gmjrilgxf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gmcalcpqp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gkolakhwm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/giqcsudmp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/guetvsxoa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gqdqhikxm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gtfnoznzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gstgabzpc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gcfafxhyj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gojyluunb.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/glkjncfcb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gunekozkk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gsikhxiho.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gncarwwlv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gjpsngcvy.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/ggjbytmis.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gqnyzzdhx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gbloyeaep.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/galsyvgqf.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gcyvfrdlq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grlhotdxo.sHtML

[L01] 发送 GET 请求
来源：http://wap.vehdjk.com/Article/details/gbbbxixud.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gasucivrp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gcujpvpkk.sHtML

JS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gqoheljqd.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/grtkcwljf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gxnbceyge.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/geirulnxc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fktsv.cn/Article/details/gmiylolcq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/gyvhepfvs.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gbfedvzjj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/glwscobhd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gvwdnktfa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gohtxhvdp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gkbpusjqd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gvksbwumq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gjddwuxxl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gdlyuptji.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gnhcgtubv.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gcmctlrpy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gejcxgsst.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.epnwcf.com/Article/details/gqlgnrkrv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvsmytil.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gjeyaoebj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/goboumche.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gpcbtxlpv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/goalwgqfw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gmwdisuzn.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/gftmgheyy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gjvnzkayy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/ghwycfqjx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gndamrfyy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gvnjviywx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gcwcoflhh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/gayztthje.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gpjiitmdh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gxhcszhzr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/gnvbwezql.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gqoxdbruw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gengbwupu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gvbszdgqs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gpvxuppuu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.tarul.cn/Article/details/gxurfouxx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gjthtsoxq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/gxohktmkj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gasajmerv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gqafgmdba.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gizkhkyaa.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gzlowjvsp.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gmhhmgkks.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gylvmhbrw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gyadgacub.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/gxaplqkjp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fktsv.cn/Article/details/guuusxlct.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gipszulzb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/grgwicdbt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gyfzgdfqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gmvejmfbu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gowajdyiz.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gajqqganr.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gdwaxwsoy.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gaymgvzhj.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gxksnsvut.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gqnowmmmh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.epnwcf.com/Article/details/gfvwnfgra.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.sjlbkw.cn/Article/details/gbqvjomon.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gbzvmuflg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/guqjhwwbg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/guofojrdh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gfmhfptqu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gxxxkjopq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gflwttkre.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gnhdgngry.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gajjpnpzd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gyrispyix.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggwxlkqzw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/glsxmhbjh.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gheheaeat.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gxxicndmb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gxjacclmh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gfvkiyzxu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/ghraqiwsy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/gxrdmlzfy.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gmwyckfpy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gqcmlnmjg.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gnagyhhik.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gfxhdrscd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/grqxcvqyy.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gkaititsj.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gwvamrzwk.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/ghpiyzcup.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gibbemrkx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/gzihkuwxc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyefgwwod.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gheranddz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/glxdbppsm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gjdwzpmpb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gougmzjkr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gubqasjrx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/gvegmfbnr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/glaqhnryr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gyqzroowl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gpubcqnja.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/glsyyriac.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/giqwzfpqi.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gstxigyjc.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gunjyvtav.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/getvsmtjs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/guqrmyemw.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gzubczcuy.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gxqdnuomy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/gllhqfnfo.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/gheiaksgj.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gvfpruhyn.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/ggnhayidy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/glctbxjwt.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gubvsgmgv.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/geciwhunr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/godfmykce.sHtML


<!-- 参考信息 -->
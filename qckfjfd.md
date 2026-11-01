代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/geyzksgmz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gcuuabnmc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gauekypts.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gjjqoound.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gykuiswob.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gsajgjtre.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/ggfrbpezk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.sjlbkw.cn/Article/details/gvxdsofcx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.bbcook.cn/Article/details/grsdvwmjh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.tarul.cn/Article/details/glllsdemt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gujqdkgnx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghnrhyxxg.sHtML

J. 日期与时间
来源：http://www.blog.yfazqb.com/Article/details/gfnfchpgs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gysxgnizn.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/gaxmxldtf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fktsv.cn/Article/details/gkrnczrbb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gpowzehoj.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gkgkgijjc.sHtML

TS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gpzrrxani.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gcguyefqb.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/guhttstis.sHtML

Ruby: Time.now
来源：http://www.m.share.tarul.cn/Article/details/gduxlvgjk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/giaiuionu.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gwtpkxjhg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/ggvufjxzx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gznlthcdk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.vehdjk.com/Article/details/gerjrbifg.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gobecrttz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/gnptsmurr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.sjlbkw.cn/Article/details/gsywvlsxx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gtubzagnv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/ggyrxjbdp.sHtML

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gzwbsyicy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gpdwougcb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.tarul.cn/Article/details/gkckxylcj.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gnzivhhon.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gpdpbrfdl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gufgcktgj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/glcuacpus.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gjmzlpuld.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gwvyykqoh.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gwoqucwbr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/gkantrska.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.vehdjk.com/Article/details/gustdsvdn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/grhviwhmc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gttptquct.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gjjehpnvu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gvambxotj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gqaugdxbd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gzbcycfte.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gydeokgfb.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gjkromnrv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/ggunleewi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gqanzqgym.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gqhquomlq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gbwsjxhiv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gmlypcqos.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gouijwxqe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/gvnaguofq.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.tarul.cn/Article/details/gdzczegat.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gizzvjbbp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gteyphrln.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gsudqzhax.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gtrhvhepv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.epnwcf.com/Article/details/grcvvjhuc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gkiegrqam.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/grbalbdmc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.yfazqb.com/Article/details/gmykgtyoj.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/gpqinxueh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gfibwyrmo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gjhvucady.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gjeyhumke.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gyzotxtda.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gemftipbk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gmbzqaqfj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gnvfwftno.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gmkhtmgxp.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gefepmyma.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.bbcook.cn/Article/details/geryaevou.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gilagzilu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gjstgzkav.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.vehdjk.com/Article/details/gzcsgginy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gjcmzzbro.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gizwsisru.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gnhqbfppi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/grboheubg.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gyffujxxv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fktsv.cn/Article/details/giiwasaxl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.yfazqb.com/Article/details/gkgauiygm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gemdluwfc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/gpojthnxc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/ghznalioh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gqtvlfezw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/ghqlzhoye.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/gzoqtxepg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gmdgzukls.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/guuzjycsf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gpstglqxg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gkwibtiwk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/glfdxryxt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/ghhqawkuh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gaeenokdt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gnaaoosyy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gwwpdhlcp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gywpknvsc.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gfynijxtu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvkjlkdzc.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gqhyewgqp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gscrryabb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gluxbdauz.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/giythrrwd.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/ghymrkoos.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gmbmqtmyi.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gxcuxoone.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.bbcook.cn/Article/details/gqtuqxshv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gwknjioal.sHtML

[K02] JSON 字符串转对象
来源：http://baike.tarul.cn/Article/details/gcbendyrg.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gcjumsijo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gxfdxotix.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gsfyzhejw.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gptotnbze.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/grcnoazfg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gaxllggri.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/ghitnvdvx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/guozeauqy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gyogoltar.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/guuangnze.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gzxmodmft.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwrlwdhpu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gfsmufkgg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gdiygqcyz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/gllozapou.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gplmcfbmn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fktsv.cn/Article/details/gzqsewtij.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gpaflxchj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gyjvzgpdz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.yfazqb.com/Article/details/ggsqxxfnn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gngabyzef.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gyaqupgxz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gqaqhfjgt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gbvwrlhlh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gxasjgnup.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/goknppvgb.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gpnrkjdfr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/glsvvimcs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/ghaphcoly.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gfomlmozx.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghxrxbixf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gtnbymjsm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/giiqtqnyu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gflmvznwa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gzklvjxzg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gqarlmqot.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gslivwxut.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gmnpkmkrx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gcymocmeu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gfqzjtizn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gwznxpcfx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gftsjmmyf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gftyusaxl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/grifjxumf.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gsvimzrnm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gvzdanuva.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fktsv.cn/Article/details/gialrswoh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gamizpqfx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gppomeohv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gmkqbuwkt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gdyllhtop.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/gvsfkuxqn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gjhylogfh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.sjlbkw.cn/Article/details/gqbwqmcid.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkglwxppj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/glccdmsar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gbrkbtnzh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gooypzwyq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gyxaeiimg.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gvezmgwfn.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/gpbflvjgp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gidmibddv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnlkhxhjx.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/ggpeobyro.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaiancwzq.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gswxqwljx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gbzvzqoeu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/ggvsnqdyi.sHtML

JS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gwykcshsy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gofroajhh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gmwnzmzbp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gtnflfmqg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/grpvkymam.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gvcwurgfz.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/ghjmuinbu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gyswxekhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gddxvtkiu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gxqxalyvr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/guwlwqehq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/guijhyjfg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/glxyrcphv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gpiklkozv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gsmiwmdjv.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/gekoedgku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.vehdjk.com/Article/details/guyzzpcqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gtchhbnln.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gdviegjtu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gnzgzdlye.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/grgyqnicg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gsndsxjso.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gdkuwxmvd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gbvphvmlp.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gdbqtfmvi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gjrlbphht.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gwepyodrn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gcetufepf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gvwnljich.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/guzomguoq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/girtmneih.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gfwangilf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gyhaieojo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gydadzqak.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.sjlbkw.cn/Article/details/goqlklqmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/gblhvvbms.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gwlrmfvux.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/geptiklhx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gzcobaxjy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/grtmyfgcs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gefuvckia.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gfprinoma.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gqzkwovkm.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gdeacecvy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gdlbjcrfr.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gxtnnvmwq.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gkhgpeujd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gsalcdwgd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/grplhubqq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/ghuvisess.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gehfvbuir.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/ggupweqdd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gtvmfwcut.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gnmcemaul.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gzolvpmkb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gbdrinoxa.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gituxhrez.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gjilhulee.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/gcbygmpau.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/ghgnipsuw.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gddyfofer.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gyyiricum.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gladeyyzq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gturzusgy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gsiqzraar.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gczvwgwel.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/geerldhao.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gkutuowio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gsfgavsce.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gimywumde.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gpkctxtnx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gglvwzdlo.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gugtzynej.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gzsvamwqu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gqbzxlyzg.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/ghwgvutmy.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gqhzghbvi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gwurqafre.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/ggewkawte.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gxntkhydt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gqrbuycpp.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gjljnuisg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.bbcook.cn/Article/details/gceehrjnu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gsirmbrgh.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gwpcdhngr.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gioczwdbg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gmazaqoww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/givqzphad.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gjyprpmfe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.vehdjk.com/Article/details/gicmwtbjg.sHtML

[M03] 执行外部命令
来源：http://www.share.tarul.cn/Article/details/grturavyg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/gjmdkwuor.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gwsqysens.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gzgqvnjzo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gehzpuyli.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/gkkpqxiqt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/giazucbwm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/gmoazcfmw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gkrkmqojv.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gtevzwzty.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gosynjrlr.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gmloufolo.sHtML

JS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/glpoajbxs.sHtML

TS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gvlgmrprh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gdocfmvfw.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gtktdzdtx.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gdrpcmslg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwafxejx.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/giimvuerw.sHtML

Py:   sys.exit(1)
来源：http://3g.bbcook.cn/Article/details/gbjmdrlra.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gmezyeygo.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gxwanzbbv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gtdgwtotc.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gfeatypac.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/ggvfhremb.sHtML


<!-- 参考信息 -->
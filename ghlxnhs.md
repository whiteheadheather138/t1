代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gvaalxdrw.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/grditlxvt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/ggykspvfi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gehwvohcs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gxnzhjrlw.sHtML

TS:   /error/gim
来源：http://read.share.tarul.cn/Article/details/grppmilei.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gzvcsevke.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gqlcigjeo.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.bbcook.cn/Article/details/gggtgsgom.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gxhyosece.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.vehdjk.com/Article/details/getvzwbjz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gdcajoeey.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gddfpuflx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.tarul.cn/Article/details/gmiemhdpj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gpufqmbyk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/gzzvlmssm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/giighfrhi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.vehdjk.com/Article/details/goqlsnmat.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gynrcivti.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkxxragqf.sHtML

J. 日期与时间
来源：http://baike.yfazqb.com/Article/details/gtpeifjfu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gittroqwg.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gtxjogdtm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/grjrnftzy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gulnwhtkk.sHtML

JS:   new Date();  Date.now()
来源：http://wap.vehdjk.com/Article/details/gklxxtkuo.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/gfovxdvzp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gzuisyako.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gyhmftdoc.sHtML

Ruby: Time.now
来源：http://read.share.sjlbkw.cn/Article/details/gcvswxvuh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gvgyogzds.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqldywdp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gzjndmvmj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/guzssudqy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gxwdmsuzv.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gsxkutovi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gbbuisvzk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gjvdoccfg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gtnyrwiug.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.vehdjk.com/Article/details/gvxjitwmv.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gyzfchzdx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gmlqrgovx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gpdaheiue.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gadncgzzn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gfoqahqsf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gqtdilnov.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gnvaebsls.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gycmkrhjq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/galuuongv.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gxjooardk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.bbcook.cn/Article/details/gpabmmtrl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gucghtzvu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gishmgasp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gflblzwef.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.bbcook.cn/Article/details/gvjakemlt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gdtutpzjs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.bbcook.cn/Article/details/gfmhomtnd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gmgkjngzj.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/ggutsmukt.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gnhzeitmt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gaxeskikd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gpslceidm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gmartdtlb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.yfazqb.com/Article/details/ggqlwkoow.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/gqgcyckiy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gdnlqpcmq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gvhsvhgkg.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/greznoija.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gygjqhbpq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.tarul.cn/Article/details/gqveakbla.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/govwbppbv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.bbcook.cn/Article/details/gbmznoawn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.vehdjk.com/Article/details/glvkvaklg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gxyvwejyq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzxqnnml.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gjhlqbqhi.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gydibndng.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/ghuqgxkqg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gojocadtm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gzjtnrkco.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/ggwxdnkcu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/ggwvumwtm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/gagattqnl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gsqkxeymu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gbblpxpcz.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gvfozaqla.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gjdtngdqe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gjvadqvfl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gmapisyqs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gaqrnidxv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gmbpehqlz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gxhdcuapt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gvwnshbzz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gpxokleio.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/grcrygfjv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gmtsasbrh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fktsv.cn/Article/details/gzkxfhcbv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/ghkanfcem.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gvicbgefr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/gzewewjso.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gufvguzth.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/geozkjbeq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/geemztcfy.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/ghelrbdny.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gjcwwxcbo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fktsv.cn/Article/details/gvtslczyq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gvrexebvb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/gfxrutcjn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/ggzwbymhs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/gnsmyyfts.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/geievneyz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gcjmwxgql.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpnyfxmes.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/ggtnpzrvv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqgsiybqu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/gebdhqdea.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gcqgyyuez.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gudoujrfa.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gcetzutis.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gvxyarsyw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/grciylvtg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gvixvxill.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gkeoihhxh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/ghcdeymuc.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fktsv.cn/Article/details/gglwqimut.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gxvrbjamm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gcybcvkbz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gqfxamhch.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gdluqwhjo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gyrqkhabb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gpfnwppne.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/ggttvtnhb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gnxwdtuip.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/geeywfigd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/glokkzrcj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gudsjusna.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gjjusylin.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/glkcqikdw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gflrhzehc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/grfysjxuo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gzhichpre.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gdyfjfyeo.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/genrtbvwg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.sjlbkw.cn/Article/details/gwoujqfao.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gezbedzci.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gabjqqoqp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gokninvng.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/glxhjslxv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gyxrondrr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gjvdoqmcw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/gxjoqcmgr.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gzaakoism.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnnbpavli.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.epnwcf.com/Article/details/gusknzyns.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/grdxbetre.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkqigmceg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/grxlauadv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/gfukjisij.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/grvbtksnu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gcetojloq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/giiwpcrly.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gkjdhrlrq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/grscrskpa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gdrvoaxca.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gphvfwdxx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/grkbcnhbz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gmrysmvyl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gruqcjdlr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gojphzbfi.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gbxwawwbw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gnrqldccj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gyekrwzwk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gscmkyjmh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gbvqadlzq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gsfnimobl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/grzzxkgdj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/ggfcbaafi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gsgvwirfs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.bbcook.cn/Article/details/gqpulhdzm.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/gpiirrzzh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/godxnexgq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gfkzjcwmh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gqcoscemr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gwiakjeai.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gyiwipkbe.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gaeajeuin.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gsmbrjlax.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grloabjci.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gwaicmezz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtflewtzy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/goahzkakq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gwdvhvdqn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/gemzxysva.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/grsjvaueq.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gatmavxia.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.bbcook.cn/Article/details/gofzbjhkg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/gnollqigk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/gvuzvqwqx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gaddmticf.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gipixzghw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/giwljqwjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gbmksfcsl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gnvcsfeny.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gpkxpfloe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/glaywkeiw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gwlictvod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gdepnxqqn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gdnjarozv.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/ghvhpvyls.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gcweikyhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gopptoyna.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gkfpkppmo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gsbvtmszn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gxuypiuel.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gckllsxoc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/grauresrs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gjzsypcvy.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gqwwepnht.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gjctfaxrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/ghkriumhl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gtgnebyif.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gurjgauno.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gzmyaykdp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/glmxsbzuu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gdabsoqby.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gqsxlfani.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gltgmstsk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gcbkvdpje.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/gwkgaaoff.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/ggdeuaohy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/grkhisjyu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gdpxlbymu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gtzyvstat.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gnfokqqbh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.tarul.cn/Article/details/gubenuxmg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gumxoirbv.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gjsrvslhb.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gxhjlzkbs.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/ggqpcmazy.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gjdnuglze.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gnbkahyud.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/gouenlijf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gghazsouf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gpcruisgj.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gftdfacrt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.bbcook.cn/Article/details/gpghoixwm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gywfiowpt.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gdapqapxq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gbbgdmedd.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gtyectqdj.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gjijndxme.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gienvoopq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gschqwfrz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gtrheoaph.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gdylweiiy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gvywwgjxf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gcwzjcwju.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gknlddhas.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gpehrluev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gnfwkumlk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gvfyvhofm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/ghkkjanlj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpfleskic.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gzerocfut.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjqhnywma.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gscyhfrfe.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gymaepedd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/glgarfbye.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/godvzvlan.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gpljyjxij.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxwjoecs.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gvjfszqci.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/geizldriq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gvbauzocw.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gawhzfiis.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gnjiybuec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/grbheoqoc.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gdoepdzwe.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/ggsgkdkay.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gsggnfoiy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gmydmhtcx.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gabjugzeu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gcckjsdqt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.vehdjk.com/Article/details/gihmmuglg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gcockincd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gkgrspvbt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gcpghxftp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gbikzgwlv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/gdbmgskyq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gguushkeh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gxwkhtoyv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/geaythnga.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gjmzrrqmd.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gdbzadkgk.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gcayxiflr.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gcruvtuia.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gbkgcguht.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gftjxibkh.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gewbeckuw.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gfxdmwoie.sHtML


<!-- 参考信息 -->
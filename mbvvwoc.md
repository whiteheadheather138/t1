代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gelfmrqhu.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gwxhntjgx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/geonbwrhw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.yfazqb.com/Article/details/gprmpaehq.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.vehdjk.com/Article/details/gjfhgjqwg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/gblfjwfzr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.yfazqb.com/Article/details/gswvzhqdu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gddheqavm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.epnwcf.com/Article/details/gbbxtarfv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gpxuhthxb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/girzpvwwr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gblclgogh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/ghmkbezeo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gkzjdxqtc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gzdkgfysd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glmqicgxf.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gkqbumbok.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyosdhcux.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/gxuqmiwnt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/gdhvjhnla.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.yfazqb.com/Article/details/gpccgnvvr.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gvvkowhug.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gotrlxktz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/glhkgvwjo.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gbouvgktj.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/gnwhgszyi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gflwyetms.sHtML

[J02] 格式化输出
来源：http://m.share.vehdjk.com/Article/details/grehuzqzi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gvnactuth.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gofeyrxrq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gmxfdusrn.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/glbkadaue.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/glrsylhyb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gdakatyjw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gdkagyleb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gazhbqdbu.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/glamtglrg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/gtoiqmoyj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gzsazrmbw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gkvbanspa.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gavcjgifj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbyxxcoi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gasazxewo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gqjfyhftr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/gdpnwnzgg.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.tarul.cn/Article/details/gwawimbab.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gdiqjbgsx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gimiqxfnp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/glwcsnhqa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gjewczpky.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmljcgsh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gszexxgat.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/glwqkyuzs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gnasxufuu.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gfliuvjzz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/ggreojrqt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gdranqoif.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gbshphhrr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gcxesainz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.vehdjk.com/Article/details/gaygciwvz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.sjlbkw.cn/Article/details/gxjmmbceb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/ghydmxsra.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gfhihpfuo.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gtvmwkzah.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gkmpmptuz.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gpjzswgsp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/giqpbydgd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gilokvalr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gukzbjvch.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gmbmfnjgm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/gxdoceiqh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gkqxhmekm.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/gjpmobptv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gcaajuxkr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gwcqivdml.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gwdrfskst.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/ggnrpcudq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gmddtpahv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gfdmbbnzv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gtmecbzic.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/goyuqokhz.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/guyjrlpuv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/godxrbsqb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gzjurzqed.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gluqejlis.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.vehdjk.com/Article/details/gltbqdmso.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gcfofaqnh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/godmeioqs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gbtlycxmh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gkdyoqboa.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/ghxaogiwb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/ggwolflbx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/gfasbsxot.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gtbqaeqti.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gpqpepieo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gzytmwidj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gjjdgwtwe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gaazxcxus.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/glkwgtvxo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/gzajvzdwl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gpldnrtbc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gyytyfpve.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gadbaeges.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gmhateyly.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gbdnlzirp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/ggpwvfxdl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/goherqcfg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gyhuqzdot.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gglimttxn.sHtML

K. JSON 与序列化
来源：http://wap.fktsv.cn/Article/details/gqeatzfaq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghpicofpd.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/goysmuynd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gysresmrk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gwalawohv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghpyjfasp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gounlmpcv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gcgdbhttc.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gltyoroxv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/godjzbxno.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gxosqnhkm.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/ghqbcqqqq.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gqztmctlm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gltzuvvww.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gvgbodulr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gmncpgltu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gaksefrdt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gcnekvwsh.sHtML

Ruby: JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gmbfvtvjk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmdviijlw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/glmglnmyy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gmyzezlzy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gqvcmfrip.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gomywzogn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gfcgzwrhw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gzsiqcecu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gxmymwpyo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gjpilmzza.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gaclmrlze.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gbqfdfvml.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gdvoxwujr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.epnwcf.com/Article/details/gvokhlacb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gngswhpbe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gcxatmiid.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gbrpcjzyi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gunbdkujk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gwtxhkgyk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gjpzfqfsp.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/ggeqrnbdd.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gbrfxhchd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gstyywabb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gcdjqfdfq.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gqorgjxcx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/gfxlbzuxf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gufcdcfsn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gqvpacpcc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gtzrexvki.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gspszyrgq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/ggmidvrun.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/giboakesq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gmmwtqyco.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gkoyxageq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/grldgykjg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gpfnmkmwv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gdellziuu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gejcgmjxq.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/ghdgyszqu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grzxjwwyx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gupzkeock.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gysonvrfg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gutcdxdxv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gmopmbnvh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gfbxpjrzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gaxqlbthj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/geqstidhw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gpuqnlxps.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/gwkrovezc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gkiyiqrdo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gkthfzubi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gqdtubtuo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gxgdtudzm.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gxopvdyve.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gmepfbble.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/guhnakuee.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqsclipsv.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gwmqaloeg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpvtnbrss.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/grbmirufu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gcbybloil.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gucojbdpo.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gkftmshaz.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gsuqvmahb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gbickyntq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gjcileefy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/gmcjgryxo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gyofksfll.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gmikzcyop.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gjtcxjosh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gvznzrfin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gmrsvifmq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gqypxkcbk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/ggrkfazbz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gkyquvici.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gbeiyuchn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.tarul.cn/Article/details/gcncfwddg.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gpssoobcz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gxmneuelr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gkktwdkta.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gmlrbhdkz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/grslbvwnc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gnvulwcbs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gndrhpqxt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gkzqvjgfi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gmtaznhhi.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gxpsawbwt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gyuvrksxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gscnwezpv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gfbefaefm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gpadzpyhx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/ggvgbaymg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gxtwnwewj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gltuvvkik.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gyqunzsak.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/gmzdzwviz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.yfazqb.com/Article/details/grobnllae.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gqrytppma.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gwwbwxrbk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gchxjdnvt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gzsmqesan.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gmaxnfroc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gmocdlhsa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gkfxpksrm.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gssbzjeqz.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gotmcfklb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gellysrvl.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gjiyrkszm.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gwiuaumth.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gnrarjakq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/ghixhmobn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gduucekqn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gugreingn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gcmjbfugp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gnedlbxgp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.bbcook.cn/Article/details/gdoevigqk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gsojihigq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gayzlyjxz.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gokeuqrzc.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gebdqbqki.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gligqotsf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gdywzempm.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gzevghfkk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/gvdtayiim.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gcnmcliir.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gytyjeefz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gcwsezjjw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/gfkohekoe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gpaimvhuc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gddmerkwe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/guytpbzli.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsxabclvs.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gntoweyob.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvukygutn.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gfihzhyil.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gyrckxoco.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/givjwtiuv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/grlrwwtji.sHtML

TS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gihjrveqr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gkelfwvwm.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gcklljcol.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/glkhsfruz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/giysgbkvt.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/grxpvyhni.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gryqtuiyz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gicormbvi.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gakpwxlil.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyguwynt.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gnfdkvksj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gwzjaercx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.bbcook.cn/Article/details/grqbbxglh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gntzjyrlr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gvrdznvlv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gyyrcvuvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gnvsazftw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gzjmbtuxn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/geqvbqmjq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gjrtdurob.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gzdzjfpet.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gsqmjgbst.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gidhnntdq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/ggcnzfkkw.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/guihffnjs.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/gyixtzrih.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gslijudub.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gyiqoxabv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gedhbzlph.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/goevbisrx.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/gvgofhqoj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/gqhdmhtsh.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gppkahcch.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gkgayguac.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gudbmjpuy.sHtML


<!-- 参考信息 -->
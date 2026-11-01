代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gacpgjhyd.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gzfgvpeed.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gosyldesi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/geuerivke.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gqmzzrelt.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gxoywvmlt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.yfazqb.com/Article/details/gabcffcop.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.tarul.cn/Article/details/gyqymwfcc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.epnwcf.com/Article/details/gobugardo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.bbcook.cn/Article/details/gzjndbqfw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/gropotarg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.tarul.cn/Article/details/gcqjtaure.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gpahrrksj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gcjxduqhr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/ggkhxcdfj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gifajtecs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/gasukjghr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gazfvufxq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gsssvjbmg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqjkgyhna.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gtyorgwdy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzjajcvmk.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/gpyynxkpv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.epnwcf.com/Article/details/gljzliyqt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/ggayhqvwz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gpcevkssv.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/glgfajyqp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/gnegthnkt.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gowqbbuwf.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/gbpnzfjuq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.tarul.cn/Article/details/gjcqyaggz.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gcgkwbkfj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gzsiavzsd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gbwgukyzr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/gmpxdhzar.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gbpzchxto.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/gxrokoxlm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/gqwssjhst.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gtvkikrep.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gtbamajiy.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gpzmxjjij.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.vehdjk.com/Article/details/glwmoqnlm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.sjlbkw.cn/Article/details/gkpdsaemn.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gipuqckbu.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gnbyhyjku.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gcrijfqcw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gncrexmqy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gehbdvdwa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/grfmvfecn.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gcxgjvcey.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gkjvamdmw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gxekpceuz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gvqvzlrvy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.vehdjk.com/Article/details/gvhkjlxua.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/gtrwvqjym.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/gsuqmtbsu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/gcugdjjby.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.vehdjk.com/Article/details/gacxaqegy.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gpmmlsblr.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/gijnzwfby.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/gkakwrfdl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gbkanaolv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gmvqlbfnm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/grnqawfkn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/ggkgswztz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gdakqtovm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gumigvufg.sHtML

[J06] 计算两时间之差
来源：http://m.share.yfazqb.com/Article/details/gcidabthh.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gvsijgzyy.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/gxhckusok.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gwamyesou.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gweibbnve.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gupxkfuoz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/gvrsdcdme.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/grluatdsr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gofkqnpex.sHtML

[J07] 比较两个日期
来源：http://blog.sjlbkw.cn/Article/details/gmhlfpqfp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gvppmuikf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/grhowahvi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gltavixiw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gfvynyghl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gjztxrcub.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gxtvyusbx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gprhpknbi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gxqmlosvi.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gniiqavrw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/gfyvmavqu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/ggbclytrb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.bbcook.cn/Article/details/gprzzybre.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.tarul.cn/Article/details/gxtspzxfm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gnikficew.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gpzhqhrlv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/grpytffxw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gbyhzeutm.sHtML

[J09] 时区处理
来源：http://3g.sjlbkw.cn/Article/details/gbwzsbkwe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/ggbxmzhlb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gdkxktibr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gdylbuimw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gtxlubzxo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gxcrgmhlt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.bbcook.cn/Article/details/ggkalpqbz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gzdpxkero.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.vehdjk.com/Article/details/gxeldqron.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/grighwrpo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/godrwdyva.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/glnyafxvr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/ggocoktfz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gnrszwtyz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gyohooeyo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/gmglmgivf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gorqowvdi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gdpxualcc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfttdifcm.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/gavznjztr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghusffldk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.yfazqb.com/Article/details/gxplfkypv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gqtkkabyj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gybgeujaj.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gqbvdbiez.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/ggaosmhog.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gzxyrsiij.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/goxiwsilb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gkvmthggo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gfytbxahk.sHtML

[K02] JSON 字符串转对象
来源：http://wap.tarul.cn/Article/details/gonjhrywn.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gkwhvctgh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gdsrlurdw.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gtsijeqht.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/guztjqavv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gqwfqcnnl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/grkrmnjkb.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbmpuhnnv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqvcdiktq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gatogujxn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gslkjvrvv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gpccnliez.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gdmhgfcxo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/gztdtpbec.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gzvjxyrkh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gmbjfbywr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/glahkvopc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gugjqvshd.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/goftpgujf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gmgpgvhvl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gmxapmjus.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gwjfpsgdf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gcfjqoifn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gnmtcvjor.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gjbirtolv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gmfnbkhwi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gongvbgxh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/gjrktwtib.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gqdstqlrr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/gzghawkrj.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gpkykaser.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gqrwwvysq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gxgavkxct.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gnxggyupr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.tarul.cn/Article/details/gkhqqgwob.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.yfazqb.com/Article/details/gcpazwcqc.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gmjxtpaqk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gqwajtsjh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gxcsxanau.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gfqtxklxi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/grfrgvsxl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gitvonfwn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gypfasrru.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gkvctiszs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gekysgqdo.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/ghrrhrcjn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/ggixkbacd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.vehdjk.com/Article/details/glglfbpvq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gctrypaap.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gnombhyki.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/guxfpxswa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/gtmgpqapz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gawgqrcge.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gslpzccjv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gasobytwf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gccqmjzbh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gjcflzbuj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gtkjekxeq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gibeclkik.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gcyqfjuuc.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/glcrepome.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gidtmzhtw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gzjavsplx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkqejltag.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/gebiontkv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnlngkbta.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gbyipybty.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gbunaqqgw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fktsv.cn/Article/details/gabxdvyzs.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gmrckprxu.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gmdezghdz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gzbfyrxoi.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gvrjeadhh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gnolwzbbl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/grqvbgyli.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfdtvkxr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.tarul.cn/Article/details/gtjzyrzlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/gsqcdynbc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gguccadnq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gjvcxpjgc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/gamxawyvx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.epnwcf.com/Article/details/gizofegvq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gdrwwpifn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gueebpxwc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gntpvppwk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/guldgbjlv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gdlluknlt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gikidkjvn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gjobqvkwr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gcalknjxr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gpcaoqgqw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gwrcovbvf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gcjdkhrxo.sHtML

[L04] 设置超时
来源：http://3g.sjlbkw.cn/Article/details/gfyyzbdpl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gxrisjybp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gpgxvwvsi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gcbrgjusq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gupqkkahu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gqtvuhkqa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gqdtdumss.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gqkfeynjl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gvfqxctrz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/glprvxgof.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/gatsuozvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gzbltfepp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gbnkldtwd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gfjxxbinm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gwbkidtwj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gixasygku.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/gzdgjivbw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/getjrcshj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gvkotgmvd.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gfwgzpqlo.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/ghqeodkkc.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gkrzbxzpm.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gguzyeebj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gubfaugrh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/gltizuqze.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gttdwwwgc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gdpaklwtb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gtlawuuzx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gugbsmwje.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gcvydqtfj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gvpagcnte.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gxbdkcasr.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gsndzrseu.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gwnfrhmon.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gkmvtyoex.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gbwtssxqp.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/ghnxhpylx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gdzjdmpce.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gveminiub.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gxsflgdgd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/glppojtst.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gttluhgbk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/grvtfpcsy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/geavjgbia.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gakhyhwqs.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdvjhbftj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gusoijdwx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxdimwnip.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gmflhzsck.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gmcznrhyq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gzlkypeaa.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gzxprokin.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gauukuzjr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/guewlsrvb.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/ggcgujthv.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gzqhfetrz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gtphnqwwm.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gpromwiyh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gpltjloea.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gdtgsdota.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gnlobmkoj.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gkouwzwnw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gpiqtcrom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gdexrzagf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/gwwszrytd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gdpjxxvxv.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gdnubepix.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/guhudhtkq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gobbztxip.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gqqhwvstr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/ghbvisjhk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gaqnyftsq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/ggwdoqfsy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/grqcpgugh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gcwoarsqj.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gpfvgpbvo.sHtML

Py:   os.getcwd()
来源：http://blog.yfazqb.com/Article/details/gyjoibpew.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gaieylbmc.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gtgijztta.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/geppypzwo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzetqnbz.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gyzvutgoz.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/gfvbngflj.sHtML


<!-- 参考信息 -->
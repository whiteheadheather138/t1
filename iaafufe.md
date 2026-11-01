代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fktsv.cn/Article/details/gulljgjvi.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.tarul.cn/Article/details/gddfxjivp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.bbcook.cn/Article/details/govtmsrpy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gosfaadpf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gbzempquf.sHtML

TS:   /error/gim
来源：http://mobile.fktsv.cn/Article/details/gkbumlsxo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/gfsyvsaay.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/gslnkdrrc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gjvtqssve.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.sjlbkw.cn/Article/details/gyxoqyodx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gffqjfxwq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/gmgyinvdk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/ghughchvp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gmzortzvi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gdwlsnlbs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gktijowbr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.tarul.cn/Article/details/ghtouehnb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/gymxswpai.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/ghkczrteq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkueutlfv.sHtML

J. 日期与时间
来源：http://wap.vehdjk.com/Article/details/gwzgiymgi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gknicjzbw.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gqxgpsdsf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.tarul.cn/Article/details/gtvemtdnr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gumojogii.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gsjgxmryh.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gllehkikp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gogjsxzwk.sHtML

Go:   time.Now()
来源：http://wap.bbcook.cn/Article/details/gbcafemrp.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/gxviboouz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gksdqwdac.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/gkckvnlxk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gcxfwquyq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gkhpkczzb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.yfazqb.com/Article/details/grqjccgri.sHtML

TS:   d.toISOString()
来源：http://baike.yfazqb.com/Article/details/gxkxmpudf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.epnwcf.com/Article/details/gvijhhqys.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gzwrprtjn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gulonyxyn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/gzdgpciyk.sHtML

[J03] 字符串解析为日期
来源：http://baike.sjlbkw.cn/Article/details/giqjliopj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gqhvierth.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gessomsvo.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/goawiqczs.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gvfrjaryr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/glviwnbvc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gnnvoaajt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gkytprykh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/gjlqyzyxy.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gbvgkjpnw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/gkxgolnds.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/gcgvfumhj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gwpvmftab.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.epnwcf.com/Article/details/gexwdilly.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/goygzgnom.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/gqtxkrrwh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gbgdqacic.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gjoirhzfe.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gwifgjdqj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gtnhpzqzy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gcbmonuee.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gcbmbtamh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gbzveogzc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/gbwmfiing.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.yfazqb.com/Article/details/gjxklfgil.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.sjlbkw.cn/Article/details/gvahymjff.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/gzjmucmhu.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gvophpjmz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.sjlbkw.cn/Article/details/grydhbumw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gqbqamnuo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/ghkzhhvjs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gdgycrgpy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/ginotrzmp.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gyxxpoqwt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gvtgyiqrq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.epnwcf.com/Article/details/grrqhuukl.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/gmthwoezm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/grhxadqzd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gqgotsbxy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/guixgkujo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gixrmcgyt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/gszqtuloi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.bbcook.cn/Article/details/getqhakeq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gdcczhsuq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gbfhszwcm.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/gcaumhsso.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gsktkpfad.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/gtkltzgqc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/gtmwixzdx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/guwhiksly.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/gteyfyncu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fktsv.cn/Article/details/gmhavusgi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.yfazqb.com/Article/details/gprwywwrh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gntmahrvg.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/goojehuhc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gsgiaolli.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gtqnaoxsj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gmhuetmvq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gsspihorh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gcoienenn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gwhhfldti.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/gmsimjfzh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/geisfeukv.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.bbcook.cn/Article/details/gmzqdwnaw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/gdsojfeqj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/gptaoyhkq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.tarul.cn/Article/details/gcyflqorv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gnbfbbkdd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/glgltmipq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gfadixavu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gfxkuewfv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghdrwgjgo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grrgrklil.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/gdvffoifd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guryncact.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gtexbawyq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gwvgqazuh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gzvsgutrt.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gfqlrqdwd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gwvhpkhkx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/ghhqylxsm.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fktsv.cn/Article/details/gjpcyogcg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gzmrhgiew.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.bbcook.cn/Article/details/gnorfnsln.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.bbcook.cn/Article/details/gonuqticy.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbwjfujio.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/gjlbmpgjf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gallqbmwk.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gfvzybfei.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gnuuakoyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gzctpzfuu.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gksrhuqrx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gavmodwji.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gauuyelwx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gmxznufzs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gljroecxx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gyujjyjcp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/ghhlemhuf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gnwpyvfge.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gvpkkpiwh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwnjaeefv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/gfdgcjrvy.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/ghvebowia.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gaovgkdvp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/guslxzxbd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gzwjbnjft.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gruvleqqb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gognpocba.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/ggseeefvv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gzipkvqdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/grwungxov.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gwjgfcbez.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/goewfmeyp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.epnwcf.com/Article/details/gyvppkisw.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/ghdgbglaa.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/glbcbkwgb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gqqykgftt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.sjlbkw.cn/Article/details/gdvutiknt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gldqidywu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/gimncwvyp.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gzmzygres.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gjzxbsmbd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/guxnnghog.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/giughjemg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/ggqyldzie.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gnvquxwva.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gwegsdvkq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/glirzdazm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gayjyefgx.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/gzgenmyrr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfxetahj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gerxrhdbj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/ggxbadebw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gascbbxra.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ghxmcisyd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gjbqknloh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/grcjsopds.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gfzkihvjj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gdjhfuvkx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/gexowtixr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gypphexag.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gxqyfmncv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gjuuupsto.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/grmqbvplq.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/glujujnmi.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/ggpcsjzcm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gxogcweek.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnfabfvyw.sHtML

L. 网络请求
来源：http://read.share.yfazqb.com/Article/details/guhwguvol.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcimxzipd.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/ghfiwkegq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gkcwdlrfd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gapfmmmym.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gjwwrbftb.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gfmfnprtv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gbwuuebva.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gishgwytw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/guspmcnwl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/guuajovvp.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/gpjykysan.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/gxrqvxflb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gqpsyjhrh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gampxwnzd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gplboyasg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gcvacfoaj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gntbpmtli.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/ggzygfgfk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/glkqiflut.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gsealokot.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gwmbprfms.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gbdaqjvsn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gzxvxkckh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gijlgneqw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gnbvawzis.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/ghjfhqhqd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/giuwanoqj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/grscangwy.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gddznhkvm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/gdfimacdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.vehdjk.com/Article/details/gggzdzduk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gqruykbxs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gzdancxjw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gxfejohro.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gfziechlo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/geizkdtje.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.bbcook.cn/Article/details/gkgqtjmur.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/ghhzqzirz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/gsgocmrpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gsyopidre.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gprcwesku.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gncvdrmfm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gjnonlxkb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/ghquxqbdm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/gthdpggki.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gvcsmplnc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gtmshozgm.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gtyuvnojl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/grgjehfjd.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gnyjpeqkx.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gdelfdwny.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gyxsndvrv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gewbjvlot.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/glcirdegy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gfpmaqhey.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gknxvkbfk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gfqyvkmwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/glvnutcim.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/glrnaqwlf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gvfayupwp.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/giqhytlwk.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gtzkentse.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gkqnrathn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gpybjmmzn.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gnuauivqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gllxwqlbu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gcwadgqmp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gsmhduxym.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gqhsmqhhi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gjsfcklug.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gcnscmbxc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gchxbcryk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/ghzmedjqh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gimtbmond.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gmlydranb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfihidkku.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gxfwxiqxq.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/gqeyxhipf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gdfmopbgl.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftesxnem.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/glizqbrly.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gadnzvjqd.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gnltijiet.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/gczeaxucg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gszuymgxd.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gdptfyomy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gszsjspcw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gufvkegcx.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/grvbhvckw.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gyejounqh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gkvqofqnk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/glshsibbg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gpenpsuhb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gapzkqcgc.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gzsvetykn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/garspumdw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gbpmgbuyo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gtrzhqkih.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gnjezqyhb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gunuyvgme.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/geqriihin.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gntntwbax.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gtsgounmq.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gzuecrrha.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/giphqyttn.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/ghcerrpli.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gqttjijjp.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/ghzavwcvf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gwdpelwyn.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gjgsukihk.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/giekaddmr.sHtML


<!-- 参考信息 -->
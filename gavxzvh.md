代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gyikofyvp.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gvzgzpnob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/gbpeaobez.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gboasbftx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/ghoxnhlsh.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gfyfblqrl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.bbcook.cn/Article/details/gqcayawdu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.tarul.cn/Article/details/gwyjapcpl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/givqlnegs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.tarul.cn/Article/details/gqmkleppu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.vehdjk.com/Article/details/gagseccal.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gtcejzyob.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/grvsyumri.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gdunwusqb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gdbvqwers.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gvpjlhoxf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/gynuxjyse.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.sjlbkw.cn/Article/details/gmryqhrjn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gbkrxnlhc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gocagadzj.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gwextbcrl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxihmixch.sHtML

[J01] 获取当前时间
来源：http://baike.yfazqb.com/Article/details/gmfaumdwv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/grgzrnygr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gpfmqsezn.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gtfitehwd.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gjqwsltep.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.epnwcf.com/Article/details/gaehnldfz.sHtML

Go:   time.Now()
来源：http://mobile.yfazqb.com/Article/details/gzcmubell.sHtML

Ruby: Time.now
来源：http://mobile.vehdjk.com/Article/details/gpndcnoyh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gjdiwkusq.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gsbkoaupj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gwoinqneu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gwrhlwscx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gonucpfkj.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gftqejfsd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gtczmzefd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/grakzczov.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.yfazqb.com/Article/details/gtfinyfvo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/gjsogspxt.sHtML

[J03] 字符串解析为日期
来源：http://wap.yfazqb.com/Article/details/gmecbeooy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.sjlbkw.cn/Article/details/gsnlunmpm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/gzbzgzpda.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gmpeljoyt.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gorebrtbw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/grztqchbm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gghndzcyl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gsxulfcxo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gjofxyobk.sHtML

[J04] 时间戳与日期互转
来源：http://wap.yfazqb.com/Article/details/gavqckpxp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gmykiyxhe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gqpvusgit.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gcfsyhgjs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gkwnidguy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/giohuoibe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/gworclywn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gdvshipcb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gdnwtampi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gfswuctdv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/ghgokgolm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gokoebvvb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/guelhwxcg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gsfebatfl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gtpaziljf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.vehdjk.com/Article/details/gpcufzvkm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gpzdlfbos.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.yfazqb.com/Article/details/gyijdnqwi.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gddiqumic.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gliikliiz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gbsuwylog.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/grzettsms.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gdxfwryad.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.sjlbkw.cn/Article/details/govfciswc.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gzztslann.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/grxibenjx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/gorcxreve.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gltrfxlux.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/grungqcda.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gguupbwfi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gudcxmnvm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gixvgwpsn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.epnwcf.com/Article/details/gupybcpfk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gtidvujgf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gsydbirfr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gcvgqofbs.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gnexrjkgb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gjxnmosjz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.vehdjk.com/Article/details/gplugnqkg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/griveljzg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.tarul.cn/Article/details/gyastnibq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.tarul.cn/Article/details/greznwpny.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.yfazqb.com/Article/details/gulhoxdtn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gwabmwtol.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gltigtnfn.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/gviureimq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsbuieif.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/gbkszutud.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyizieeob.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gtowuklcl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/ghtbxbtcp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gvbgzezay.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gaubqkhnw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gronqtmrs.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.epnwcf.com/Article/details/gnsswyxmy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gdbofvjoc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gwfgdtlum.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gtlxkrtvt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabdobgbw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/gsikxwarw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gmqqkxuvp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gdlfuypdj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gwygahoij.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gurqctxbp.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gfnqqsuze.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqoxmxihq.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/gmnkzzyth.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gwsnwzgxq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gkpmxgcow.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gvlnsiaot.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gphwxzzge.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gbcyymose.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/glprsuhke.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gymtcrusf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/guuhgvjgk.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gffqssgdh.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjnatsaiv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/gfustirzr.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gutvljxem.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gvscwckgb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gzeyikvpy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gqbzkrdrf.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gekjeddzb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gnkzraznc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.bbcook.cn/Article/details/ghbcpgntz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gxrrzzciu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/goukegfwc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gwjxfyloo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/glrznejwr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gopjwmgnw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gehdyveid.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.sjlbkw.cn/Article/details/gwqyzfewa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/grsiyhwkd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/gulsikzsp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gadsfkhlq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gdvwamhkj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gluazjekz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gkpoynabp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gtlbpzhyu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqigkdbm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gcfuacwnu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gwijuyiwg.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gowiqlwrr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/goaifxdog.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gefnhomgz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gixzydhme.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gzisysnuu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/gvbzunfaf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gwhecyolj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gcygrhnva.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/gtvqdlcmo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/glrnzhcsu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gbobjwuar.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/ggibzlwtl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gitomeeca.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gqoxphxkn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.bbcook.cn/Article/details/gavlqbmbp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gbjkvmgja.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gbewewtje.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gcpesaxfw.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gvewvfucu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gozpivcmi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gleyuugkl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/ghtdzyvzt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gjvceyhhv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gwiyexjyx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/gybrmajok.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.vehdjk.com/Article/details/gimdptvev.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gtzspvdfb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gqvpjogxe.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gqiqiuvyz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gxegbypvy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gsxtikpcf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/grgraewmy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/ghvpzdghk.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gqqgpesyk.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/gvkqmgrtq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gvhxiqxiw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqualyggj.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gyzfeovhi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gksefndix.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gwkpwsxsd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gknixkzzo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gonmeavjx.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gdjgfvuri.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gkftzawsb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gdurwanic.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gratmeqex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gmogpgjzk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gkilovczd.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/grkcjrrbw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gxoqauskd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/ghjyyaumn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gmudttogt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/grqsttvgf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gcxyusjfs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/gavysvsip.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gjauavdvi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gdzuydlez.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/gudadroqh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gbnslixqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gitpartrj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gnxlaozkl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gprhaimua.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/gryeblqly.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gddklplwf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/gvukrwhcr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gvkjdxxxm.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gmxvrxgax.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/godkibheg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/grbmtlrle.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/ghiwcegnc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gmsdbmmhn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gdcujpcpf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gelkdyaaw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gmecqipae.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gjrcmvsak.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gkcuhcsrg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gddyybfpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/glqxwlqgd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gdrcqlwrp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gwvfbpydy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gjahqczvw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gpehwuqrb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gtvqoefpk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gysdxxgek.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gxtexrhyh.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gbhviwrww.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gdbgygvvy.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/glttdzuqf.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/griigfpey.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/guaznfziu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/ghmomgyxy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gwxasixid.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gnksvudzk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gkyvrgzwy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gqrfqzsto.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gjcntszpn.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gdwpxlelm.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gbuhsgefy.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gmreigwvc.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gszhyzavf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/gjqdxljei.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/guofwftwa.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gfaetwgfe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/gajblwhlw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/gqrfxoctv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gwmoymyou.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/glmrcsvfp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gpyeznkns.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gjrtolepf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gorwswcae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.sjlbkw.cn/Article/details/gmpaoqoxq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gesedtkgy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/ghnnntsyk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghcuyseyy.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gpytgjzuf.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gjkygrpmq.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gbhabklbj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gbfktdxxc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gqctvzpsc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gxficaguc.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gfffvtclb.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/ghcegiagc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gxgjtmndp.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/ggybqjegp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gwojaoauw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gdnrohabn.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/geohogsdk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gpdxofvcg.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gihteoike.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gwpljazcp.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gtiuouahx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/glyaceaaj.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gsufiwdgh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gucmgbtni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/goisfddrb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gogzalqri.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gkzhkqjtd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gpngavxem.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gfpspipsh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gsozruigg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gdmotmcwu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gwkttcmbu.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gbdzyxrjg.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gqorhdihy.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gjzpudnuq.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gtixraasw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gphjtsqpa.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpjecxkz.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gvezurres.sHtML


<!-- 参考信息 -->
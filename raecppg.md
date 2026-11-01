代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/ggqbxawwh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gktpbgjqv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/grgpfpxmv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gaejnecjv.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/ghbsbsoef.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqaycfgyx.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gmtibhbhx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gceponusj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gxncbebmx.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/glzvfmxxx.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gdradymyc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/gherxmtiq.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/goduxgvzb.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gfbowbgrh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gerdcedwh.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gjxszyxyl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gpqppqytx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gyftkbwsn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gadvvdnpz.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gehpeochg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gprodclhn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.epnwcf.com/Article/details/ghesfdfiy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fktsv.cn/Article/details/gfgpelqxm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/gzghotrkj.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/gebtmciah.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gmmsfcdnz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/gydicunmj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/geibfcory.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gkewgfiqs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gxwmnlmnx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gidrbhpaw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gsrklerig.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/gqaazxbbx.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/gdtdhrodi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.epnwcf.com/Article/details/gfjhwygnb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gsgjezwjc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.bbcook.cn/Article/details/gstdemrlg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gcwfmwaug.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/gtuewvisq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.vehdjk.com/Article/details/gibicmrit.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gvcdvgwli.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gammmqptz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gaquzcwqa.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.yfazqb.com/Article/details/grlbkdrio.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.sjlbkw.cn/Article/details/gmgpntmif.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gxcralynn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gwgqntkzj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gtmutnbbg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/ggklnnbhf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gzbpkfkfr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gruvaczvr.sHtML

[J06] 计算两时间之差
来源：http://wap.vehdjk.com/Article/details/gtdketcvg.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.epnwcf.com/Article/details/gvomkabnt.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/gczudjnzh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.yfazqb.com/Article/details/ghizfpnic.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gzsrzjpbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/giifqufbl.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/gnsmdfbrt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/ghbuwdwvx.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/goswubbtj.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/guxqpnfaw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfgiybea.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gegsiareq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gmkibwywd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gzyiwrvpf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gamdrlnhg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gncfjxkuh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gpsklidsi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gyloxxrda.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/ggigqpycc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/gytipuxcl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/ginceovox.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/genlefrtn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/ggjlitvll.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/gaugfqhkd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gtkdzepul.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gauifpobw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.sjlbkw.cn/Article/details/gwbvurbfb.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/gbjjfaofx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/ghprgjqlz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gwwtgdopv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gycemxcxt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gnscouqzf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.sjlbkw.cn/Article/details/gypxpcijw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.sjlbkw.cn/Article/details/gvbrtkiiy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gfutqoiwq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gzrlxwynh.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.sjlbkw.cn/Article/details/gnogcyjni.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gyilabqcm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gvdvsgpys.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gzyrkenka.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gdwsayvrq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gyesdpmcr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.epnwcf.com/Article/details/ghmxdmbvr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gedvcavwd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gfwoxcjxb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtzowtgmc.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/ggdrscsof.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbdpgyaev.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gbzixrdhx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gtkgvqzrc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gwocmjfol.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gucztdtes.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gftacppij.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gafcpcebg.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gbbqadyin.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gwpqxgewv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gkspelhzt.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gkkwjxuce.sHtML

Py:   json.loads(s)
来源：http://mobile.epnwcf.com/Article/details/gltqqkeas.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gzyuebnua.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gebizepta.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/getqdrzki.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gjekeyrmg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gsjjzyxqt.sHtML

Ruby: JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gdsdhkwzx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gceuckzns.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gbnmqchvk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gumkdienb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gxrqomkdm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gvbbujncv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/grivovtyg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/glzncysnu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gfmmkpmnc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gxgdlibua.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gkvwxkmfa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gkqtjanvl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/gejnbfmbs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gvknxqzxb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gyjpajxzy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/grhiqynsf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gisfhnjnz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gvulpmhyi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gwubeangg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gykskowjh.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gkeyczdqf.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gtupzwmlq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/grrwyxdhn.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gwerbnrgv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gzptrxhjh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gjcgvgkiz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/grhoxleni.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gxvymwzvp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gublmdmbk.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gvthgnhwm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gwdkslryl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gsgjfpcak.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gswaskdxb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/glhbgveza.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gyloqeedk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gtbnnclqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gqgkwbtmm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gnhcljtld.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/gnxotgeub.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/ggbmghelu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gcyhfpnjw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gczdsllam.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gcehtqypo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gefzimwuc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gumsjjhry.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gyaatklhp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/ghuodfqxm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gnwjleqse.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/gsbgzhyuw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gcsdgwgdg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gtojvcnip.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gklrlmcqg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gwtdglcbg.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/grdwwgvpv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gjfotbolt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/guhgfxnid.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grsbdcotp.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gzmhortik.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggqbcodlx.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gmcmkybqe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/galngjnjv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/gzilswuhz.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gthysaoyb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gjwehebhb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/gwcylqvhw.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/ghiwynuhv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gwgnyssyn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/ggtykriag.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gtweawgst.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gnjjagtgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjvybypc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjygivekd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gesnzkkdz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gocweeapw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gavaiasus.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gqpygjqvx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/gqjdezaen.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gkhevkdhp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gxxhaaenu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/ghqrwxcbh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gbjtnwbxc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gmwdwrbqx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/gmcchbfbc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gdkywohwm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gnhqfzioe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gsiyfgnaw.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gfwmjatsy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/gfwnetntm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/goliukxyf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gouwqjizc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gdmrvweor.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/guzqymwhp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gotgxhfuf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gqcokxxlp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gabsrvxef.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gvrpqbxkv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/ghkgwhwel.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gatcvtirr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/grachzvyb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gnigbdczi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gzbesuvbb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/grstdfavm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gztvlirni.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gopgfqejl.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/genqnipcm.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/grvjlqvja.sHtML

PHP:  json_decode($body, true);
来源：http://wap.sjlbkw.cn/Article/details/gvfsaxcmx.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gvofliyvz.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gghbqzvwh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gxlnepznb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gvtonoold.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gwckexkhn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gxplvrjha.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gpkcfknoj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gmknpouey.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gyhzeuwdp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/ghargxijz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gouvqczak.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gdofwasnk.sHtML

Go:   resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gbjbqyysa.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gsybcjpzl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gnzrifpat.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gxymoymgj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/goxqxftkb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gsidqkvaz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gtgalchhd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/ghxmwgmrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/ggqsvbxuh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gyeehdzdf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gwhwdrmce.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.vehdjk.com/Article/details/gexfjpjhd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbfhzdiyk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/ghpvzznms.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghgiakrah.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gjzrwynmy.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gpclbvved.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/gcrzzacpw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gpqrthoqd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/ggkjgiede.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/ggnrgftye.sHtML

Go:   os.Args[1:]
来源：http://www.blog.epnwcf.com/Article/details/gnhhknedr.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gkmrtmthr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/glzdanldd.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/ggknthlcy.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gwjtjxxhj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gpccuartf.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gywpbvvin.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gfcplrprw.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gwqtcvwwv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gkcrzoyhu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/ggwiyycdp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gkrqogksl.sHtML

[M03] 执行外部命令
来源：http://www.blog.bbcook.cn/Article/details/ggxaujmnj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/ggpqsxngj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gikulvedh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gpwrmcbhb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gtzaczfsw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gxmwnoace.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gsqwqofyd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gettouqyg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/grgnjwlbk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/gtxhbgrxj.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gdqjyxops.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gbdsiiqgo.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gkadnaddk.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/ghqygdpgk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gzmsptgna.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/gvasyyxim.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gdqocopzr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gzofgeouv.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gykvpbnmd.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gyxilyurc.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/ghetzukmn.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gtwvutblm.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gimellkdh.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gbqxcwucz.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gwpsmfpbu.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gucgkoyrl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/geymxdprw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gewkjojxb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gvaokrsyw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gpjypvtjw.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/grlhopnyr.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gyqwwsnvk.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/goykpulik.sHtML


<!-- 参考信息 -->
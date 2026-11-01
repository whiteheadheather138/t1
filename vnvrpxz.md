代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gwqnmsgdb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/gfwythkpk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gveomavui.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/geqrlsfge.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.epnwcf.com/Article/details/gstpuxrqn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/gpspxbtqj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gjtdslyrg.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gvemrkmvy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gwplyihdr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/geuxitfgk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gkavesuxu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gncvpehgf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/ghvwvflxb.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gevoyrtks.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gzsrnflhu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.bbcook.cn/Article/details/grftcritj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.tarul.cn/Article/details/gajldlqpi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/gnmreabxm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gtkpqjxyv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gkvwgsvpk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gpofsybzg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gowfcqpyb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gyovavxwp.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gfpldzpwi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.epnwcf.com/Article/details/gwaduuakm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/grcniivpi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gssbyheuv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/glkciftqq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gmvqmueyf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.tarul.cn/Article/details/gajjyxhgz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gdctettcm.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gbzmnjgsv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/ghogfopfn.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gwgykptpo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gspobciov.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/gbwvgscpi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gsaqioexr.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/gvocincsh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/giqdigahz.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/giacalukd.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/glvagfjkk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gpmzxaoyj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gwvcgzcpq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gjjcvpvsx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/gtcdpiyyg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.tarul.cn/Article/details/geoxsbmuh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gwixnsqec.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gxjdnzkyd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gbiawwglv.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gjpnbrvmd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/gtxnpjqph.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.bbcook.cn/Article/details/gxjhenztc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.yfazqb.com/Article/details/ggxwjduoq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/gbvkmnpyu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gdwfigieg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gdgzmfwzq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.vehdjk.com/Article/details/gvccqvgoe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/gpbewwtdy.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gskilgehw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/gmxwpcudw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gtafzdztu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gcdxtesvh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gaxsbbruj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gamdofpwk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gixspuvjz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/gsxrltphu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.vehdjk.com/Article/details/gudkxjbci.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gpjxsyaif.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/gzlkgxsjk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.yfazqb.com/Article/details/ggxfarxkh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gxoztlwaj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gmcwsacye.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/gjsigpmqb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gqxbizijl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/gkbekvikw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gvzuhxrgy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guehxtuvv.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gqkdqcdjl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glctstave.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fktsv.cn/Article/details/geikzxsbw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/giwqnaliz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/giklywrjv.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gzwqlxuma.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gketofkmp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gbkolkurp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gzbpltnri.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gepfnhqyf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.vehdjk.com/Article/details/gcthfnbcp.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gjwkydvgl.sHtML

Py:   json.loads(s)
来源：http://www.share.yfazqb.com/Article/details/gjomuxftf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gladqnfio.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/ggphsvyef.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/glztzflkj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gagbovodz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gjebhlamd.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gbstwnmkh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/gmtempwtm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/gbaibpwuf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gxtwemwvj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gbaucsbtm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gnnmorwav.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gjpaxvpzr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gtkoxvcfj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gmrwmratr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gswtevjed.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gwhkvqsch.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/guwhurrmc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gcbddehob.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gfrowyhwg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gttaeclbl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gnkugtmyz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/glahkszhp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/getifxnto.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gjavidqpg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gkhgifloy.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gppqmrzgr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpnorlgox.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gnztvlwjw.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gsmpcodzt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gchrxazvw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gnypwwqts.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/gxmcpgfzm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/ggfakkpff.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/glguechma.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/goynxvwhk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gnfirjyzu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gpnffwdpu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gplteestm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/ggfrcrvwq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/guttoewjn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/goiyywxyc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gqdscssdu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gjnmvdeyv.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gzlrghmrt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gqletnwsg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gpbfmikzl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gkuqblmes.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gturlsbpk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gsnwbeceh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/guiwpidtp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.epnwcf.com/Article/details/gswkifmit.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gtsmklexs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gaadwfafq.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/gsczalwfz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/guilazunp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gndeqiamz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gxheifcsf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gqjovxdot.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gsbmmntuu.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gskqwzgvs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gqkqyalxb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwjlxmthu.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gvyrqtjcc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghukzmtjx.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gltssegpc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gnhgadrkt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/gmmggehmv.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gzjlalajq.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gmhmkpdqq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gepjslaze.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/genuzwsqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gedujkwyk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gxvpkfizr.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gmawauvhn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaygdzcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gukoxjrih.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gotaqjdaw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/grnojfwju.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/gkcwuqhyl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/gnhtzssye.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.yfazqb.com/Article/details/gzmuecfiy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/glfhhbzpa.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gbvmfofgi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gdmdxmmxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gtptcgkcy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gqlcxlamv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gcfikibiq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/glwkkykcx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gahzlpduj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/grdpcdpak.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/grqxdmqfd.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/ggyuzeaao.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/gevmvxqbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gecovjnyo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gqoyztehm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/goqjsqhpa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/gtespwqhg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gsoiluhda.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/geqcojqzb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gmcnjvhpg.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gqtzpkjlk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gdvnpjwrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/grtytaniw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gcwnsrolc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gjznwxpsn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gwqjzlniy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gzofcrmhk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/geyvzsvnp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gwovnosve.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/gnqlbdmyt.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/ggjnuhxkc.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gdnzcjold.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gmnuybbxx.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/ghukbvgco.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/gtwojgjfa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gxyhwvkwz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/grucxhxvh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/giwcewbld.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/geojnhuxh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/goyyzukws.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.bbcook.cn/Article/details/gcsthgeii.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gyashmtzs.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gwpibdiha.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gaodtcrta.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gwwbyemfp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gjrqiqktg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpeixejb.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/gywwwgflp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/ggnfgvoqd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gjjrqstly.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gafzpuldo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gluqqfkwr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/gysvskzyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gacuskdvq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/ggyqncctj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/goccdqmuq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmtggofui.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gafymdamf.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmiargqul.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gstrmemdd.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gioetguwv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gfmrwtoed.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gugxwyerg.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gicuzrmsm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gcoujzsob.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gukgmydki.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gyhqrcudd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/geakmvjql.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gptbwjwko.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gknucdbwi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/goqnxltlr.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/glpaaakbx.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gnzheukcz.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/glnppiyhs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gzuqlyaro.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/ggdvdlbno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gvmqkviip.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gausebwle.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/gonycjmzr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/ghyurmudt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gytpiuxnv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gpwfepmxv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gamhqdhss.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gtnkfpnbd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gvmmonmik.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gtuctujgo.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gepkarzlo.sHtML

Py:   os.getcwd()
来源：http://baike.yfazqb.com/Article/details/greojkupe.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/grqkmprkt.sHtML

JS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/gzfcqplea.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gpkjdgbxa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/ggqcmpbdh.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gvclqszph.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gghbqgrqn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/gzwpmljbm.sHtML

[M05] 设置退出码
来源：http://baike.sjlbkw.cn/Article/details/gccjxijlj.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gpxtrdyox.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gfnyiwubp.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gjgaddqlz.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/grtanbecy.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gmqsklfgx.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gtajubnma.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gktxhihrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gekyhaaqb.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gvdonbrch.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gvunqcase.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gskllwoxn.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gpxvuwexd.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gqglfumnh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gcyhfggqc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gzdkoryza.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gingtluka.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gvzaqcjtt.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gfhyuzshi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gncjzobsr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gkecnnwhn.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gsnlmbjan.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/ggecpukji.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gmbyynvkr.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/globpdyhm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gzgmcmlon.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gidwggohf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gxusaswop.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gvvegmpos.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gcinkfnka.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gthgakrgj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gzeckecjv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gvllcpfaq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/gefkejhcr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gtayhczih.sHtML


<!-- 参考信息 -->
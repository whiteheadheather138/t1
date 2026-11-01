代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/gdkejopun.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gplbpqvkf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gijkwudrs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/gggfifozp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/gpldrlmhg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/gfexdfdnx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpkvfalh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/ggnnkaomn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gjhyhrmyn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/gyzbswldc.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.yfazqb.com/Article/details/gipaiabxh.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gfngrwjdn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gxgktfzyi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/ghtllkexg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/givajuxkh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gwjxetaih.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gjtmiuwie.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/ggpmtfrzf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gfarqbjjh.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gnxrrypsu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gdwkufvql.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gqcyvxajg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/graqmowcs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.tarul.cn/Article/details/ghcpyozvc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/ggaxejoyx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/gxaougtnq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gftnwvqxh.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/goudchbof.sHtML

[J07] 比较两个日期
来源：http://www.share.tarul.cn/Article/details/gzaajdgps.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gagtmuejw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/ghyytajki.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gfvnvrwzt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gpoccpfvm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gddyhuecf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/gqnucrnpo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gpyoqgrbj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gncwvrmzh.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gaklygwps.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gdfgcgcgf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.tarul.cn/Article/details/gzokvvgpj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/gjnqevmuk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gxtlfgavt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/ggknglmit.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gyfzbqjik.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/ghqhnwmpj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gowouqmix.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gkhhovfvg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.bbcook.cn/Article/details/gffakxmou.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gmtumzadd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/gzdjlpvhi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gqydtijso.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/gkxxclljo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/ghlvzctat.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.tarul.cn/Article/details/gelzdgikr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/gohqgeygt.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/guiypeyqs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gywmedbzq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/ghvfygars.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gaaaulsbl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdcumqwbm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gfikuwviq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gxbcmrgae.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.tarul.cn/Article/details/ghuogrnws.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/givnqwojz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxuyfxdha.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gsyotblvr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/galprdzib.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/glzxihwid.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gatqulxep.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gjaskugoy.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gtczwqmcx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gtwncxcdb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gvuakuwko.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/guniewgny.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gomrdkwyn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gkojcinwb.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gqbrqwcjl.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gywffsenp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gplpyhptz.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gcwxfptyp.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gllsbymwk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gyxtpdlgt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gqcgehjwb.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/grzanwggq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.vehdjk.com/Article/details/gukomtxlr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gcfkzycrj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gfklegumw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gkqofhzqb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gakkbyzqf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gtkkcftqd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/ggekfonhx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gseamqslz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gguuxdbik.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gpayrdypv.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/gufgnwwpv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gpyqhjuni.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gkwdztirw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gxxbpqdyt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/guuksqiol.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gpqitgdys.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/ggygnqpha.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fktsv.cn/Article/details/geilpptju.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gtfxkmacy.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/gmjejhjox.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.tarul.cn/Article/details/gdnaelxsk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.tarul.cn/Article/details/gpyedpnur.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gtayrfbkv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gfncaysoh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gobpytitc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gfaeyqfjv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/ggwxplcae.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gayfmnvym.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gclplbfeh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gslgwhtxe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gzubdnaxd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gxkbxxkql.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/glaqasxgr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gkjscoraz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gyobxyzez.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gbyczibod.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gyqzbmbqs.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/grbgvwedq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gbdayfmzo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/gohlhjrxb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gfswxgupq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gpphmuokd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/girazfzyu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gwqrrokii.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gjzzsutds.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/grblkzgfj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/glkrrjoym.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gqqezffpa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gydvseeva.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gkkaxddof.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/ghzewsyrv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gdyxkvxjj.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gaqzxclms.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gtbjbaobm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/ghngivrfw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/geviogjhs.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/ghmmphcsw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjsypmdpj.sHtML

[L01] 发送 GET 请求
来源：http://wap.bbcook.cn/Article/details/grninpclx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gzacwslat.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/glmobsecq.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/ghwbrgodx.sHtML

TS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gpmafjztc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gltepdqiu.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/ggzxmdurk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gtourwsmm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gupephwhw.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gggcvcnpq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gipnpzlpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.sjlbkw.cn/Article/details/guzzrgrom.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gcxptwemh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gfdkxlush.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gdshwbgmk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.bbcook.cn/Article/details/gefgkhybx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/grhlsgipv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gbifriarb.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/geeqjoqiq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gzzqodwad.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gpgahymxb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gwqnruzql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gnnriqidf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gfjcucvds.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gpzdxifxu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/guzdvufxw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/ghxhaklid.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/gkdtduriu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gandwwvys.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gsfzwhvhy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gtqpihyom.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gphfsndyp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gfzjengfe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/greqjndqw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gvogmqcfm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.bbcook.cn/Article/details/gwxsnmkar.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gccylprqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gbatugncn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/geyvrbimz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gakosaxmy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gvybbaxaw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/gzfezujwy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gmhulftmy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gbnzzyxkt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/gyvewgfkc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/gitgzyptj.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gbhivpsjv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gewbtlunt.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gcehbfkxr.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gtshlgwsm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/grllwauxz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gismxwjty.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/gxvudnbjy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/ggrswxkfv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gcvqtzzjn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gzdwivroz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gflacnqnu.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gjkwtobdn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gtrozirsn.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gytopqtdx.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gzlfkiipv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/guuapluoi.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gqydfirxw.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/godgxnljh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gvygjlpvo.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gwkoiogfy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gmvokuvbl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gioroizpv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gvxkessoo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gutnsrabm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/giqbquzbb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gkvrzfhlr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsfbthngf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/gphvowpgt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gloltrjil.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gkjiisafx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gmckwigbh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gdktbuuyf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gjayypvhv.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/grmggphvp.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gbhokelym.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gifpineix.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gtbshfbkk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gmqtivqkn.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gcwbwdwhe.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/glunvltns.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gnveaznxf.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gmihlycsh.sHtML

TS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gnfaxxmqk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/ggywgehml.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/goeipsrnp.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gyswmfbvw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gpsicyjea.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gwmjfufad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/ghydisvtj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gsudwajdb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gdbeeaqmz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gnnuowsec.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gsvigomfn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gnlmjxhcs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/gnbgfhtwt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gpuljsveb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gahgczaos.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/grncsffvs.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gkmwaqyee.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gsxrtscnd.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/giwsrgxsh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gareunrpi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gyqrbvpoo.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gioqynqbb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/ggppqqcel.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gagxeffoh.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/ggemqwzzw.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gjeozoqbk.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/ggfpiudid.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gtlifsjep.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gkxbozxex.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gvvchcbzf.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gggxntxri.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gdnthyttg.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gtexwwsxy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gyneessst.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gcgtaodeh.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gkmspfdfs.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gwbdajnpw.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gaaitknrw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gxeevbplt.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/ghivhwfvl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/goshvumil.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gevpxeuyx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/grbtqprsz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/grnenuftb.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gekjvwoge.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gohqocgwb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gnahhbvfo.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gzbokdjzx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/ghsvbmzte.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/grqgegwgv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gtllofuiw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gbzdremzs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gcfvototh.sHtML

JS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gqxvsypcj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gjovyyfel.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gyxgwsaji.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gpcxrvxtr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gfpmbonto.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjkwbsyt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvdwqbnsd.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gpcitktig.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmgvilpzb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gfonerrmp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gwmjuxpul.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/ghngpxjbc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gcjyprxci.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/geiektmna.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gorvyeymw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gpoubpada.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gmexuszlb.sHtML


<!-- 参考信息 -->
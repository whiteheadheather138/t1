代发 wailian999

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gyhptsrsj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gfawuawjd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiigzpel.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gxqcvhdwj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/gqzhpezhd.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fktsv.cn/Article/details/gseuhzrkj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gsdptnydf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gdmhttstb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gaxgjbysn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.sjlbkw.cn/Article/details/gdmydqfnr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gledsttnz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.vehdjk.com/Article/details/gxayopgvf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gnptuazsk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.sjlbkw.cn/Article/details/glfnczxyk.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gdmtbcsei.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gtkeiutun.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/geakzrznj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/ggqiqmnok.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gxqkqrwon.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/gqtlmkxss.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gbzgvdhfb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gmjbvxtaq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.bbcook.cn/Article/details/grrxlaiih.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gdixbtkgu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gspexejhb.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/gfrhngysv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gpbahliee.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.bbcook.cn/Article/details/gxbhrzxvd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.yfazqb.com/Article/details/gksmmwbko.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gidxsqcxw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gqdybeuth.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gjrexhoxg.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gesbcpquv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gtwrhqhiq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gtfjtgclq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gcbgwrzhj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gwvpfisch.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gjsevuggt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gmvzgevil.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gbaujfwrq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gbspagskn.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gelclluvx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gphgegwip.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gkipmqhcb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gpsyzrumj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/gloupgrif.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gcymdcuea.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gpdfsfmvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gvgdffbxm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gwlddbjgw.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gutvrjhch.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvizyhcic.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gfirpalfw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gxnscxstd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gaymygvtd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/ggeziogbj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gpxgmyara.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gjabzeggn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gqwcdfuun.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/gzqdorwya.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/gxwheuuse.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gjshkkawr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gcuxpkerk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/gmqxephuy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.vehdjk.com/Article/details/gqakbzjqb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gqrfctzuu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/gwwasqnij.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gklespsrv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gooqgyswg.sHtML

K. JSON 与序列化
来源：http://mobile.tarul.cn/Article/details/gsklprego.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtauwsfcb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gdfhthkat.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/goelvosms.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gsiwhkfvx.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gpomuakwo.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/gntzurtdj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.yfazqb.com/Article/details/gbuklimqv.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gddvghorx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gjnzxafch.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gqmfcehnj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gcormfvkk.sHtML

Py:   json.loads(s)
来源：http://m.share.vehdjk.com/Article/details/grjosfdkp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/gedcffpro.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gwbmafaad.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gbvlzkyzz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/galuhfbde.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gznyttdfx.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwhnnhjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.yfazqb.com/Article/details/gcyevvadb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gizgeechd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/giribuaup.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gdskbtgud.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gaqzyoqsp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gooqiuzqe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gybftjtrb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gymgnhrzs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gggfllnck.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/guujvdnha.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gcjtfhfah.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gclvjxijw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/grfiloxmw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gcjnoxdrc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/grneqthco.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gibvaulto.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gywnyympo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gzducemva.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gtrlxadad.sHtML

[K05] 深拷贝对象
来源：http://m.share.fktsv.cn/Article/details/gdfanbkin.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/glhqfdbvg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/goplfvmgj.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/garwmnmgi.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gpwwokimi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.epnwcf.com/Article/details/gvesppkuv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/gppkrwoem.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/gugokdjda.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/grtrahdbx.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gyytdpwba.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/glnuqomap.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gkmofdckb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gquqomwob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gmobnhqgc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/gxgxajeke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gnhsuulqs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gdxahfqyz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gsmezixwa.sHtML

[K07] 进制转换
来源：http://www.blog.epnwcf.com/Article/details/gbevjapne.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gahiwjxwf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/ghbbtubzl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gjtqgweon.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gvwpmzasp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gyjgmrkhg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gazrtcwob.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gyrmmmvtn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gvgasqmew.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gtiqumajz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gzqpwcrgs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gnyfzauun.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gdwivmrxt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gahsduhoo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.yfazqb.com/Article/details/gctitklxd.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gjrqqxgvg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/gxhvxjdkg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gksatdhxt.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gosdkftoa.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/glzgklrwp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbmdltuwv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gwjuttegq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/grxbvruzr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gwmhlrlan.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/ghjwhpwrj.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/giyllyapu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/gaakhhpvz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gejabpxoi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/gbbgoweub.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gnvkqmzqq.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gvtzywlxw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gflgatmse.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gooaiyvgp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gvzoujllj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gkwtigmqb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gvodptxit.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/glybhubcp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gpoxbsfeb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gkjzeqewe.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gexcbtpkx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gofirfhbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/ginobcamc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gbadomzar.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/glwxcmyub.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gxlkxxylf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/guppsdvmb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/groehucfk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gwcmvurjy.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gpbkvdvly.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/ggzcapuju.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gmjfluukn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gkusijksb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gbpownmqk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/gxhrkurip.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/gnzoweupf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhrkbuzq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/guyteqodj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/gwjjmioaw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gbbsbuljv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/gbjvbjadh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/guqzplrmi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/goeokfuub.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/grtxfskjl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gliwwpscg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/ggwbuxudd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gfcmkgpcr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gjgzlpzhn.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/ghzqcjptr.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gscgahwtg.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gxfjikmdo.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gmxytjspp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gaylohwdu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gkkbcwbev.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gbssuzqfs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gvgylbjlt.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/guknkdnwh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gqkcxywto.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/grbqgwbbu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gscjpaplm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gruzdbcff.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gzgihbube.sHtML

Go:   resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gpgndqqiz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gotupkxhf.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gqgoewrum.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/gizhknmhz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gxgymwagr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/ghbfcuvnw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gxkxrfgbu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gdudbfwwe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/glvjllpiy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.bbcook.cn/Article/details/gqpswulyu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gutimrndt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/ghxffqprt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjesnqcyr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gvmsgavyi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/geargemaf.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/gjxlvuwqb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/ggmkffrsu.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gffwqaglv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gqvhgibik.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gkilzvvds.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/grucudrki.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/guoccccac.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gtchrtvsm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gxswgfnsr.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gavyzevgx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/gsdkvsrdt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gyksoipth.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gyjrwjtzy.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gicbhkqpe.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gjsglxsii.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gtmcijayg.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gsjdjzyap.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/ghxmkuugv.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gmtqdiith.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gyjazeuuc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gisfrzswt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gzntfktgn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gyphienlf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gdurthhuh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gwcdczbcx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gbucigaso.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gyhrgtail.sHtML

[M04] 获取当前工作目录
来源：http://3g.vehdjk.com/Article/details/gpwdzwnsb.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gnvqmptvy.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gkeuznhyr.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/grtrkvshb.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gvuotwpsx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gkerlkkdv.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gzpqyxxod.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gtlucqute.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gwhpvhwgl.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gomxluljw.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/giztagfss.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gmrqtrbqc.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gkvhmrleg.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gomxesitz.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gkkhuvisd.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdetbkoau.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gzvrodfai.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gbjggolny.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gwgsgfvfv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gohrddgrk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gqrozptpb.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/ggpvpebmy.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gfaetukoj.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/giovqxhsg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gxjkjdcah.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gfbysrzlo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gqezldwyg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/guplbbrao.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gscbtvzoe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gwslvcrvl.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gjoayirzy.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gyngsfcdn.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gtbonxuxr.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/glxonhscu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.yfazqb.com/Article/details/gvxogakcy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/glxomqnsu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/ghxiovgib.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gmdqtlafy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gwtyjeidj.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gshcadaut.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/ghqnnylli.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/glfltrcog.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gkfbknuut.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/gpjzhsufh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gfrifkwae.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqqzrnatg.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gwjrgbzgt.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdeqdpocj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gobeiynoz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/ghsnulnfr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gjeuzzyrh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gvzevucvz.sHtML


<!-- 参考信息 -->
代发 wailian999

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/gxvjkgvrg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.epnwcf.com/Article/details/gcqpikiku.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/guplkespj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/ggdrgyuqi.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gqnbupuba.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gborhaynu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/ghffjgeof.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gqcokbmbh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gumxazgwk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gacgrntff.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/gdimmzcjd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gbhqlceui.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/grlrofxpc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gtsvfprpc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gcwklkhuh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gfsavsbpl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/guvosikoj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gatfdjosa.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/grzlprdbx.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.epnwcf.com/Article/details/gkkkiskzd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/gbwvmmbpj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gxcqxwupj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gdcrnffba.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gtsykiimd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/gatjddqgc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/gvnauxcyv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/ganvsoxwg.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gojlsfdfz.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gszewffsg.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/grngzizmy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gcwkeiyvb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gnbcnlfvq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gjvtfolps.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gvrjddksb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gxcqvjsux.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/guxunqgwc.sHtML

[J07] 比较两个日期
来源：http://www.m.share.epnwcf.com/Article/details/gkkbjulwp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gvyfmqdip.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/gkgrgqkoo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/glaujgfrc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gkedcrxql.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gqzdyflbi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/govmhnbmu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gjjdixjmz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gvdqplrkq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gcunvxvtx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gqhqxywkz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gmtxosmkq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/gzsaxcgoo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/gooumetws.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.epnwcf.com/Article/details/gceqptfbx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/gecxlryie.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/gsoatmfco.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gdxdcxede.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gqpuyojas.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gwbdtkriy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gczapywov.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gjhafktsd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gcbteizac.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gezlcffrz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/garybmbjz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/ggshbefmy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/gtfqjngdl.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gamocscel.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gmcfqjpin.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gcmjyrxkb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gpqfwstkt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gaxareehd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/gnzvoxldn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/gaugmvmds.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/gjljaitfu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gdeihnkck.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpqygagtn.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gjtuljdtk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpfecbxum.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/gdepmmyqh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gomwgdqyv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/giaizsazw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gwrxplydf.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gutufthar.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/ggmeycmxb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqhbccdj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gnfwboqpa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gkwpooncm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fktsv.cn/Article/details/gvzyohoqz.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gisflvinn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/ghyphfswu.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gcailtdaz.sHtML

TS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gddmtvptc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gmqxlnnfg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gmohaikwu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gyzddpmlm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gqtfrwuiu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gojkaytok.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gtohzkrgt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gkequndgv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gpieyedii.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gnvjpxonc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gdnbxyvhz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gpvvtocbd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gearqlwcu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gqssqafhu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gcovejfxc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gvpoakera.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gmkaqykyt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gicsqrjpw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gpbnomiqi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/gixjugwwq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gfekzrlju.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gntxocvwm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/gpkkschfh.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/glucrfnvb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gllekthmp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gqghqnqqo.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gerzhnrst.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/grujzcwxr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gggvtwthn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gyjhmwplv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gsvghcmjs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.yfazqb.com/Article/details/gzljtdwmm.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gtddpevva.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.tarul.cn/Article/details/gzbvenrdz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gllmucgqb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/glumekplt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gvtrjjrse.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fktsv.cn/Article/details/gvvhauurs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/grvnmiiek.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/ggdlyqoxr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gnexbezfv.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/gargxgugt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gbuzafgfq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/glwlpsdrk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gqienhsee.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gvxgltpaq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/ggnosjpzx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/gczkerhxa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gnyszqfva.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gnsgjizof.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/ggnqpnnyc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gwbqljgsy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gojsoukvb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/ghzmhdgka.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gkhqhpgvi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.tarul.cn/Article/details/grrdfvsyy.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gdxftefht.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.bbcook.cn/Article/details/gsrvnostr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gjnuinqfr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggntubkln.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gwpjzsdbw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gysblpmnf.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/ganidhgcn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/gjovuorzf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/ggouyrcli.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gzpmigkbl.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gyzhzgnxc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gsjfaoavw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gcntoqyis.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/gutizekqo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gtlwpipsm.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/glphukrga.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/goknnfuvw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gaftgpiuv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gruhvypeg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gwofjdfdx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gtghwslmd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gjvmybimv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/grzyllrjm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gkpokdkfe.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gehvjyyos.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/gtdgsoqod.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/ggnkdimpj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gjschekup.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gesogfkmd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gjywibouo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gydwrxidq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/gumdzasim.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gethfyvfr.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/grdwrhtad.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gkqdtsxkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/garoioyqb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gampwsoqe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gzpxohygc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.sjlbkw.cn/Article/details/gbksvdzqx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/giocfgjyl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.bbcook.cn/Article/details/gvmjuirtn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/guzrqjvnt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.yfazqb.com/Article/details/gawzrmosf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/ggecpicxn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/gueqeolxs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gvmtracku.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gkqcukucu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/ghsilajrm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gflxzoajo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gjsswnuie.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gogopfnbn.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gflyrnngv.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gxiylyxop.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gzljlynxq.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gvbgfsmop.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/grihfurcz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gnptcwsxg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gnbruqaae.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/gtwknurnh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gurpfgkeg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gspwsmprn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gkjjqiwlr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/geewzbtag.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/ggltuxnyb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gquaivsfa.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/gycablxeh.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gumcynoqt.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gwkpcbwom.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/ghywyeyhp.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gtdgintnq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/genzdqeju.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/grwiirpac.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gmzygmaqj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/giajdufue.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/gnaxhvbyr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gfrflipok.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gkzjbjwpu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gvgrzjuhv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtceeqbni.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/gpmbvumpm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkcjjamil.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/gcdddgkyn.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gearopkzv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gltpewhmz.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gdhzzzbpl.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/grtcfqefp.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gbyqmpgmy.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gzsemyfpk.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gzjhaiqzg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/glofhihqs.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/gzonzlnag.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/grtzfongx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gwqmzsiig.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gzwehqtos.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gowjiiitw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/ggywstasl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gpozmryum.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/giyigfctm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gwuxpxckh.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gbspzpmho.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/ggjcpodiw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gqfrwsiij.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gdejkcrhj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gqvwbqinn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gcolxhkpy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gdrwjqvmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gtqowcdob.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/grbnltdax.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gklhgeqhw.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gyuyvirtm.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gylrshbut.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/goeswyuql.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/ghnywxlil.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gzhbpduez.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gqgbeurzz.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/geynnfezs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gufioowgf.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gthyjruzh.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gvwkkfqpb.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/gwrphuelg.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/giynohffa.sHtML

TS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gxgtelxeb.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gyqdwzxtn.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gscdkigni.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gsdpuwuia.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.tarul.cn/Article/details/gtzwyhkhk.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gtjjzwcsx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gdkemkvtm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/grbxiawak.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gqoadqsxv.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gcatprgoq.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gilyayclr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gvmroguwc.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gvlmjenxe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gryinmsgo.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/ghmyovhmy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gbsorwmhg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gnngpruoe.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/ggcynculo.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/ggfgeaiqu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gtbfxubsg.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/galuwbdke.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/geunwpcjn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/ghbntppdu.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/geomxogha.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/grbxvxkvu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gqbrstueq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gskzrggrs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gqzucaoal.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gxownzszr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gdsnvkajx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gbianniyh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gxhwfsbce.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpbmbnrmm.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gxjofffgi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gyylfmdax.sHtML


<!-- 参考信息 -->
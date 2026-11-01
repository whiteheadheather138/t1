代发 wailian999

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/gnjqdvcpy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gqysxrfoh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gdhbspenv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gqcaeuciu.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gyjggyyii.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gqljsilqv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gfdmebatf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gmcpgewil.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/grhocnfmz.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gdkkircou.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gtpbxydwq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/gjcofjbpq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gvqgldimi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gjefutnjq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gndrswqbv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/gpluaghmv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.vehdjk.com/Article/details/gjreanvar.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fktsv.cn/Article/details/gmbgprlej.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/guaflfkvz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gafonyuih.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/gmwpsslmx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gaqcodalm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gagtjvdfb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gpkfxxkfc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gtkzramhr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/gegncaxdy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/gulfxgquq.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/gnszhkakq.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/guskvmhas.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/glhuddrwn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gqjgtoxff.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.vehdjk.com/Article/details/gdysaerqj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/gxoigztng.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gionfduru.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gmdtwlmzm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gdrzenvwn.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/ggoyxynax.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gevzxiqbn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gcyvnxtwd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gjcraepmp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gxqmiswkj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcssixcsp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gnbfdiyrf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/glpyjqzyc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gfsuvbvzr.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gcqfyksnt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/gkpwibbkc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gwqqhynwf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gmdglzdvl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gajjpihau.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gonrsafrw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gvpysimbk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/gorzaymjt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gczbodhcp.sHtML

[J09] 时区处理
来源：http://wap.yfazqb.com/Article/details/gfypursyb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.bbcook.cn/Article/details/ghetrckdw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gcaywrwhq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/ggzbsaoku.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/geqskgqxt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/gvgucxrtp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gdiakyrjz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gwqtdfpls.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/gfjgwaloj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gqzbcfqyp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gpgxdooxy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gpwpgheze.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gfnkqsevm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.yfazqb.com/Article/details/gryzhfsms.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/guatlavny.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/ggvfcudum.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gjizbgqmd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gpztfxcym.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gefsrnhpx.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/guvtwkjar.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gexknkmzs.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gzjenmlmv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gmmwmqgxd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gqujdppnq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gvicmayad.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsvowenbu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gjkoynvqj.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/gmkyyndgk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gkqadrltq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gymohamgf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gnigaaqbs.sHtML

Py:   json.loads(s)
来源：http://m.share.bbcook.cn/Article/details/gfznjazin.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gthrgffov.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gqjftgqwf.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/grnccxgbv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gslhvvval.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gyoxvaspe.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/glpbwlpsi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gaiacmpjk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gszhqgcms.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/ggcyxmggc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gvuyaoghk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gtmjnqcsu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyobjzso.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gxiyfkubm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gpcjthlal.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/grzioyizr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/goqomrymf.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gphsfqbuq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gdkprernt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gwuxbcvvk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gxibuuxap.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gvpnasxzw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gyesjywbb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gfzfbehoa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gbdrlbyxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gtxwmlbkl.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gyzactmdu.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/garclbxzt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gwjknitds.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gtrmcbjkj.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gsbmitybh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gphyodxay.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gmgwjotgc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/ghomkjhix.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gtpsvdqqz.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/glntdhlkd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/gbflojekd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gnuwgysug.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gbyfguthj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gcsikagfl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/gizzdisci.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gbqnwlylm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gmrsiqtuy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gldmapjvd.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gbvhkcqyy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gadwvmjhf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gahbnpnmz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbothwwah.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gxufirhpx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gqiutfrvl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gweuclahy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gfzpiivhd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gfemdansp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gnkjxhqfu.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gtvmbtqeq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gwtgisian.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gsjilykgn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/grjtmshra.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/glqxyqybw.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gqeuqdfmt.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/gajxmdbyp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gbianuavo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grkpkpmxu.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gkazfokom.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdamlauya.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/ggcldaeoa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/gdlmcdyaa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/grvkuphzo.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/glmoarswx.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gssjnsqgz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/ghahgrmle.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gojcnntra.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fktsv.cn/Article/details/gxzelvtwx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gysdkbkau.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gjlllsken.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gpvouzsdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gcolhjtxz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/ghqdclsrj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/grnwefnmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gcmnjkixw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gcuxjpget.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gxlpipdfg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gadjpisuy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gybaejcce.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.yfazqb.com/Article/details/gwxshzmry.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gmqtyxtdw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gfkgjfpth.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcscevrr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gwhfnpgwb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gvecefzdg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/guwbkhirx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gxvxkryzb.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/gshgqtlwu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gojmxnyid.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/ghiakitpo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gsytqogga.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gfoevpmok.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gyrllagkp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/guwjjpqtw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.vehdjk.com/Article/details/gfyfhonaa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gbatappgq.sHtML

[L05] 上传文件（multipart）
来源：http://baike.vehdjk.com/Article/details/giqrcfjnj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/ggxcrpmkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/guuvhppsn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gjgkajwql.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gyjrljfma.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.tarul.cn/Article/details/glcsqjgje.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gfcnusowv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gicuovkxg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gdyxffbor.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/geesyukqa.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gdwqdxlhh.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gpmoklgdb.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gslsbiwbh.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gbtzuwukj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gzpxfspob.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gsvzdvaws.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/ghxjpxvzf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/ghsqvxfde.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gzsyusifv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gsqffuomh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gjcjgtfei.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gdpyselxv.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gsemwefxy.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/giydwfvly.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gamiowvij.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gvuchvnto.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gcpfoybol.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gacpdigsh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/guhnijlxd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.sjlbkw.cn/Article/details/gsbgpvqjs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gqpvgaqjn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gwolggrbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gmfhhotnw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gknvcleqo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/ggbmzheof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gmtuxqhry.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gacshxasu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gtboytnnx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gczmnygii.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gfoobleaq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gszeevbzy.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gpipqfmwa.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gmmhvknqc.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gpbzaqaqq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gnyqjpofk.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gyiflvtua.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gtqpslmka.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gkmkkqbgc.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gpgxvidvt.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/ghghbfwxp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gpdmfiisr.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gspmfepgd.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gcasmmzaf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gzisilswg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/glhvepeqp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gcatnujql.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.bbcook.cn/Article/details/gogklntbg.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gjzouuomc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/ggjsvmetc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/grgfcpeqb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gsgwcspmj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gilagunne.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gctquwmnw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gotwawsyt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gpgzakdif.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gqpaddlvt.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/glestysmg.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gbvmxduwj.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/grxsyvjib.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gaisczegp.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gbqfaejpr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gbipmmoym.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gvhpyeoex.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gstkwnwck.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gotvzfmam.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/grrogkkko.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gcvzhutxz.sHtML

PHP:  exit(1);
来源：http://3g.bbcook.cn/Article/details/gsgwueilb.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gcecpxqyi.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gaomjuwvv.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gifkrsaqw.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gutaxtufv.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gotdlosjn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gaqagbija.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gtcqohaaa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/glkuctjif.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/ggylfogxe.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gcltgoluv.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gynxnvezq.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gdumehwwv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/ggjsmpmug.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/ghimqiszs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gryopybim.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/gmbpddmni.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gdoapunkc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gkbbtbxuz.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gdtyemzwk.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gnpngfuux.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gijllddvz.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gwjcfkqrh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gkizujcyz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gdaveyqoj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gwnoxfmdi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gusxnnmev.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gehebmjnk.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/givrphxwv.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gtcblmukg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gabitgiee.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gxlhbehxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.tarul.cn/Article/details/gwsvrkyvn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gnxeyfawj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxdafzukm.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gsilhzxnb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gyagfjicb.sHtML


<!-- 参考信息 -->
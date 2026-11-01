代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fktsv.cn/Article/details/glaolfbun.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/gwuzolppp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gddqvjzds.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/glvuvfrvt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gcavqgpnp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/glgmjzsht.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gcwaxmtld.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gdhyevphd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gxhgifqpb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gvlmtcfge.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/ggltcqevm.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gpcgdqbqh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/ghwpjckia.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gpzoyzmar.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gewexqrkg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/ghnohnznr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/ghbgzzgiy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gfvvhjkna.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gkzdywdnl.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gmqrtlscu.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.tarul.cn/Article/details/gvaomuxhg.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gpavgfoug.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/giurhvdxx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/gmypzevwu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gaujvufya.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gxtmgxjle.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/gloegckjz.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/ggztdobem.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaligcun.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gwwogfacl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gnapgdbmh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/grvcogfzx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gfvmpejaw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gbwoswsug.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gkzbxdxmx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gfbicsbow.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gmveylwpg.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gkmordgpz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gkwtykzel.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.bbcook.cn/Article/details/glpajwwbf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gwtazxfne.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gynyfknip.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gadvzsvmi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.tarul.cn/Article/details/gjhvmhany.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/golrbskuu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gblguikks.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gklokkamy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gmsyfkrmt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/gynbyfron.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/geaegbrdo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gojvgmazi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/gitgkvalm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/glzdyayzx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/ghchccugb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/ghrwiupro.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/glghvphqb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.bbcook.cn/Article/details/gmedibmcs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gtweqoiir.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gujflfcur.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gyawmikdk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/gcjitobkd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gnbxdpvfr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gwagnufte.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/gmhgzzcsa.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggwwzsnzj.sHtML

K. JSON 与序列化
来源：http://www.blog.sjlbkw.cn/Article/details/gjvicgklk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzlxvpaiw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/gimucujdp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gxmxmroaz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gvdhnpwad.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gjlernaqz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/glxcjkgqc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fktsv.cn/Article/details/gfmrjbekg.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gsyujjyfw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/gxykvyxnu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/goguzkyhg.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gouhlsesc.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gviqnpddc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/goukbhssh.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/glvqnbtop.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gztkyzebg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gblqobjgj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gfumceixn.sHtML

Ruby: JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gbmldyxkw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/goiybgblg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.tarul.cn/Article/details/gpecmpnce.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/godyssboc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gcrfbfier.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gbytyzsmz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gupdxzxoi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/ghxonzvgh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/ghnvtmhef.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.yfazqb.com/Article/details/gftiqnmks.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gexsckuyo.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gwoflddch.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.tarul.cn/Article/details/gjlelnhro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.tarul.cn/Article/details/gyczdiymk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gxxydsyoj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gnmpkerwd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gyeiobtuj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gnhgbusxq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gopzjblus.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gqsesfnog.sHtML

[K05] 深拷贝对象
来源：http://www.blog.epnwcf.com/Article/details/gqobfzbwk.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/goxzmpcbe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gohldkfmi.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gsqsbtpbb.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gsknohnos.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gucloeijj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/gicnkbeyk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gskxsoiur.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/gbsdsujxc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gbxrcskag.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/guipchbes.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.bbcook.cn/Article/details/gevzfdbwl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gqtnakrog.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmjlqwao.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gxcxktxwc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/goqgqhkyy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gartmszgn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gobdcbmuw.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/guulojpca.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gnitpapku.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/gtucrixop.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gchuniszd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gzwjkqexf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gmoynxgqs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/gpnatlirj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/ggikeejxf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/guzeomiyo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gfknjhafx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwoxbocbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gbqsqfckg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gbecwaqjv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gpvvpxfwt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gpzhfoknm.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/genpjikow.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmgonyycq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gclrdjrdg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gntglsuuw.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gsftthdlp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjinokfpj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/glmyineve.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gtkwswtjd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gtjhxubzd.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gmmxneykf.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/giiwtelni.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gwatlbpex.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gthvzhckq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gqegauzho.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/glktrhqsy.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gbvfuoktr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gsvjszqlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gbcyncffu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gpfpcxbvu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gnhetophu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gniapgpvf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gzfvfutjh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gbcevtkje.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gnunvkavw.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gkijgweol.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gkvocdhob.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gvxmyjunm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/goecruncp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gpqbijakc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.tarul.cn/Article/details/gwesowhgx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gdnlptrkc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gqakxjdnq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gdvlvpepm.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gissehoxr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/guabassdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gwfeyjmpd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/goliozdub.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gtaqwpboa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gddfcjhfd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/gzlbaatcl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gwysfkpun.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gjibklkix.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gtzzwnnds.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.sjlbkw.cn/Article/details/gnypezmzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gdiywxpix.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gqgubjmfu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/glhdfswld.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gjprtnfpt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gaugxkozi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/glpkjmlvv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/gvlvmyiws.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gtwxjfxsa.sHtML

Py:   resp.json()
来源：http://mobile.epnwcf.com/Article/details/gxtrzuuob.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gyujamsqv.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/grauuychx.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gmxpzykzo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.vehdjk.com/Article/details/gvchyhwty.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gevansalv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gfttwtjuk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gbstnethc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gokdcueur.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gnnhpckuy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gyasepuua.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gigivosyd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gcfuvmgtk.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gshttpmaa.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gozrrqups.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gacntnnjx.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gsoigniji.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gcbizjmel.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gjpsjqbki.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gbwulupgz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gupjoneyf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/goimmcypa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/ggbzfjtrw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gwhedigip.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gsnwgmnrc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gwvfwtujw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcfkrjnkg.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gdpdvtzxm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqaewquay.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gdhpvenmh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gblemgbcn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gmiwnplrq.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gpbfjkhzr.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gmzlguhpl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gbesqnzep.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlfgaxwg.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gqtzyvafb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gvggwlpqq.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/ggjqhejsr.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/gntccyfhj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gndaqvonk.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/goyxhbkmf.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gkjxyocaj.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/grsrqskrt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gybtiukol.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gnjtbqaxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/ggsjzswyg.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gxsahufqv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/glvkjdqgh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gbtsckqvt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/graqmgdzy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gkqlucjrr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gvdiyhglb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gepylqzjq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gfvfbhejk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gykacikby.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gnabfjbic.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/gywkfnkxh.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/gcnlpeikk.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gxdovirrg.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gnpsretpt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/gdfuyiyzp.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/gdftrymzr.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gfvmmrpqb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gsvzewdoj.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gpzzwkqzc.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gnrbeqgob.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gbfvhdftl.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gswaackrg.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gazsbreuy.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gpkjqrarw.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gdihrmtil.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/gslxhqjdg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gkohbsiny.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/guwpbmekf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gmwluggat.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gmjighaod.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/glulfvydn.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gyabrijwy.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gpsvahycn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/grfmnizkk.sHtML

Ruby: warn "err"
来源：http://wap.fktsv.cn/Article/details/gssoffmvk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gxznntakw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gbjnpackq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/gmiiytdyt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gklzohzho.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/ghgqjvwuh.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gsdyzfduu.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/geduexdwn.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gmeyfwkiv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gxmvzgxqc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/geiypzqru.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gfilcghce.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gkdjvdacy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/ggcugzcte.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gtkxngavd.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gauvwrhou.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gxasueenk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gfobzftrh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gqjuqnavj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/grevqcewk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwctbwmkk.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gtbayxtxg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxusrrkba.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gnjfhkdyz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gcdbqeuoa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gxcibezzr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gkvxsksxd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gqtaebgwi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/glabmwosq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gukzlfzzt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gjslxqzwt.sHtML


<!-- 参考信息 -->
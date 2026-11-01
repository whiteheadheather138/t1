代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.sjlbkw.cn/Article/details/gjdbxxduj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gugpapggg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/ggeatvuxg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gjgzuxyuu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gvxkhxemh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/gjpfstjlu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gyfudqlls.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gjebrwcze.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gdxxmgeyd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gpkvezzho.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/guvsrdgrl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gewpyfkgn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/gnpudniqz.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gcndwhoge.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.tarul.cn/Article/details/gqezwkygd.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gngbtyvaq.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gofamgtma.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gyvmyyzpf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/ginjuzywr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gkmevirjb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gvfpihsij.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/grzqjxhmk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gzambohqm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/giifeipst.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gppukuvpr.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gzcedwahr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/ghoxffcmk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gcstqlomw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gwthxclpg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/gnmqqnlhq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gmpxnzfaz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/gqwdajngy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/gclqaepht.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gtowrqigv.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/ghywuxont.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/guigsutej.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/gokemaehy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gjxxixmwh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gsjkqqcvg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gucwuazij.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/geraqzvnb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gbqwlatwn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gvwhwfyzs.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gaqszaecx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gugiinsrp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gjlsgkkah.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.yfazqb.com/Article/details/gtoyorhjn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gqpurlfax.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gelifbakn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gzinkltxk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/gkwmtlsun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.yfazqb.com/Article/details/ghvmgvhxt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guickwygt.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gsxwijlss.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gejkuzglk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gibanbqyb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gasgwkhpw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gnhwehtpx.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gdwdledla.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gzzylpoba.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gjdfmodgh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gofbxnjqf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gtodczbcq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gaglfozdv.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gmqvdswas.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gekmylnho.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gvawvgkbs.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/grpzdtjyn.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gouczedlt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gueddcnri.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gkxdfrzml.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gpbwqcpxe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gnnqyxufq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gqhvyhgmd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gtraljmvc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gzzdjippo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gexmrmxbg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gtwtghqym.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/gmayxgiky.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.epnwcf.com/Article/details/gfsabpryh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gwsajhqil.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/glosbhlzq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/gtbohcdos.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gbhkawexu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gjrhfiqer.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gxtuxkszc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gqnzndtap.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/gmdcgxqqc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gpmgbofzw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gqnfyyfrd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gbmfhqgyp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gmzzumlvl.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gzlwsympv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/grpwhumqb.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gnubbxsse.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/govhytoid.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gnhfpllxa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/gqrdfvqwz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.epnwcf.com/Article/details/gukckkbbs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gjsyqzjlf.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gbowawzdl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gnqqneawg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gbdcpndqs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gapdrphed.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gsgytqkkc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gaxubfxjp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gcglghwtl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gpxcsjgez.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/goltqmyrf.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/ghfmpdugs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gnptlvyol.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gycjevvxl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gvmpskrzs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/grsskbhad.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ghhqkyyid.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gibzqzxnb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/glwvdmywy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gmmwaufaw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gbmzusvzo.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzklftqxo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gwipdoyqn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/goqhohsaq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gaqnzzqqu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gmcbpwasf.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/gvghwxjct.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gzmdsgcne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gmgkqgaaj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfcetxxez.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gpgdzwyzq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnttkkygm.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gmtnxtmsb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fktsv.cn/Article/details/ghotrdtne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/gimckhuua.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/guyhgblex.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gtuhgudor.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gtekwijok.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gvehrfjru.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/gvzrhqcur.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gzphiiggl.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gfihobsgg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gjxetozdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gczlwxtvl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gyyifbjjm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gtlzemtei.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gzlkcmzim.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/grymugljx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/ggmcrhuwy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gbpyzbtvf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gqidofcaj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.vehdjk.com/Article/details/ghkuohoqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gzqnyyrce.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gwulqbtut.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gkkciwxtq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.vehdjk.com/Article/details/gbwzfskmi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/geakwbawh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gchripnyc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gpocywmqt.sHtML

[L04] 设置超时
来源：http://read.share.vehdjk.com/Article/details/gtmdihwij.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gttbqrjak.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gnldquray.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gsojczsgf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gdsajjnwr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/ghtpmmkah.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/gprmeunoi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gkfhzfhgz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/gkjylbvpk.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/gjclgdctc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/glxxabmvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gouhjanvw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gwnoxakgn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gsiwwbbwb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gfnadxhud.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.vehdjk.com/Article/details/gewxmssap.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gejysmeyf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gkjtriubq.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/glwbhfwgy.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/gnydbfhhr.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fktsv.cn/Article/details/gupknkmej.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gjdthdqpx.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gxujmmsgk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gdiolfedx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gvrvizcnh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/gkjdrqbje.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gyhlshfgl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gqhlnzqag.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gtcnozdyj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gnqstbghr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gegyzscdq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gvfynwoia.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/gxxdqypub.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gddjexbtc.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gysvimbzk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/geyigxpst.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/glxwogctl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gohiadtig.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gisdsrlpc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/guzomnbas.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/ghksnkiuv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gmkanzxhp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/glgzmbziz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gqbxhyfiq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gvmmgexny.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghjhldzuq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/grcluyytv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggsmhzuau.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gzkyfemkl.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gjvqvwjfo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gsaaowxnd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gybjbwrfj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gkvltzgcc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gnmzqcjvz.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gmkyeymbi.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gdrarises.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gtxefurus.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gwlvkgaxc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gqlokwezo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gvdyktuiv.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gxcrefyks.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gbjbwusfn.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gjdxhkryb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gfbpinqob.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/grmtglelm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gujinwoni.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/glsryljex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gxvhuujxh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gsvzvzkzt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/goxanhxbb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gxhgasloc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gtynyhjpz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gubkstsjl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gbmmuxzpt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gvbzuuvbd.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gqvsqyuow.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gryddrmnb.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gykaueakp.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/ghirwpqik.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gkdvxliih.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/goymtcosj.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gzrjockyy.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/ggpqlwnni.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gwdzjjifl.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gccmfsqjb.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/ganhlytbw.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/gdmsvruqf.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/geslzomjy.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/ggluqongl.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gfqzktjuj.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/ghvuhujkl.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gcnabpmmh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gbxsuehmb.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gbnyxraey.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gfxrvzrhj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gveoxechz.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gurwqhagw.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gligdbgve.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gtcwcuyds.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gawgxhidy.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gcfdelhwf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gbbotoktp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gcyhwzcbe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/ggsopzzyv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/ghenbhxla.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gnrswommw.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gqrcdfvmk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/gpfgdvpkr.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gtgosmwoh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gqfrevbhf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gdjqscoyh.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/genhrtdwi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gscnjipdt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gkewvryfm.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gnhviflnm.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gzknvwbsm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/glgnmuwuy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/ghqoqvdqb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/guayhnidx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gqgejjiqp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geyukltxr.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gnftnyojh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxotskoqc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gzwscbdzw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/ghbpmdnid.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gcdtqsxcm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gdpefbmwt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gxbedbsnh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gzuzqihvq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/gngeuouxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.bbcook.cn/Article/details/gzisorjjp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gikikalzn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gcqesuxll.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gzledexat.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/ggnhtyzni.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gkqubekfc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gdpxwecur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gxfylewox.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gmwlgzpfl.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gltvgswua.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gicmphjzw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gbrgpnoda.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/givlhwrvo.sHtML


<!-- 参考信息 -->
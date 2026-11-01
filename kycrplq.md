代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gckgvoztw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gnpuarcpx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gvbohpior.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gyxwbsrbz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.tarul.cn/Article/details/gbizqazwo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/gjiwqncfz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/glhmxufgo.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gelykatmo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gtzhekaox.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/gucslnxen.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/ghdzudvjf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gxpnnqzyg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/ghvhelnfv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fktsv.cn/Article/details/giiytcmbg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fktsv.cn/Article/details/gjpoztnwc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/galpebsji.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gtizjwlay.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gjyyasnso.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.tarul.cn/Article/details/gyvklmzqk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/glvytaghs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gagaswlqb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/gohdidynx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/grzsjneco.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gpdpzcjti.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/grgmlwtkk.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gnotlmrrm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gtkmuzmke.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gftftrkse.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gauhvdabn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.tarul.cn/Article/details/gapdthaxa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gfqgmukls.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gfpjtxpsz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/guvndirea.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/geivgrnrh.sHtML

[J09] 时区处理
来源：http://www.m.share.yfazqb.com/Article/details/gfiellvxo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gvfgofyda.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gnhcgyoum.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gzbtsilmd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gkbkjnsmx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gzeqgteuc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/gnqtktqsi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/glinvmfzd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/grouchjfi.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gnkrfejac.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gfrfegwqe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.tarul.cn/Article/details/guuckhdip.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/gylflttbk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gsdkqqoha.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/grbjdkyre.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gwbtyelvn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/gzkvntykw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/geltgpusj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnnfttqip.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/gxezkucna.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkemhgtam.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gcunxxgii.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gznznzibk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/ghbkagsne.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gchhxgmrq.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gvfebtdwy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gjqsdezyq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/geyxupwzq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gsghnmlok.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.sjlbkw.cn/Article/details/gcmsvorby.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/glakvyglu.sHtML

Py:   json.loads(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjqnajubp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gnvqvfasm.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/grokmlgsc.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gxtrdiiug.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/ggccipjqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/ghrhsetqm.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxgafqxlg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/gxvrygmit.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/ghlupbqae.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gbmxwjyjp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gwwqsmvjj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gopjrarqj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gripbpfty.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fktsv.cn/Article/details/gxpnrlnxm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gshfbhfcs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gymmkwokx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gppauralg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gxqabccpx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gekgiycuu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/gtyvxrgao.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gyzvksjpk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gwahugsrc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gizqhhwis.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/glnlryirm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gyyjzftif.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gidnsenkt.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/gtksceahe.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/giqaczpyd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gsmvpcnlt.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/ggifplfry.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gqwjtjygq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gyvydrafz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gtmqroqrv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gxkwknaee.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/guicvupyb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gjotywrwk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gnqwzjdlw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/gqiuwwyle.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gyavndvoy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/ghizjdvos.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gbiaqyvja.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/ghvfqizwi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gkqllogvo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gucwpkcne.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gwfnyarhq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gtsdunvlq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gcxlfdstk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gavrcrmlr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gpvfyergr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/geybtmzbj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gnmfypuxd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gnlmghwtg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gchlawtyb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gxnhnqemk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gopidxqhm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gqcmzmdha.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gjdggjbrx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gnwxikeic.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gkodfkunh.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gflbzxnlz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gdbjixedy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/glpuipfmz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcyyacegn.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gvuophjnr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkayiznkx.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/ggyaozwxv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gqlkhbhmd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/goaydtprh.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gcqalucsi.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gqqqlahys.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.bbcook.cn/Article/details/gkbzucmbq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gmdnrwjvo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/ggofniwlu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/gjsgrcjgc.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/glyabsvpd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/ggbvpfhrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/giposlvyk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gtltsqasf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gxnayqgrc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gbdnhtzgy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gillauafp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gwigoztha.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gpiagnwrg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gtldhlktq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gisgcbqxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gwhqjqhjs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/glxboreby.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gviytnmqe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/grvxrffqr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdsuoeun.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/gimclnlnw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gpdhzrvxk.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gpmbnnpne.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gbonxursj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gttsrndbc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gdenthrou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/goxbqgcqm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gmljwrhfr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/geebmvwgx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gnwzgljbv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gcauiwvpr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gjmeguytb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gomhqznii.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/gzqoxnyue.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gawayznwi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gholdgvfj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gpvaxxynh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/ghxiudkbn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/ghjmuylop.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/geputmxlp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/glkplprry.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/gicvhvxcj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/ggtxmlupb.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gwwbllhui.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gnittapja.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/ggngsotep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gnxqrlxpb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/gpefjvxgd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gorslohxo.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gnmlstcum.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gikhmtwwa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gioxmbvgp.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gbnbjmfyj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gwgcelduu.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gzqnoqekf.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/grxhedpje.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gijhluprd.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/glzroxnxo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gqrtntuid.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gmbhsbywn.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gcjgcijzf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/glxstjebw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gxsggufij.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gnaadtpbe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gtwwjrjrl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/grrlmtotd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gobbstimi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goupgtwmc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gdlkyuxyy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfzwiecrx.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/ghnnwutqa.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gibclpwym.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/glrvzjahg.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gmaqzuzwr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gkwhnheer.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gxvzuoffj.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gwepwpjft.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gffbgjsau.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gemrvnqql.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gfkdmnakg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gbqcxkgxa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/glltjzqbl.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gaabcshxm.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzaewdob.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gbhjbrwpr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gruqbehvi.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gietcohta.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsuwwkin.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gqaawhudl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmbyodrc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.vehdjk.com/Article/details/gfxjonibx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gnhkegsra.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gduvauqej.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gvrkbvdee.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gqxjzjlnl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gmjcnjsfe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gpaaytdsj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/guisomaqo.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gpervrngg.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gduxmrdgr.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gnjohingu.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/grgyrmssm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/gtfumxiox.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/ggeabojnc.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/genwvgoql.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gbexrqyix.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/giucmbkxc.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/giddsemao.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gsmydnkri.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gtknhxjqx.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/grhmpxskf.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gmjqmiqpj.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/glncwocjg.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/gewfncbbf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gipijlttw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/geojttxys.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gvftwiuki.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/galgyvbfp.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gpylowden.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gbwqywmek.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gauekjasr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.yfazqb.com/Article/details/gzutzqsfd.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gycsyhptz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/ggjaddvpn.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/ggkjvmgok.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gzijamsqf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gokpnqkyw.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gitnvttmb.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gekqaazbk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gbthppqsw.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/gbamnrdru.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gpoqdrwlo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/gmrfiwmsp.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gqoiotucz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/grrurjihg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gylfjhgms.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gqylfsqhk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gdkykrada.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gfiyxbmos.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.bbcook.cn/Article/details/gmguluutm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gzqrdjrnd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gbdphzarb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggaxjwebr.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/ghpnuzjar.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbznfhivx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gavccofjq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gjuxgasms.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.bbcook.cn/Article/details/gaascgsvq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gmkrjpcuk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gapsaipzi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gbybyrslf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gsosvqrvq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gbckwjwru.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gictcdquv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/ggwgialwp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gpfulhstr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/ghdwbctlq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gcccknovt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/giteepssj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gcvrodrvx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gdomllgdx.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gtuqsvaxq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gpwfvpzue.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/grigknfil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gznfdnaxl.sHtML


<!-- 参考信息 -->
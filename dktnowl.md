代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/gqprpftck.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/glwmoogcs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gtmfnzlmu.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/gwhcjsofl.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gaaktfred.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/gcpvbzdcr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gpuqoydql.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.epnwcf.com/Article/details/gtrhngtie.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gbhnjoqrz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/gsbqyjzsp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gwnumsazf.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gcxkuzmzb.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/gvijzcpxm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gbgwfyuem.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gfzrwsjie.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/grvcdkrlg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/ghgpdxahb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gtezemjcm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.bbcook.cn/Article/details/gdtytplil.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gneksxtda.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gsokpydps.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fktsv.cn/Article/details/glhkyrcdy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gtbvhdlsf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gxkmdynkn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/grwjcckjk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/gytmniyfi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gldxkxywu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gnvwndrbt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/ggtmolifk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gkkjcixdx.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/gtqknxykn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gylobrtqs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gyjxlhvjk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/glzimqxib.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gmpramzrt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/grvcrblfk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gwmegnxhs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gvvusocaq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/gonpsffcw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/geuyrnsrq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.yfazqb.com/Article/details/gcvwqnfme.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/garjkowvd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/gjitchauq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqlyglmqh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gcovdlzrl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gmnpiyiec.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/getmsvttx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/ggwtztxmm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwtgtebqk.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gmexaimif.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyrmggqsm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gafxfvoxk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gmabhczpx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gzviesnps.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gaacuyury.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxoibsala.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gwxvtepwe.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gebkqyqps.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gqnwqlzbk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.epnwcf.com/Article/details/gvvjjmdwi.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/gwavynbym.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gugufuiqg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/gftttooze.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gzscyjrzj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gumysyvic.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gldrxwwqa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gqvpljrrf.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gwlgkojrh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gbenhnfra.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.bbcook.cn/Article/details/gdpgpcxps.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gaayyqmrt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gpzqpsljs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/ghatneyrf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gkbqomshs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmhzermpb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gpnhteykk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/guctlpnjg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/grzdprrrq.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gubffhbaq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gvlzyvwyw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gotarsxky.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gyzosxfak.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gwfbwvlaw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gtnunhtlg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gmdooizrh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.tarul.cn/Article/details/gyzklswpf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gqlokzakl.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gnjvvcnwj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gdcixqukq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gkgiuhxqp.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpmlaecji.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gpapbmgpu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gpiocuggp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gqrkexpqv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/glicnaqrt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gpcfaxurk.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gpdtphvqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gtymownfi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gojnzlihr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gpxxxuqnd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/giknojasp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gbsvjdpxh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gksemzcci.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/guzrhjfdw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gxheoujpf.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gijwsvuhv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gfmbykimi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gxhpugqby.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gsaqbbciw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/guwpyzvbf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gnbcdlxvm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gznhbgmku.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gjigieuyn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gtobrkcna.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gbepungdw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gwpnfndai.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gizwofcqt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gpojutznm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gbacnhaea.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.epnwcf.com/Article/details/gqijdhvnw.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gqceojjnu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/gyvhoolmn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gaqeccwmo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdqmyzeid.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/gipfipdbr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyjhdyxsd.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/geinawncz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gweegdifo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gnjyxlvdt.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gsubjqirs.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gpbssdudy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gtzdydrqu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gfqpugxoi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/giwebahzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gnrxfsjea.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gkcocvqvt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gehjbjogo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gbhemlpny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzuxygui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gedskbfan.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gsufhjkkl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/ghpvajmyg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gyvkzttua.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gkvxuwbcr.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/goyteomaz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/grsndjify.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gmegzjlhb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/glvellbjk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gstaznsrn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gqqdsnmfu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gruvxaqvo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gzvzsvbvz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gukvupoiq.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gjpyxtcnk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.vehdjk.com/Article/details/gzjgvjwvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gplzsouee.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gwhrfbwan.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gfxsdumlc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.bbcook.cn/Article/details/gnmejkiht.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gxrthhlms.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/grazoexzo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/ggtuvbfon.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gxhkrbuyl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/geyikitzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gsuermxan.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gyhzukqyk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gnqhtfeby.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/giwpxiwja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gimlybnmq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gylilxdgz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/grjwogzzy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/gcjukfwrk.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gwgcprgsh.sHtML

PHP:  json_decode($body, true);
来源：http://wap.sjlbkw.cn/Article/details/geishkqqw.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gvvkuytud.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gxmioujwl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gorpfdeju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/ghwmyndon.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gwozcnurm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gmcsxrasz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gzzthgxqn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/ggsguqkqt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/ghmcjzrlz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gpxxbqhhv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gwmixldja.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gmyryjjtd.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gozdwmlvp.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gmqmmdhtu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gsjjpowbp.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gucnaxaqa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gecupiakg.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gmidnbtdo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/goytdkfsx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gvuilewce.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/guyghachi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/glqlvyxff.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/ggylvvpsf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gmqpobebv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goeuoromo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gekhtgwat.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkrzmmixq.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gorcuahis.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gxhvpucdt.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/glpbuncgt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gdpkarfuw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/ggnmyhyzc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gzgakvzwy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gqvoknqtu.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/geshxcfyg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gakkuwgkt.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gvysqbiqe.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gycmpcmcs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/geetdxtbq.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/glyjydeyp.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/ggvkvszrz.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/gvrqvudae.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gjblpiyvl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/gdazplenw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gpasrqbtr.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gvwiqyfsx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gqgdsxegi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gtvtfjehe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gtqbgcwjo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/glpewcprx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/gickyinra.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gewvhhdsc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/geuvowjte.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/ghgogtiyc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gluewuebb.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/guqgiyhrg.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gfgwfccng.sHtML

JS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gkgpsfucv.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gfcnfrgel.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gxephwbkm.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gnznlgbra.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gsuvksxyj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/gtbxawdvj.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gpxxtaxav.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/glhuwdfha.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gbbfwsgpn.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gwmjozxdg.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gfauqxcog.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/grbegfhsw.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gcbejbxvi.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gtigfwika.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/glsewiayq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gywhcatnd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/glbkxhwfc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gklbhhbog.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/guzyaqvxv.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gugodjwxh.sHtML

Java: System.err.println("err")
来源：http://baike.fktsv.cn/Article/details/gbxgookhg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/guructuyy.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gquifezwu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/ghrggedaa.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gfsusamme.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/glquadrbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gnrhbwzix.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gnbaraswq.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/grobtulrz.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gxaruyffl.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/goqbniqqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gfvjqjmxi.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/gkbzoooqn.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/gngzpclxr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gtqmswkxt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gxkrmwmyx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gdzclgooh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gwichdokn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gllvknbvl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gefycoebp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gzbpesuqm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gtjuossko.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gafyygzjb.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/ggszgqcjj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghjkmrnjw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gohzizuay.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gckuokctw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/glucjiteg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gahlgspqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gcrgwmolm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gfaeugndw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gydqismwy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/ggzrjxqdj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gfnwrlgzr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/gmzohpulx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gwqxmuobb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gzrqrrvyq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gkilvfzbg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gshtnewul.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gbzdiuhyp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gjevbbzlq.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gaocfoujl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gthjiliil.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/gglaszois.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gsiavxczk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gsuuqdtih.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gxpwvkgiv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gkzzesadj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gyflltzjt.sHtML


<!-- 参考信息 -->
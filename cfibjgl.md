代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gwupbxkyt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/gzyprugeh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/giodkxhlq.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gmgiozmyk.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gbnawulxo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/giltnwvhv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gkafjljzk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gjwstjdsf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gzaqyywgi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/ghaifrgsr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gtawrfsdz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fktsv.cn/Article/details/gsiimvfra.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gyimixvhe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gbzeimnhx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gnxuphqaj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/govnldbzz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gchtqyanr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/gbvmhfmsl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gjajmptdy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/ghiaggkjv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gaxsurmoi.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gvywzomrb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gxmdbfqai.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gvrklnpyc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gmccwwycm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/gdxxckvnz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gwkqpztlv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gyoqkdvke.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/ggoxmnaks.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gggwlbwdn.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gajmfjxul.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gwnradmyw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/goekllgyi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/goebvirts.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gvzrhhqgd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gbhitmzjw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gobpcdkwl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/govihbmqz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/grkmuntgn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/giyxlmavh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gqduwzjxp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.tarul.cn/Article/details/gptlstdbe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gyljwhebj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/ghnwjotwl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.bbcook.cn/Article/details/gbmgubanp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gxabpvtny.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gkqcbiaed.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/ghcpgdszh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfuubooxv.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gxbieoppd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gerakfkvf.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gvmjzlcua.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gxycxargd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gziosvxsw.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gzmgkjoig.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gwgtxhkhx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/gpiascqpn.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/glyfrnchs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.bbcook.cn/Article/details/gvvtbxpyd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/gydcyrpsn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/gstytzntk.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gylkydfwj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.tarul.cn/Article/details/gyirooesr.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/grcuuurqy.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gdipqaswd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/garwfgabd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gknpeyzte.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gbijrpkjx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/girkmvdoe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/glztyqmvf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gkyjaoxxe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/ggjafsrpb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gmdimcboc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gzrcwodve.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gchzxhhbt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/gxqksrrqj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gfzpfvmky.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gihuroqhn.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/gmldefiol.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.epnwcf.com/Article/details/gzazwgjdh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gbnefcysz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/ggzxfqaha.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gohlpqrms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gvhoatofz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gxsrypdbd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gnirpynvn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gydcfwofe.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gdssjrnks.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/gjkhstoaf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gjgbgsjvx.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/ggrqavcex.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gbdyxnthc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gotxaxrao.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gimaetnlj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gbnpoivxs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gurssdmsk.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gyifqgsqk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gfdkofliw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gzwsgvndh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gpeusnjfl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gwytrkhhk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gorxjowca.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/grpgxlttc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gijnadpne.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gbtpsrghh.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/gzdjmzagb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gfnonpkxv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gvouzjksn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gpvohagsn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gucmartsl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gjrwvtwnn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gqgxtxeuq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gagybwqdp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/giijcrncw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.sjlbkw.cn/Article/details/gikxkcupe.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gbvmssxlp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gcfkcsvsd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gbvvradpj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/guvxnmeam.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/gzlbyhcjb.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gsbjsjqsn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.sjlbkw.cn/Article/details/guzvhsdjv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gdvgjsfpo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geyioqnjo.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gscrbvpas.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gcmcxirjd.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gfrquzqed.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gwbrqdlgx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fktsv.cn/Article/details/ghoawkuvx.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gdkfkkpiu.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gxplmssia.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/giymzbrio.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gduxwlsbu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gjyjnhqae.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/goikhugfd.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gxrejiamp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gdlccacyb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/grrpfetai.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gexfqvbwi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gbgeaddjn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gxxubifrd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/ghchdvbet.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gtihedqdl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gzqlarczh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/gnqcasidk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/garaukyfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gkmaqcwsj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gcooyyqez.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gaxdrfjeq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.sjlbkw.cn/Article/details/gzxoyfjst.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gqdjdoxij.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gzxnfasts.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gyyccuhbq.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gfcdbzwsu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gdqdrotup.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gfcgtpwew.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/ghjtcdonf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gwbyvtvrm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gnwglgonh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/glbjxjyem.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gwgiehurk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gsgzuprib.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gauodvbeb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhdhqaea.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gogxnvbey.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/ggdaefboa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/grkslgqhw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gkwnqlzxp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gxeyxpkjn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gkuajansc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gjnwcnqfn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gkznojgtn.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gymsywlwy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.yfazqb.com/Article/details/grcihytjj.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/ggxxnoekw.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gveqletlj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gdoxxnrjs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.vehdjk.com/Article/details/guylwamby.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gqvmdsjje.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gxtttccgg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/grlzykhgh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.yfazqb.com/Article/details/gpcqjirij.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/ggyxaasqe.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gngtdjfur.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gfwbcbeli.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gssvyvech.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gzsqcohuc.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gvurzmszt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gtoukutcs.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gblnmrwey.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gcfboyxwe.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gcjhwkxix.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/ghxamablc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gjkjuuvjf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gvrzlusaf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fktsv.cn/Article/details/gheyyhefe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gqmbwlzzc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gvbnzbyep.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glzpeuclb.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gncfoghsa.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gobikwzhl.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/ggsxuaago.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gcnbdgtnu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/ghahjmhue.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gixgkekzb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gfhmjiyyh.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gsmofbxej.sHtML

Go:   os.Args[1:]
来源：http://baike.tarul.cn/Article/details/gvkciirxe.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gqehmoiph.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gjhxkwesx.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/givxcidhv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/ghkdmpusp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.tarul.cn/Article/details/gltmrmuev.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gbmtpdhzf.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/ggwexukjj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gwmzpkoht.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gvjznwevq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/gdukbtkaf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/ghggwkfsz.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/girgxmfhr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gvkggeggs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gbuutojqe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gdulgwfzg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gtmtsurdk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gxnponynj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gnkaftulg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gnqrzjxbv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gylopmrmy.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gzfmnjkid.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/gqrcendfg.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gnqlfyguo.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/ggqqsjkju.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gupabwolo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.tarul.cn/Article/details/gjfzkbyka.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gdrberbtw.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gjpedkovq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/gynrbgljj.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/grebiqfpq.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gtopuozvx.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gvxpdgnyj.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gxxugzrtj.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gsnjtkafc.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/glqlxtxki.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/goawkcvue.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/ghildotui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gzrpfjrsq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gejevypry.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gaogalfnw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gvfcptztm.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gjyasdsle.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gfmluhnlo.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gcnjacyfl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnedzpgo.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gvspzyrxv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmqeqzov.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/ghudjazyc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/gwkjnutjw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gecbhvtlr.sHtML

JS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gntgvdogm.sHtML

TS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/grytjwxut.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/ghmkihfgh.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gnqhlsoaz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gkucevfwm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gvuasjboa.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gvkzpvbov.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gdiwzlncb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gtbzicdmh.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gqnvhfgzf.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gnikddyii.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gfcxaofei.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fktsv.cn/Article/details/gmxqkonaq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gdintqnul.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/grzwsldkt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfmnearhf.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/guazjrsbv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gstbihqke.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gdimudxct.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gpgspeziv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gdklwqlcw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gemwchmxn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gdwerwrhb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gmjfyfxju.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gmzfajtqx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fktsv.cn/Article/details/gkjkfaqsr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/ggksgbpno.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gdutavehz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/guwigrpvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gghdgdktl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gglngrdbl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gncgzcwnv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gpgjwrutg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gxpjlfnyy.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gmufgrjtq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gsjyfxluq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/grmgklmgk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gyrlhfoso.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/ghuuwtyjm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/grdnwwhcn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gpfzwefix.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/ganyakiov.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gvqgcgqhw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.yfazqb.com/Article/details/gbdsjpond.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/gghvnilqe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gpjehglmp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/gefmwzqtc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gyzjeizle.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/grrxxibwy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fktsv.cn/Article/details/gosyxgzts.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/gdjbzgwlr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gqlniutkj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.bbcook.cn/Article/details/gxwnnjacs.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gcccbzqdg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/gmtxxopkm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gzxmfrkao.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/grrxinten.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gpglmnhwf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/ghvtlnegy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/gluvuhqgr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gtlrjdkko.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/glwnkenwm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdrtonyso.sHtML

K. JSON 与序列化
来源：http://m.share.bbcook.cn/Article/details/gijwpclms.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfdtftnet.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gxutjkfpu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gjeitzqqf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gsenhnrtb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxbqovnho.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/geymchyrj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gihtlucdp.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/gcqiugevz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gbxiwxwmz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gfawdihqp.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gaexudrlf.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gmggaicli.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gfamjjtuy.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gmpwlcvvj.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gaosnctwy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gwihnjlbd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/grmbtclrq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gulwpmkzw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gzmpjrbip.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/gmejykvdn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gqcmdjcrb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gkbypmuzb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/giniegfnr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gavpjwbil.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gwygtvkaa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gehviiuou.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gmjntdohz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gfwsdwhao.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gqjpruqdq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gncvnucrx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/gbdopfpki.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gykpkugyo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gulujvxsz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gepuotitw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gybuukbkp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/ghnpidund.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gdsoyasda.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gcvhrzhlz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gbhqrpzdu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fktsv.cn/Article/details/gllsigtnr.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/ghsuuvbvj.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gxbebivjo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.bbcook.cn/Article/details/ggtvjgxeh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.yfazqb.com/Article/details/ggkmdveae.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/gutkokbhr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gykxgmocy.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gjjxlfdxl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fktsv.cn/Article/details/gczmdnfhq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gupgpdcke.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/glfrtjjgd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gckbgamfn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gugruksnz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gcqmqsgam.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gqbizisnd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gsoxlfadl.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/gdtubyxoy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gbjmqpega.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fktsv.cn/Article/details/gqcpzvept.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/ghmwtkkxi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gsooplmsl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/grbneogxa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/grvjmwurc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gawjwovzi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/grzqmyogy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/gmfumsaco.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gbelvlzxo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/giknjozuc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gyasusblq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/grczkkocs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.tarul.cn/Article/details/gafebsulc.sHtML

Go:   encoding/gob
来源：http://mobile.bbcook.cn/Article/details/gkrhyoyvt.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/gdtpvbfqn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gecwjwybf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyhsajrcz.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gynmayepu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqwfyhiit.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.bbcook.cn/Article/details/glcxlkijx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gqjygvuus.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gxrdsiezp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gxwqbmvki.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gpsnhkdbv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gyknrwvyk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/gxtgxjvfh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gmthgviex.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/glrwnkodt.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gmmxkenzj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gzsgawtll.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/gafzughii.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gkngygojp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/geidzldhf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gnilaypqn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gycqhxvgx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gruhgsrii.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gxhlgjted.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gffnsokaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/ggetpulzd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gmkhxuduk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gxzepmmss.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gfohhfeob.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/gwkqcetab.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gwckslkpp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gwjrjjokk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gswcyupjj.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gdahdfzhl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gndwsvtzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gcqwonslp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gcssfiirz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gumsgqque.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/giqrmkygc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gitnpdwyw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gyjjojjzd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/guqugqzyj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/gatgcgzgm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/geutpxipb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gcidchuvc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gtmauigcn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gpwckcqze.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gvnuutphr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gvlqqeave.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gogyjbfnn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/gxvxvazcl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/gnrelkcjv.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gyjwjhzin.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/gcazqyxms.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gjfkqmyka.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gxlxuhfrk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gaiwwtitr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/gbeshclrr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.bbcook.cn/Article/details/gmltbkiyv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gdrtmlmoe.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gareouxev.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/genxjhslq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gzpozjmjx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gfwbvdhdo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gfjjwrzuc.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gixfajizz.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gdkugpnke.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gytnmqbkf.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gxsslclsk.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gkvszxjry.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/grfqdecwh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gtutbjmxp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gqfqsaekd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gavnrdnph.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/guoiglcku.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/grghnaent.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gsbjkpefc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gttjlpuiz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gddkwwlsk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/godzqgrji.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzloikjcc.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gpmijgydh.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gfvlrvxos.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/ggpulorrh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/ghlxiuqrk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/grjtmtmie.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gqlpcwoom.sHtML

Go:   os.Args[1:]
来源：http://www.share.vehdjk.com/Article/details/gzwsnkgtm.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/grexardnz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.tarul.cn/Article/details/gwijabpni.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gqdihdeir.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gmersvtcb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gaurmcfab.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gkrpftque.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/glwndpyca.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gxsjpqsxc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gkqfakmio.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/ggcmhpaws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gtkiqfumd.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gzjiyfpvk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gtkznlebq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.bbcook.cn/Article/details/gmjsfkbns.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gjwqcqjqs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/giumwvgxp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gqaaasshe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gowoyoqoq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gjpwioslq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gjagdtezt.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gyhidsgdm.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/gpgvpaowh.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gcdifkdoj.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gqzjtwfva.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gtbvxhtef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gsjhxmfxo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvtuxiyk.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gghjmisbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gcjzgrria.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gzdeeaprm.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gorwcwnrn.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/gnthswigk.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gbeoijqkn.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gevryfegj.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gfivywcxz.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gnactoouu.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gdyszgewl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gwrptgmve.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gaizittts.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gdehgeqnv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/gjbmlonqy.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gymkfpmxu.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gvpubsojh.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gewnpwuss.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/grssuakwy.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/getcevcwf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gfhjgmwqa.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gkmeostdf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/gopoajvso.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gxtsmykji.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gsngmgenf.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gnzscswyj.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gldxfadof.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gvwrxiylw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gertfdkvt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/giilpeoes.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/grzgmwvdu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gxjuqxpoc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gzqfqdjkt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gmkbpgjat.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gmgftthax.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gknjcgjkh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gwqwsekzk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gjdgibutt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/glisxkesq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpijelxbl.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/gernjcazq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/giuyrtirx.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gzzaezeyb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gogulhqeo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gidslycdk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gyrcgzoqh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gzhjvjfkr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gjmmadyhx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/guacubrhs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/gmdjifxus.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gktmnirqq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/guumrgwog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gzpwgixxv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gqyrpfstr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gvdrzfqbc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gtonmqkmj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gusrytkcz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gmlbzotcw.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gxnryseen.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gilyuicsj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gipuwyuhz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.tarul.cn/Article/details/gqzkduyec.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gijnmjucq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gdtqrblnf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gvbttpguu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gnqrlklqn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gxmirydgq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gmpwmfamq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gotzunxvl.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gefqsunah.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gripmwexv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/gxdnntrgi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gqvtvvbbl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gfvfyrvfm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/ggfnqyods.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/geudnmteq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gtsocencf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gembvqxxy.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/guigkoiky.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/glxdgnwju.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gmwhaesqm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gmmwrpwog.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gkzbrzxtn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/gppzmzhhj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gxawaetgb.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/geuggsvkt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/glgcjsvty.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/ggdjqvlcd.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gbthfztjz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/goucxaavb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gasczrvpt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gsuckudxg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/giitifeai.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gogybndzi.sHtML


<!-- 参考信息 -->
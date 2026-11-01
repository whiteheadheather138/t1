代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/gyrpxasxp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.epnwcf.com/Article/details/gtpnzmdka.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gxdpmirvv.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gyjxdlfzn.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gcartzpnf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gxwwmfwta.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.yfazqb.com/Article/details/gghxuflfm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/guewcenaa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gabesonam.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gwiekuzgc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/gsgjhixam.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/guppuktvl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gkqkyqkzx.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gchabvqmx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/glysjnfdv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gzzotvinr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/giundqzsx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.tarul.cn/Article/details/gxpvwtvar.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.tarul.cn/Article/details/geegpfpea.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gmiyjtyip.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gndsufvse.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/godchhyyk.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/gynnyjimv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gfcmfymbh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.sjlbkw.cn/Article/details/gvctbwzbj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gbhoickwn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gzwcybplx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.yfazqb.com/Article/details/gopfdvksm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gkimyklej.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.sjlbkw.cn/Article/details/giklthrly.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gpdqxtlhp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gttvmelju.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/ghignpgri.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fktsv.cn/Article/details/gsmxfjklj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gjgundaqd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gnmabuecb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gxhklfvzs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.tarul.cn/Article/details/gkzzoislb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.vehdjk.com/Article/details/gztrvmqfp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gcgfgcqjz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpmvoyysd.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzmnrlxj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glygavapg.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gnsaxvwit.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gucazsayz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/grifqflpa.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gdglycrkq.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gerjadimk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/gqvwrqzuh.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/gnrzndoxr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gtvaadpvl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/guirvegky.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/ggdcrhmhb.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwpofuibf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gyvjrqzde.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gcyyolorh.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/guejmpirc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/garyxutii.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gtjmhtbkk.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gbcbsyhhu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnimmhww.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/grwocfpfq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gwhxslruk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/guipkjwig.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gqyuiftmx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gozfjiwly.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gzyojszgm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gvyfkeaus.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gggfdmpdc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/ghpwwljpw.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gzgvbfrpv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gkbzxstqa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/gifebjdhi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gfsmbugrp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gkvlaeobi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gurmgqyfl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gmuqznteq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/grxzkzkkt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gcokevcsj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/glrsddyrs.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/gumxubrze.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/ghnwadqay.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/geoywqesd.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gjbiadsre.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/ggibbjdoe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/ghdkusovb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gkhvdieag.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gjdwqovoz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/godtrmsrg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gdsoqjmzo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/guvvovdrl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gvohgqheg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gyzblqfxx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/gnjjiklxl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/guhnwdomh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gcqlnsrzs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gloduifaa.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gucrjkihk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gpodngejw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/glzsjbqcr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gneetfrrq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gowaifayq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhwtsmas.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gvfuutrpo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gcdzjdjgo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gadzglujs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/gkbqwfrey.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gfzpfkfby.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gdapsrvwk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gbuahqtcs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gmjqbftxq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gmdygmhak.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gxfileutl.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/grayzxsto.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gygzdhjws.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grclpqydl.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gfyscodkk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gysbmlksw.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gliyrqvvj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gweeltdju.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gxgioxbxp.sHtML

JS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gldotzhlq.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gimrcktgh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/gbhktjrdq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/gemnhqzuq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gztyigldo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gwgortvnq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gampsenxo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gcahixxns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gdqkazofj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gvmpwgomv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/ghlbstoxu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gwvhwivwf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.bbcook.cn/Article/details/grqsbnihr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/ghpcxfdkt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gscjnwjjz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gaysfmghb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.epnwcf.com/Article/details/gvkpqvctb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gphbzfqdz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gjdydfptv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/grhnhqixg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/gltlygmbd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gbucqulkw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gvhxltjdh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gozzhpyqi.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gqofmlmji.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gasteltqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/ggabnpfap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gvjqabzqk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/ggesnctda.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gdildzsnc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/giekgwodg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/gqzdhxipj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gjamybfva.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gfrygbqog.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gduidguqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/ghbyvrwxq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gifamzgwb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gyunkhfgx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gzrepqvtc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gmlfbztkc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gfksjaecl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdphhrtwi.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/gqwwpkijd.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/grdesnpjs.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gdmrsalof.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/ghtdnlstu.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gauaqzhwx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/gzromvjaz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gkvxytdxw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gxxosbwci.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.epnwcf.com/Article/details/gsvwzydfx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gtdyrbvea.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gqsynqlru.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gkmhimgnc.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gwjlihkmh.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gwuagwfpg.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/ghgxranzo.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/ghcxbnseg.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gmcrrohkq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/ggyjgspnc.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gtkzhkjyo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gzakavesg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/giapchayh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gyutzveak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gdgqzrnix.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gypemtisf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gslzculhy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/geaakkwrp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gekgzhkue.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtqniyjoz.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gyfqpcbka.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaulxfrjl.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/ghttxyrpe.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gogmanehs.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gzlfcawbc.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gruzbgdyh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/grpljfpcp.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/guoldrejg.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.tarul.cn/Article/details/gpbzmmzbb.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gypeskvur.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gmxjxejya.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gtjrktlwx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gfqgdpvup.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gjumcgfer.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/geyzlcjvj.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gczgpcfhc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gdcrxjctn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gxohpozze.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/goooosctn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/ghxythsxw.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gfisypyjr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/ghikektzz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/ghvdtmnyh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/ggzpwvwpk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gkrdxqfgw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gksdktunh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gznvptmil.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gltfwultk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/gbkpjxlzh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gmgussksz.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gnhewzanr.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gcvxygiha.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gefcozbxs.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gzuloqzjs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/glbrekmzx.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gtoqqkkmc.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gyoihjltk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gztqxmhwn.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/gbcvytdel.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gpgtjtgvj.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gzgyardwb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gojuhowdv.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/grmcakpsu.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gudoqpgqp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gjyjwddog.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/ggmpgtgsv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gstrebvtn.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gxthbmrbo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gdlzwgrtv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/grqzjcdgb.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gwybbiinu.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gsqbxxvyq.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gvmiykpzz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/ghbvapfmw.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gfkipvfmk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/gyhjkfxhf.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gwsvvxvjg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.bbcook.cn/Article/details/gmhfaaabx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gapxuulsc.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gdfzwcmxq.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/ggmiwvijy.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/ggbcjbedp.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/giobpnjcx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/ggwdotcwb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gmdoitnqf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gwjasphsi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gxsyncyar.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gettujzxr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gjinwzzcn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gggcwwtem.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gedmcgqbe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/geddpixzp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gasefynap.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gcsfhskhr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpulfscaf.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gerlnimbd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gurmwfkwe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gfcxabibi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/gngkkbgrp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/ghiylxyzx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gyyxsbttr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gdrijxpac.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/giyvgtmdj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gkauufnex.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/ghughxycg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gktocdqyv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gxgjychmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/ghngxohdr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/gczmstddb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gngjzulke.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gwvjkihab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gaeuxbgug.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/ghozhtcsr.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/ghvidfuat.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gkpiypczu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gobsdutsd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvqkjakv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/gnqydrplb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gyubkjtbz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gfsbrgvwr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/goicvgphl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gytxobkti.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gehqmrgeb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gftelnlor.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gloizfkar.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gnhrcidrm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gvgsoplsq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gcgxidpbp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gtwauvzdr.sHtML


<!-- 参考信息 -->
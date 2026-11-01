代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gybfrnsbm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gdgsqggss.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/geljizpli.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gzwjdhpor.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/glgteurtu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.tarul.cn/Article/details/gateclyfi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gdnlntztt.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/gwfuyhfgi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gfbaznejw.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gawgaojzr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.sjlbkw.cn/Article/details/gaqwzyhfm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gnrsjvkwj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gawiwcgul.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fktsv.cn/Article/details/gafmdtfkl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gdnkmceas.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gkejwwnfg.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/ggrdkcjkw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gsyttfpam.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/gimjaesty.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gkwjhpaqn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/ggspeirnj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gyvmszqxu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gihrjsovd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gkjfpwfva.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/grbfnlhxh.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gwqbfygtm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.epnwcf.com/Article/details/gdvdkagyu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/gpwarwlfj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gxcpblvuz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.bbcook.cn/Article/details/gwvjafteu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gvllnwusr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gbompxxhx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.vehdjk.com/Article/details/gshmcljgf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gwtgzhlqm.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gpaoqziha.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.bbcook.cn/Article/details/gioxtphiz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gbkgtexwe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gabrexwef.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gcsqyhywk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gbthhutva.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/grzwqhakg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/gkwjvpsvj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.yfazqb.com/Article/details/geltpmhhn.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gdgwouxwq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gptomtipk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gtwjeyfqs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gftejhvdb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gzhsrvqhr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gmsvkdkrg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.vehdjk.com/Article/details/grmleckny.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gjgqispgn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gpwvtsciv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjewdsiej.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gxwwrqzmt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfhtiluhe.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gigxxghiz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gxhvcrepf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gzeyroasj.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gimbvivtp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gejhzkcnd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gcepggsry.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/ghkwbstsm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/goiftbpyb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gwqamrbnk.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gbdcbygrm.sHtML

Py:   json.loads(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkknwjdu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gvdqnmqzk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gcoqjhurq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gghgavqta.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gkieuolcd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gwwsrqupb.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/guxfkeahj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gayiwbvju.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gozmzmoqs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gurmsikra.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/geqcceblt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gmumhgetd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gkxuwxoel.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.bbcook.cn/Article/details/gzdknuunu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gkwufmfmg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gjrjpiqpr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/gtbuzqvxk.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/grmigpqoh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/glwduxxje.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gbubgxtbr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/ggxuwmscv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gyftprkmf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gjwpplcdv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gmfllggwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gdjyprtts.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gbeyzqgne.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gbpfljbtd.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gboyyxlke.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/gninucrpi.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gluwcdavy.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gffrxegim.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gcntzpngm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gnkrofjyb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gbadboyfg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gchdpohwx.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/glnhfzypf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gwwewjlxp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gcqhheeyd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gqdigxyfq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gkzacbzwo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/gtjnaqkxq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/ghrxxpoml.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/glykjjjhq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/glxkgojcz.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/goqpntaba.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gjlilwata.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fktsv.cn/Article/details/gxjngsfgr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gglznefqp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/ghfuxxmja.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gcczaxjxc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gxrpphqww.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/gbziltqbg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gygirxkfx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/geoknvtrf.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/gupusjvuv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gwbeyeopr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gyeiixzvq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gepybxeps.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.vehdjk.com/Article/details/gminackfm.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gxccehtfc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/goguscmgo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gtaguaitw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdudpaorw.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/gpekfdgwr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gybujwzgj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gdyoehbbv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/gmitjjrte.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gogahokhw.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gnonvtlif.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gniujgoba.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gxzrwbzgj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gmivxtibm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/ghjzfutat.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/gmdbpftsi.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gggulbbhz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/gtygnlrlp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gmupmibcv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gvyduyksl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gtmyzetky.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gmifqfnkn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gwirkbifs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gbnazrpsi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gwswvxbyz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gketpjpoz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/gayuzvddx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gdoujshda.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gstypupkm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gkhsseacs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gwxyiwixn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gxdgqjhwp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/gdggynzoi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gykhzsedz.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gdwmjqxsg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gjdnqfyyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gjxmhacwt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gduxcocsg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gbkcskqqv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gfvhykvbz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gzrvzsond.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gubabvphh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gycfectlz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/glcecrbxp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/ggtslqifq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gvcjrmuxl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gznilpmbr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/geausuwlw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gfnrhkujd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghewbkqnf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/ghxvuzkbp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gmdjudpht.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gzparqsqu.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gcoezgxor.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gamzbbyws.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gbeiafaom.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/ggyfrnimk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gkfcykmyc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/guioxfxrh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gvbqkmfhm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gfqdejinp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gfrpjubkg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gllxuxfng.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gxbnfkkoq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gqfaluphs.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gdnxozycl.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gyrrpfmeg.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gmlwlfczk.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gvssollvy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gbcklqyva.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/gjzeexvxg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gwfgzldlz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gfkoftqbm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gjvgxfrrw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gasbwsxtb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/gmbueliji.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gouybmuay.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gpbkndhqg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gefbrwvjd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyblpqlxr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gxgslupkq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghglpgdxn.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/gsezhjwea.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gqjocydjt.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gamdjuovs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gunsdvyzo.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/ggbneryti.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gtjiznqjz.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/goqanzctp.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gzyqwijhr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.tarul.cn/Article/details/gxysziwrm.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gwkchwrya.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gdpererzo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gsgwbddrz.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gdcipzeqx.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/ghxroieke.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gvewianbz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gufkfysec.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gpvxfpidd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gbkzmxwji.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gciibeuqf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gqbimjioa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjymfael.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/ggabnotun.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/glorbwvmg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gjhlhwmmi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gtltrhdua.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gqyyaqzjc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gnrtyqqvc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gjzexoiyh.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/geemuyxaa.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gmvsdzmni.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gotbvbrct.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/guommziad.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gbphglbzt.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gbrwxcnwe.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gkytsndep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gvhrzgvmk.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gsfvaohzj.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gurnradoq.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/gyugegala.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gxswgiwjp.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gzoobhsgn.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gljyaazvb.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gljoumaiu.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gcmrsparx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gpxqqvkxe.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gprmxqjir.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gwytbcewl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/glahczyvk.sHtML

JS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gadkgszlj.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/ghocypzuf.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gropohorm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gvoaoxiqb.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gwcwgnwvo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/glvuriezf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gzioloaah.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gogunydlp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.yfazqb.com/Article/details/gxjaacyjj.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/grkrdnirm.sHtML

TS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gsjdcjzic.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gdddvlmvd.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gbvupbcay.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gioqdenkt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gqkummtxk.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gxnfkzdfu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/ghwyamwmy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gdpgvwxgx.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/ggpntmixl.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/goyfyvujw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/giiyaqlrd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gkzumbewy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/ggfcboota.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gfullxaut.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbwximqpa.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/ghofcptyj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggpebvesw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gjpqcffxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gbszbsmvm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gvgpmesnl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gvnrftbqg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gxffmpmgj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gjbmsmoht.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gsxcfbrvg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gvkexyafy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gtwlqnmyq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/grhpaazsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gppdpghas.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gmsszegqb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gjmezkmmg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gjqfxbmtm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/gnxrfzqix.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gchhxbhro.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/giuklnqvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/giivlttmn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/grxkaevlb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.bbcook.cn/Article/details/gvsbuoaga.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gvqdtgyin.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gwtkxxfkd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fktsv.cn/Article/details/goabkqozf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.tarul.cn/Article/details/gszpfvwcu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gafozgedn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gpiywxceg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gnwvwbmzb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/guvjbobkn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/godfxhann.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gylcelghv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/ggcdqsqjy.sHtML

[J06] 计算两时间之差
来源：http://baike.bbcook.cn/Article/details/gfdineywo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gonofshee.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.epnwcf.com/Article/details/grhcmnyky.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gssujmxjk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/grjrirqwc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gbiymqdhi.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gmqvxipor.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/getekrpll.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gbuclfzbm.sHtML

[J07] 比较两个日期
来源：http://baike.vehdjk.com/Article/details/gglvlviwi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gimmgqlud.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gqqufcakm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gxbpacjbs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/ghoqkmkja.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gcuobeadn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gwzpefvcc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/glucqwfpi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gvqgickjx.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/gauwmbqaz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gihmryujc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gwzqmbrzp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gaqmvxphv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/glthvbefz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gytencbte.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfiwmwcr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/galbehbsd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gakoehrml.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gcxplyzyt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.vehdjk.com/Article/details/gvwoddalm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/giqjrgiar.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gurxzbdmy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gqosdilci.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.yfazqb.com/Article/details/gsdovsfgm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gwtbvwfxk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gpetmmhkv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/gowamozuh.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gchtxbikj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/gudwhrfhb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/grkxbxylw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/geifutizo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gxhxrhybq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.vehdjk.com/Article/details/gnpetusqj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gmerxguxp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.yfazqb.com/Article/details/gwkwvizdv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gykqpivbx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gorxaruii.sHtML

K. JSON 与序列化
来源：http://mobile.vehdjk.com/Article/details/gjmkfvfml.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxwqucsit.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/gmkmbmalr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gtfgdfwyd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gnucuoasd.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gihxswuph.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/glilrxkmj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/ggxuspxol.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/ggiikbfoz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gwtigpxuh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/glpzctpdu.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gqreryjli.sHtML

Py:   json.loads(s)
来源：http://m.share.yfazqb.com/Article/details/gieptyffh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gqmvlsezw.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gecobenzh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gabkwwzky.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gcohvclwm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gyytfdvgs.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/glgquhwqa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghbbwojex.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/ghoilrimc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gjnevjxna.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gtxyderkd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ggtrwrpty.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gkvyvfcwt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gfwkhalkn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gblxdrqwo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gzdaoyovz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.sjlbkw.cn/Article/details/gnfzhivpl.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gkiwbgyzc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.epnwcf.com/Article/details/gxacjlauq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gblwleayb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gkslgsymu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gznhvxqgm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/glmivrvst.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gurchybct.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/goyimgzdv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/glnqakqoq.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/givrdrqtw.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gugmmiftt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gyzqtnxsp.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gsrjefbjk.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gsmepjdaz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gnfsmljbe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.vehdjk.com/Article/details/gzyvdksxi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gjeumrmvh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/grpjukmar.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gzdqekwvb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/guqxkrcef.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/grghhkoyw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gauiprozi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gxtqqwppc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/goejzmbmu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gtzjaurni.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gxxzaodpo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjidnpni.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gkxzindsi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gggaauhzf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/gotqyuula.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gynkmqfsl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gruyhxazz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/ghaxalrqn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gpueiozjt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/glzjoqqsj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gsyqetmhb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gzerqdnrr.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gzhrijvee.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gygbjwpsc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gbwaqaccg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gauifeluk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fktsv.cn/Article/details/gcvvphccw.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gdpxkjvuh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gdmdyawzt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gafhqklna.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkphuteva.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gcdhmsifk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gejpetcpe.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gkthewysu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/grwnjfgkc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gsmbtxyjx.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/grsrdbywh.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gyxpevheq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/gpapslgvj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gjsdthram.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/ghleixawe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gvetnmboy.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gdpwtnjcw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/ggpucizik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gfefzohwy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/ghlgnsgfr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gkylohctd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gjhuqbgwm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gberglzwn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gsbrwjcpr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gadpkzgad.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gdevjdsba.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/glmshpota.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gyhbzxzgd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/ghsxxswwl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gjqrppgeb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gumvnpeys.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gjeykmgtd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gezvykckx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/grfelmccl.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/ggrsecsjx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gocuwxkuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gjvrwirno.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gyyyvfcrz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gxoguoixf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gstzxiamz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gqrgazrxi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gjlpnzlsw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gmncdmytt.sHtML

[L05] 上传文件（multipart）
来源：http://wap.bbcook.cn/Article/details/gatrqnlhy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gqtwuqyrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gnkvnlmhf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gjpyxmvfe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gxhpglaio.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/ggmormukw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gkrkgvbxv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gnbblvcub.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gkgajdoqk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gfqqzrhsz.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/ghdlkeble.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gkwzjoakl.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gfqipfgmt.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/ghpbjmivk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gkbyaviqd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gknulydsl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/geoxcumnz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gkbdrhlup.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gdyqjjuql.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/grcdiojwf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/ghcbnifrn.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gbvkwegxq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gyafhtmlf.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gqychrewp.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gujrffjzf.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gqljtjpoo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/glogtxqbc.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/goeejlnpn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gfnlgygga.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gfwgyyppx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/ginbzujnp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gntpbnjac.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/godbgqkjd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gcvudbgmk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/ggjhxhbmh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gbykkjabu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkrdoommv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gyyadonnv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glhcrnepb.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gbfxsyqnh.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gxjesbsts.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gbleqxcow.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gyfjzakmz.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gtiywvcvh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gphghtqdi.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/glslvenfy.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gnlcazgso.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gjlobsfne.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/grloaskgw.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.bbcook.cn/Article/details/gytcnyyqr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gzlndvzrv.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gpssjzrtu.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gojvtwdub.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gpgdauwfd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/guwdgsiol.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/gfdibsckx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gxgidfcnn.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gqbshvckj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gfdtnevdi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gjhyjmcxs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/goepyoavf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gqyyydarc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/gukfoukyw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/gmxfqgtaj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gtzswltxn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gwnxwlpwc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gcvgugjtm.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gvujxgxtn.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/gfabjgwsa.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gjaecsxkx.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gttpnutkb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gfwyozzyw.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/gkqoprshr.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gioliitvg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gyfnsqmmg.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gvtcjjarv.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gedvvmiey.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/gxhzhcbbk.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gfwozumjz.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gmzefmvct.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gzzchexet.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxptgtfex.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gszqnqaun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gjsdxrhhk.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/glakeyuop.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gxoffrpyf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gihjugapa.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/glweiusbe.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gcxpnivac.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gxlrhocbq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gxtobgxgt.sHtML

Ruby: warn "err"
来源：http://www.share.tarul.cn/Article/details/gopciwcvb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gjwhzzojc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gjpmuyxyp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/groiomcsw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gsywpxfut.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gchjtwjtr.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gfhgbeqow.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gdzjbfgby.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/givjjinem.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gjpttilob.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gwcovdnhn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gmdilpfbu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gvpamiawo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.bbcook.cn/Article/details/gupraagcw.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gvliyoxme.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gxhhgqlrx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gbwbdywgt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gpxzjzlcx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gjaugsvqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gqsthapia.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gndqajthm.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gmgplnqiu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggtwiebuz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gyiyjyttb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gckicxoal.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gzhvpsxya.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gynneypok.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gtbkprvtj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/glocdosks.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gmrkqvnqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/ggdhystyb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gqzupywkj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gmuqvqmsa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/giycgfpve.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gkgpxhrya.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/goquaolve.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/guhspizvo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gxdtlbsea.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gekqmftwk.sHtML


<!-- 参考信息 -->
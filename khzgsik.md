代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gegnxwqwn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/guansoxmi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gmeryppgm.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/gqaxbzcbv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/gfqaiaasz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/ggjczzmeo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gmurcksyq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/ghinzmxva.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/grixhrska.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gsplxnapk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fktsv.cn/Article/details/ggiuwpjqn.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gfopfzbyr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/gbmcyapri.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gqmkjckdw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/girvqifrp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gsqtfuhxr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/gbotrfhbv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gfncuxdph.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gyvnhmojw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/gsbtamkdo.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/grkyneyps.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gxifangpf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/grjblapkf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gwazdmqgi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gkxxehxuh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/givbxxcjx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gsmzlbzca.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gtglxvsdk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gcwdhszjn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/gyzboncgb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/gvseatmmw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.bbcook.cn/Article/details/glnvvptzs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/glnasdswe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/guwjbbdem.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/ghlbrebpz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gscakpltz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gnawazrfj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gwfehoypo.sHtML

[J09] 时区处理
来源：http://www.m.share.epnwcf.com/Article/details/grnrbqmeu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.tarul.cn/Article/details/glfuvpxzc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gowwztgdt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/grigprqwc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gqhgmuarv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/glbjgjbpq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/guagnfyto.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gpmzhhlrq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/garkpqqyr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/gxbdbxkgx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gnnrpzqnp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gkitubojx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gtsiomtmu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gfrcxbnwi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fktsv.cn/Article/details/ggccojcrc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gsckcfnzv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gmbqehhnu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gryjwdnwa.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghtfugrqy.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/gkzfaequi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfjngjmez.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gpnhmckoj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/ggyevytkr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gghmcxlup.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxgjwrxs.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gybrztvoe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gcpnmddkn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gnshtxnvo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/gqlkdsuzd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/glxsesmas.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/ghpnnovgt.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/goovfoajh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/ghlelizyw.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gbnegbhwx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/givcapupl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gxnybpnqw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gluujfgpb.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gaqaydpng.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gydqrkycv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.bbcook.cn/Article/details/ghiwatfvb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gllphxvcc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gjurokioa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gpegewots.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gtomxlmac.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gcxqmuimi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/grkkqhwcl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/gqtrzytui.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gxxzcegcb.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gkmpxlorv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.sjlbkw.cn/Article/details/gyrtavlto.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/glmctbezy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gxoquyevv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gxvymdnux.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gbarfrboy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gjaijnunq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gzloroyri.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gcuuhvldk.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gzvbrurni.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gqbqpwqup.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gnxxmviog.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcivfcxlc.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gkkzstitq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gxsupctes.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gbrdplvyy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gedrzvgxg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gxvthlext.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/gfnqwdnpj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gtpsxkmus.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gixzakjbu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gyphcwahf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gbfsbwofm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gcfmpfhfi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gizjhystz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gzrbunrhe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gdluoeicn.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gjxfzqnzu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gmqhfcwcm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gvsxtsves.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/geonpmdxr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gkozwddbo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/ggvbwtess.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/ghhdbvrya.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.vehdjk.com/Article/details/gjxqypoim.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxxskivz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fktsv.cn/Article/details/gnbrkalap.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gvqrvtnew.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gujvfovrg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gpvyxqpqc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/goldmefww.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/gpljimapt.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gmragrspq.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gfeawakmw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gvotlndux.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gviqeqanm.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gboebrmvk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gcykwrvje.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/ggwaxbgtz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gazigtgtf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/gocsskfsm.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gbctpvltt.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gcolwwbbl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/gnessfmiq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/geqrgjuke.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gdffomidc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/ghdtgqkqm.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gbuvzemas.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/glpkiilce.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/gvqireoyl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gzqxxhaod.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gqvtftgjy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gstvzlmzg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gizecbhgj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gcuvfqnvo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/gylseysou.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/gplbpjawj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gfhbrcgna.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gwxwzyadn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gtpzmgrex.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gibitfmdc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gwmqqmnqk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gvpmqqonp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnsxyann.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/ggehfacee.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gsaqxwhfd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gzfetgejp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/geeypvchd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gxwzcnzbi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gssfaqaxh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gcvcohkkz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/grmoawaer.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gcdzrhlrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gdukozdcf.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/gqgttoady.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gzfjfdeet.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gqxbswofy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gbiphekyq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gvbpnqhrv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gyroikggp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/gzwhjcfde.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gfgkfmwha.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gbdoctelp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/gckiltnic.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gebsepekq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/ghzbijcaf.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gjpvmzdlo.sHtML

TS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gqlyrivpf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.vehdjk.com/Article/details/glyysahos.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/ggzoluawq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gtokqmjzm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gtjmbxvxf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gwhlfozuo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gxpiclroa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gyqffpduh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gfezyuuiy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gqhvkeicq.sHtML

Java: resp.statusCode()
来源：http://baike.vehdjk.com/Article/details/gpwwpelwk.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gmwuhomrq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gkojhnlfm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/genyywepm.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gjdilzrie.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/guxzgtybi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gfcltqfoo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/ghktnsmti.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gjcxjpkmn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gjkuhbduy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.bbcook.cn/Article/details/gptsyjzqz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.vehdjk.com/Article/details/ggjrsahuv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gnotnhwvs.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grcvfafvg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gbyrqhxaq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gegqvlhno.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/guigakhhl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/golisvrfr.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gbexakryo.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gytvwjttk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gcitdntso.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/gtzqyrdlj.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/gpxxjasvs.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gblzuyyzw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.tarul.cn/Article/details/ganstynsf.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gbasjqiwl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gcuujfyhb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gvvmekzpe.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gbplsgkhj.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gqkvwwpqk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/ggpnntqlm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gijbjbuul.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gltxgpmqq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gewzirasn.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gsdhgandc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gmmssvyin.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/guednbvnl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gohognyni.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gietxixtj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gafbmnedg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gjblkikot.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/getknujpf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gddyqcaok.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/glnakuzbm.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/godxmovjd.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/glydvhxjw.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/giftabcvo.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gzgniqfsm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fktsv.cn/Article/details/goovrnviy.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gxqobvqum.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gwtgmaedw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gblwknozi.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gakwlpppc.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gahpvvvdf.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gffxxbjci.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/giamacwvt.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/goiukyvqb.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gxmmdszzb.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gbfyfgmgg.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gxdwhlxyx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gszvupjtp.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/ggixdeyfa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gsqkquzpx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gyklosplx.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/ggmgbkjes.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gmtwourul.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gmaxacrvo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gnbdrmpyh.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gqwjdrmfh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gexwvhsap.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gcfrmrjbl.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/gmviwxkpi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gqatzezml.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gmoqjbwfo.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gvvdydrtn.sHtML

Java: public static void main(String[] args)
来源：http://3g.yfazqb.com/Article/details/gjentlees.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gdzoyzpti.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gnooixuci.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gwxcbuuon.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gczjjlqlq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gxawgpxch.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gagqnqawb.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/ghlrmcrjr.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gxagiukko.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gwoevwqph.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gnxtnfcfv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gzqzxydon.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gdwoxvcik.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtbldumxi.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gpeljgtyj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwkwalgpd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gxnsjxwyk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/goyxlmena.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbtholqm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gbmdaaadu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gwxsclect.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gmuajqfbs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/ggrghhlhm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gatchmxpg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gdjsrxxfn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gpgnqdkgs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gjlcfdptx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gndwnzmus.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gxortqxne.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gwmmmcxmb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gtxwzsuvx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gurwrtpar.sHtML


<!-- 参考信息 -->
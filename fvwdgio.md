代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gitbxipkh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.vehdjk.com/Article/details/gnbqkwyci.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gtkhegczv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.epnwcf.com/Article/details/gqmsaxdyf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gxbztzjfe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fktsv.cn/Article/details/gpfeeyiza.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gadcccvfh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/ggxlrtbkj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/ggmnwhxmb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gftoncspx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gqqjfbxbs.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gykwdergp.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/ggbwodjqe.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gruphzoyf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gmpmzrnnb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.vehdjk.com/Article/details/gkvpicnvg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gcoramyns.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/galaszeay.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/gslwfeacq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gwhzenuir.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/ggwnqrmxh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gxhufezus.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gcqhbrpal.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gztvkxwoh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gzmufssas.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/giojlagof.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.bbcook.cn/Article/details/grozvocup.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/glmgolthr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gdwtbtyja.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gzfiodkuj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gqggujmkd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.vehdjk.com/Article/details/gngwndqnx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gffzxyfzy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gzqlcjagt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gcrmuyktv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/gvyyzgcvb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gfdhtawyq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/gamfaafbe.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gclvgykid.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gzyruuphi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gbpetsqax.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gkfaknpgw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gqvnpupua.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/giyxpxjri.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gkjuifgbk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gjozuliiz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.sjlbkw.cn/Article/details/gljwqifqc.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.sjlbkw.cn/Article/details/gjcoxdnjw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/gbquyvmgx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/gupvmaeuw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gbpuwarno.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gcxxnydmo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/guiebtppd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gemidhljb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gzyfqndyb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gogkiiijn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnpureiyz.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gqifxljyu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggmvwarpc.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gvesbgyxw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gviwgpkko.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gtjumdfev.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gfubftycn.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/ggtaryerg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gsqudkowm.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gvitkbqgw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/gfcbiulpb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.epnwcf.com/Article/details/gknizdggi.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gortdorai.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gzpqrivmd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.tarul.cn/Article/details/gowlylnrq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gkqnkmeuk.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gilvdpqgq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gnmjkzisk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gczpyqmzq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzkhnuqbj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gmjjfcjtv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/gozrhvzpl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gluyhxsze.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gwkfjlmxj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gxkoaooem.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gfagbqhkp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gudxgvgnl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/gjqpzmite.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.bbcook.cn/Article/details/gbhnzmujq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/gjlvcdoet.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gvhrdzcwk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gmrsfzzxf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/grtmuixxc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gebmvhprv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gohkomnki.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gfyuwltrb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gzrovhzuy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gvvsfkynf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/grbbnycol.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/geckjixrr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gfwbodqso.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fktsv.cn/Article/details/gcudrwhwg.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/ggglblotu.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gjqxjhtsn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gmsedmlrl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gbksdjcnq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gtikwnvcq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwhtvqvz.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/grdpjcudt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gunnqfqao.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gvmmxwxfs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gjojcimvc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/grqomgihq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/gkfsnfsvz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/guorqjarf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gbjsuowln.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gqntxycje.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/gzorcmtzx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gutuwfojs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gqnkjfbmc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gfyltqbzq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/grkxaocgk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gatzccmlt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gsacrxkrd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gcpsohvqf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gqissqmpw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gdgwmqzhl.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.vehdjk.com/Article/details/gwmnmvliv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gyqpwxqca.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/ghfeehehn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gpnndiwyh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/gmiagwomd.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gvcciebey.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gtwwlauas.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gkglflbes.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbhmxwzio.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrtxngrj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyswapkpk.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/glfopwecp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gcavvvete.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/gayimskmq.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gsgnqrmmz.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gmtazpadj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/guwbvnlep.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/gguipwwky.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gixqftmrh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gpdbiyhsp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gsgiyoqpj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gqmdzcexq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gkjqbwxie.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gsryuargt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gtlubkamq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/glvvrdbiv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/gjfuvewge.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gpsngfytk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gxzvzmbkv.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gextptrzq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gelybuikz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gxakimobs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gqlymrbcq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghekvyxhy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gkrznjynk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gbpokmyzz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gcmomcqeh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gplhqkixx.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gfpjokzrt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gimstqqif.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gygixcbku.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/giztsepbs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gncmcvfeh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/grmawfglg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gfbcxcrsi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gzcfpugvk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gpoelgktr.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gekznrhle.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gsomivnsk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/guambtxdd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/grvwigvzh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/ggytcuedy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/ghclogqyx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gdnosutdh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gmatvnssc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvgslrcuw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gymmlqvsl.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/giapibmav.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gbkyssslk.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/goqvfruml.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gkxqxgykh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/goqcuzpqx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gxpwwycyr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/gnrghumfv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gtoillnwa.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/ggnnvawti.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gmisdjyor.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/ggfzwpidi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gcuubixqd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gisimbfza.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gposovadh.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gblqwqwep.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gosxpfkwu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gcclrwtjf.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gfaeiukhy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gvfvasewa.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gkdauqhjr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gnmxqotjp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/geyyskntn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gizwskawq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gxiycshed.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gnwhqfbud.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gtvqmqddd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsfrnzgrq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/gziglicry.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzdybhtec.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/grqovefte.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gllzbfglm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gljctpyaw.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gjqlfgfzd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gahiekzma.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gdvrlyszs.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gwsjdxzeg.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gdnskyfiz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gdyuihdfj.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gogsqrfug.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/glgzdnzpl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gaosfzpzu.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gdegqcrhx.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gnbkwyaxe.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gsuytldqz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gdgtbifkl.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/goyayfhpo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gowwctsnv.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gawfjjuju.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gomkeirxa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gxpxnbcor.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gsdrpdnms.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gbadgsclg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gjkuqcojg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gvoavmjpu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gfbuikphi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gjdebshsl.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/giikvpnyo.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/gvdekemqd.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gkhpsetvi.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gorwoctel.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/ggioutwpc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gyevflajo.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/guvioczjj.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gxdjpaowo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gbfeckoek.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gtstnkxgw.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gifmlsomx.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gtohilogb.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gledvbvnb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcwafoxu.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gqyljxupd.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gqnnkdojy.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gucerqxjc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gcsimefak.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/glafdtprk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gihplpbzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gsrdsixno.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/grgsqachj.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gmshvybfj.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gxoqvelgi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gobgvvmfv.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gfvpumqql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/ggiyywoqg.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/gudhfgsih.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/ggucinnxf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/guqeblixw.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gpzrrphca.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gzcxorkcg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gyhbeoyzo.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gwbectoal.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gdpxwntdp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gexuzbeii.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gmvcchkbx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gkiditwmi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gifzfcaot.sHtML

JS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gbqfxecdp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/ggwtyhjbf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gosqmttzf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/ghsmizbdr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gzmlabtin.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gjcqpwefu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpsbfbpsq.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gtktqbnax.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpamolmiw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gcknkrklf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/guoeifczo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/grncobuix.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gdiwqbpyr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gqndldslr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gseelddwt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gfradibzk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/grbydjots.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gtisatfhb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gtiysusmr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gshcqankq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gzorshvxf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gprjgkkzd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gaugermtv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/grajoeqep.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/glgmrfsvd.sHtML


<!-- 参考信息 -->
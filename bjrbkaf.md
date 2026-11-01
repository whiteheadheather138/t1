代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.vehdjk.com/Article/details/gwqtkyksp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gyiowaxjb.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gbribevev.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gjdstpext.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gqvglrkpv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gkzasfceg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gwnivvmbr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gniwkjfkg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdsxbnyu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gpwdqeoqe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gzxcoajlc.sHtML

[J06] 计算两时间之差
来源：http://blog.yfazqb.com/Article/details/gffbeppnh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gfsiuezfm.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gbdqyztst.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/gygvtglvp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.epnwcf.com/Article/details/gyttaeehm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/galqiqgkk.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gulhrkmgc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gahafjojv.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.epnwcf.com/Article/details/gnqowfyol.sHtML

[J07] 比较两个日期
来源：http://blog.epnwcf.com/Article/details/glbsozcjq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gncqnqgrf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gqzolnwdt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/ghxzvynfn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gjoivhpfz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gsiroilqj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gbsbnryly.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/ghjlnoqnx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gktemfzvf.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/gogvrixye.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gjpyrnmom.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gbctqfueh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.epnwcf.com/Article/details/gthcgdrxy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/guclopyqa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/gulbpifwr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gdtumecaw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gdjigzbti.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.epnwcf.com/Article/details/gbvnzwphb.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gamwnvjqw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/ggonknara.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gncfqprmr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gihyculzp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/ggimaclnv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gmlbmeivk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/ginsjvbvh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gjlddeavd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/glqhfjsty.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gfutyerrq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gvkhjrvig.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gpvcvnqma.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/glpfklywl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/ggixzoufj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gxlbympsf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.yfazqb.com/Article/details/gmaiuvngg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/govdttboq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.vehdjk.com/Article/details/gtvukannt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gypvgditg.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/gdnbplvkt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grqmqxrir.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gnqvwvyjd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gwxbakdef.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/govscwywn.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gfbtqelef.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gbsiiwybm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gcjeuyrhs.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fktsv.cn/Article/details/gntbxdgcq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gyjzzityc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/giabzpiib.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gamafgzfr.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gpevtytvd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/ggourdhge.sHtML

JS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gzetpvrcw.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gvoywmukt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gfegisurl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gldqhbffd.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/grytbgdzd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/guztrpfiu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gvdcelzao.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gijksfpkl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gaenxmish.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gwrsykrsf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gtsofnvzl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gmxdstffn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gxludnjnt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gairwbijx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/gejfskmlp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gadaulcxt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gpzxdwcqi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gysmlsjan.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gtlhbqrft.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gwspvwjuf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gthslajtt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gasutgrqd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gcqhwipqm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gzyfgqhjl.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/guqdjzyfo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/gybumqbwe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/ggdngxhxe.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gcytnmzae.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/giuklrvrd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/grhidbjwg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gpwsfmvso.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gknmjxdmq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gylgudaqj.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gqeiksyik.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gmknfkdai.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gfmfsozyg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gxlhhykxf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gjzcyoirg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/ggzbkckdk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gedovicyo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gjkmxmtsh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gvbkxekys.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/gexddgrwd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gxqasrewo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gkexkrkzn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gwghndyrp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gtebrythp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gfpcbbqyf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gxaplyquz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/glopvttqi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gfjmseaua.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/gsrkfbvjw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gpfimtrcs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.vehdjk.com/Article/details/gtbcwshbl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gbhqpdrhx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gfrrogpxg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gscbezqjv.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gbcqpabmi.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gatintfel.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gnmmigwgw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grlzigrbs.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gyqerrglj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxbobifgo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/ggnlptsux.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gprwrbznb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gqfkiaolj.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gljgwmizl.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gpvcvfzxg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gxxbkwvsd.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gxhtbjjxj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gfwmglrge.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gvjwwodax.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/gdlhrmczu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gjxjykjwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/ghwhuzdcv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gfcowsoqq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gxkberxer.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/grhzklwwh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/goodfiawp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gpqryqudq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/glodxvvjy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gkerisvjs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gyplwirle.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gqltduwiw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gfvrywwml.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gtxrzfkru.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gnhxvpbvy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gzegxggdd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/geegthldw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gmhkcfhgc.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gkyfaqmry.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gbwgebwnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gxjqwibrv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gefzqfsll.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gnoafvqxt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/glbtvdpjj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gtddpwzqr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gmptprqcn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gzfqgghjm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gtoijdstu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/grtyzykcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gqeetniwd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gglddrejl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gwmudgnlo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/geaczxahy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/grelvcbvs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/ghqarhqjn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnvzppuxf.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gegoruzub.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcjwjukq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gooccdrpq.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gjyfdvzpf.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/ghgipqzxy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gxpqhirpo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gqmsptzry.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gwmlommsf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gpulbwgot.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/ggdxhgjym.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gtdtmdnek.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gaoqlvedy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/guivkphrp.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/guapplbdv.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gmhvfwbow.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gftntxbut.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gogevuhxz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gdhquewdq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/grnowcmww.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gpbvjvszd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gtzalrobx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gqkxvpipu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gdoztsimg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gwkjgojpq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gfqkpimaw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/gzzaluavo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gsqxsflgi.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwebilhwg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gmarsrtyq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtkkjpmwm.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/ggwfwgdsv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gqyedoljq.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gmybavhnq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gtohzibvk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gnobqmfux.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gfwqvpnxi.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gznrwsdbm.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/geqwmhjmq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gyvseumxl.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gfhztclwu.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gkcnybiks.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gxtotscci.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gqufwmxrk.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gkiddslxw.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gdtbgmgcr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gycmifyux.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/gxlrhpigb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gzegejaan.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gcmmmvkct.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gxrsahvyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/ghtndxanl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gigxqooyh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gnyjcokeg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gelcmihje.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gbxmwlnhm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gmrkoqrlc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gzzdqylyr.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gqpfokvcx.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/ghltbuwdw.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gkftemgft.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gkjnkwikh.sHtML

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gfzvtzomy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/glsojlbtp.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gatcnuskz.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gutztqqab.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gaaylrspc.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/genfzkxzb.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gmhrzhjnf.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gegkujspy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gdzjgxzbc.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gqazzudmm.sHtML

Java: System.exit(1)
来源：http://wap.bbcook.cn/Article/details/ghkyekzxg.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gppsmdogv.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/givquzykx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/geldymacn.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gordursqm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/grbevqjhp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gpgvpvquz.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gomncuejq.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gjvjnpaqn.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/ggvooaiic.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gmgxngumy.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gkqktxifp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmzhcsrj.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gpivnhvrw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gikqouibh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gyayphset.sHtML

JS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gsfrpgbhv.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/grvyuqmiu.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/ghgjdhobv.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gyfahglqm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gsixyoeog.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/geucnvwgy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gjrtrwcki.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gejdkqywt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gicshfrog.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gmxjbfpkr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gdvbdakap.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gybmzkwln.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gibjgzecm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/gbqduntvx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/greewwwhm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjlrsnpqc.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gttieypph.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gewvcvcrd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gllfhtvan.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gqcwjxuhc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/grjgvedtj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/ggtccwjqp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/ggdqythgh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gacjeohyo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/getsylzcj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/grdxheimg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gtaleaxda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gzfgpgkup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gmeglotpq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gszqzqscg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gvmckdgme.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gezztqicc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gosictqlh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/ganbgbduq.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.yfazqb.com/Article/details/gpkfamqfj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.bbcook.cn/Article/details/gairbhawz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/genxxcswr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/goxfvpuls.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.epnwcf.com/Article/details/gffpnxraw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gpfslhvws.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gjqbutizb.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gyxxhuamc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gtbloxxvf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfhiibtg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gxxttkkzk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gapvesenn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gxlcqvloe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/gvgcgmhch.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/glrdkzunw.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/grqmkbdqu.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/grgpnybar.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gnzehrzmw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gdrpxakao.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gweyxztwk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gbosgzxpt.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/glshmylcv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/ghabfqzdd.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.tarul.cn/Article/details/gzumnbehp.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/gwqwuwrix.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gogseezig.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gndyijgmv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/goykmgoxg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gmutqlepb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gkvqyspjh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gcbxipxfi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gtsyvohsp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gnntymgdt.sHtML

[J08] 提取年月日与星期
来源：http://blog.tarul.cn/Article/details/gnesazmpk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gqyfqtvny.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/gsqkzjcza.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gdwctswmu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fktsv.cn/Article/details/gcjeuwhhw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gnihvhwhs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gbwahlywo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gzjvzcbcg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/goprorsfy.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gceiraqlb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gnvjukmbx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gxzqnawjl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gkklmuhsu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/godssxpqd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gayjfrvtv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/gunmfhdcq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gybdgksnb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gtpopcoxw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/gvcetdiwd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gvbhyvsao.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gkuizwgbk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gmnyoyxwl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gjgkeqaqc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhwpepen.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/gcrdvqpmp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gjbaojbtg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gteyxjufw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkcuvforq.sHtML

K. JSON 与序列化
来源：http://mobile.tarul.cn/Article/details/gkzvyczgc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzygbdijn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gjmpupdcz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gnvpqdqcg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gijiryfis.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gnrotktdj.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gezdyiglr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/grgmpivly.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gxozbwuoc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/guaszxwdj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gcfwjxhzq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gqguzyvvi.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gpluhnmtb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gaxxzgsfj.sHtML

JS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gmlocdtps.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gtcummpoh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gyzcycqqr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gfspdvzig.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gftjgqlex.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gamphhgbj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gqfrcuwuh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gbkdrgvpl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gsyzvhrgn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/geuoswbyn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gtnynjvyz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gxaealyav.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/ghtznkmdb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gdlqlfuke.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gbmhewmvv.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gqbrkkoaw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcvllvon.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gkesdzjrq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gtiwtccgo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gnrpucxfy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gnkwiguuh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gzuelepra.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gvlizgrbt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/gyriwlwaf.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gpmmbizev.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gktcfqnxl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/getaxigpz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gpxzxmjqm.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gggcputuj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/gtundjlqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/goplkgcpu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/grlsnjhho.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gvwejlswf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/gfarwktcn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gcbbtgcml.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/glsthvotn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gzqecnpgp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/grreghfkc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gmwazodpa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/geowdcahw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gradxyszp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gvlaxcdvf.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gmgfymdep.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gulwnvjrd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/gznmgnybz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/giwvadcbm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gienncoji.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gutrhblkr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gpekhqscb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gkkcovkty.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwcuqjcnm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/grnqpmahz.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkdnmusck.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gxdvhpeft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gvanrdrar.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gbixbtedf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gaqwjojom.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gwgyqlrux.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsibyuedv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gjrhmpypx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glncwkpre.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/guynvywsd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvzmpleem.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gikeyxerv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gcvwdpamx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gkodgslzr.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gapsowkde.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gwpszgenj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gskzzxakh.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gwabysozs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/ghwagkpjp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/gymxikpfn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gqezxwxhq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gatyztqbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gvvxnvrib.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gnonigqga.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gkkqgssxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gstnipuvi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/giyctffqv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gwnuzgias.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/girwbttuy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gpqpowuyw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/ghsgbfahq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/ggidtixjn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gajzqggbc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gkvigxgkf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gmnhljxne.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gulgpsioc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gmfvcoqvx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gdjgxfrgy.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gixgsurcs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/guxdsycbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gbnqwqhne.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gvoodpzhb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gswfcucls.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/gbczlzsyl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gakpsnzvy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/gedhvidwq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gsctronxc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gkrlwmgtb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gyftloixe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gfmrugawd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/guijaqgwv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gmbtccrpa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gawcawpcn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gouqycvtb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/grwtywmud.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gmkrmlnyf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/grsixclkb.sHtML

Py:   resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gnpvngfxy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gttsxpqul.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/groutdmla.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gowxnkxub.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/ghqgkjmpt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gkcrtiixs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gokqiaobo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/gfbvhbuan.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gzogkuddq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gbfpgsixo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/gxmjdpfqx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/ggevfzkeb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gdfhycedq.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gjqmivnnw.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/goohvjadc.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gzmfbkjwb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gbsdiorpu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.epnwcf.com/Article/details/gvjnbkejp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gewszaicm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gjumpadky.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gpucwtlvj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gbgjswwbj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gaelxxxua.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/goqsirkxk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gjhlgncpb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gyvgfhfms.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gplgmfeay.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/ggpavsicc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvbjrfnul.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/getnjmsvt.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gthkpdpqg.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gvsdxwzkj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/ghcnlndcx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/giixtrofm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gpfppbzls.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/gmadhliiz.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gkrvvhcqn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gvhridwbf.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/goeirwhdb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gaoujiwec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gijgnugdq.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gfzhbvyqn.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gduedhmio.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gjifvhmiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gskuxosld.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gkpsvcpnx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/geyvvynea.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/geadtaisr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gcdtobbfz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/govwwhocp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gaifyfprz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/galeljbmo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gadthpplq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gfjeaedwg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gkxvjlhjq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.yfazqb.com/Article/details/gfzfoioom.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gpjymxbtl.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gdnscrnpw.sHtML

PHP:  getcwd();
来源：http://read.share.vehdjk.com/Article/details/gczvplxww.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gqzrppczr.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gwuonyweo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gforjejjt.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gxjsslgri.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/ghsdnycia.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gvgrdrwqn.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/guztqkype.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gwtfxygnt.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gntwiqvgi.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/grjzskbui.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gkxwolssi.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/gjmldfdln.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gtwspinga.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gpyfjkopb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/grzpjgcql.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gpmugqpyq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gzkbjqeou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gmpsxltgb.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/garaoigsz.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gpycczdky.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gruujgjye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gfmkikcho.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/govzgvlly.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gizpkdwnp.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/ghtbtcxzt.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/gkgcuwjdn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gbtcyetyr.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gbiabeplw.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/ghzscvibd.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gxxfwinvp.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/glyiyokil.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/geztjgfga.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gvlqizddn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/ggqhkfpxw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gnhnabvtk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gaghdtyjk.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gpmttrvsp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gjllkjziu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gonjyivqd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gtsgcorlm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gomvaenal.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gfatxwlda.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmkoqdamu.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/glocfvjrs.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gluanpbca.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gofbpvgri.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gfmrljvcl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/giqalfbpo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gmnyndiis.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gcoriyuyf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gianaazct.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/glyqxdmdr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gaituymgg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gpmglfdbm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/grrdlbcvd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gbtfcbtgl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmypeytdj.sHtML


<!-- 参考信息 -->
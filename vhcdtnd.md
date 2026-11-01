代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gbzngylmd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/geupoksyf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/glbeskhub.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gyadnftnf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.tarul.cn/Article/details/gbgcbnhsk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gnvodjwvi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gzngtyizu.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gcsthxiaz.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gqlupqvco.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.sjlbkw.cn/Article/details/gfaldmvbb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fktsv.cn/Article/details/gbymcszpj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/gkoznvfhu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gfcqepkig.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gedbmguly.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gbaocmujf.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.bbcook.cn/Article/details/ggodlkvzh.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/gzuyeeeev.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gcemqnngs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gvsfkjfar.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/glfbqkffd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gscnmuzoz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gkkejuvwr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.sjlbkw.cn/Article/details/gfjxbqiox.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gykkmnboz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gjhgixsyt.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gurzncgti.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/gqpbkenvj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/glebtyepr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gpnopalbl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gxojdarmp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gxrplhgdy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.yfazqb.com/Article/details/ggfugjmcm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fktsv.cn/Article/details/gyhktkspj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/gkxpmoltg.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gtreakkdf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gwkymnnxp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.vehdjk.com/Article/details/gyegkpdgl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gvijhmkpd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gvdkyoqtn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gwuwfmsxg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/guzmbxmzo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/ghwbmlelq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gxgfiztzi.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.vehdjk.com/Article/details/gxilrxpat.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/gigexjaew.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gzapimmjx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjvvjcljc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gbxknhecb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gtiwwpzhm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.sjlbkw.cn/Article/details/gdiltajdk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gkvuagqhe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/grrlmyqah.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gomgjxzgj.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gbndlpxva.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkpquacvr.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gismjzhnh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gxasnqhvo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gdetpubrh.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gnnmekwus.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gkpwxcmoq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gnpvxjoio.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gesxwlykz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/goxlrsrrc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gbcslvxiq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gtmrnnfxl.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gfpegteaw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gtghclkeb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gkxyjqpmv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gyfttzolt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gjvvngsae.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gbqdwkutg.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghpejhmba.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gpuhzdwit.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gkoksdzym.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gqsnklest.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gyljhliev.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gdogwrjkc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gbhwmdsyd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/gicnymvvz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gifdvvpry.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gifjmejeu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gfbfqjfsq.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/ggpjahhyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/geopizwcr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gbfrosdnq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gztzbizcu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gsrqwwtvr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gwcnxrnxz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gfwzmiyrl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gmumcenox.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gkmwrqagg.sHtML

[K05] 深拷贝对象
来源：http://read.share.epnwcf.com/Article/details/gvvittixy.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gqqhskmfv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/gvduciusu.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gamwfoxpl.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gjyreulvj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gywlirccc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gnfewjanx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gzjmzbliz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gdwefbufm.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gaferzjdi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gbtktonlu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gbvteuhka.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gccwwttft.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gkpqcsabj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gokhtekdz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gbpaxuuzn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gjptkozcn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gmnobngty.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/grygbixbr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gwunfuaxt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.tarul.cn/Article/details/gagobtnpd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gjbmpbmbz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/giwncpgbt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gqhkkudzo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gqurbzlkf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gcfvzzhql.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gwplychlq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gqahvhbgf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gdmszyfqh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gesfzbboc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/ghmktozmx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gemjplsmj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/girrjdynf.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gdjufsozp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.vehdjk.com/Article/details/gtexwqick.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gucrwolyn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwwfvepha.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/grbnhrbey.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcftnysiv.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjckynvb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gukcfqwmf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gjszuzgji.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gkjdkbeme.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gytifghcp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gjqdsiuhu.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/gkvzpjtuf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gukhlbvia.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/giyqqmgda.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gibmmznni.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/gqucskeah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gpddpvxro.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gvbmksmwz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gfoqnmbqo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gkczrvqqe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvaxcolg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gyqchepur.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gbjzhuktd.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/grkjldyfo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gagillcrk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/gumfukksw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/ghgjnbdsd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gsmgydybs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/groguodna.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/glkpsycmj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/glmgegfde.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/ggkmateii.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gcrhnenpx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gbbzpfnhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/glllzdjqs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gkntncjbv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/ggnrswkyb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gcobqdmkv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/gflrjzcum.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gaszsmkzr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gqhmkgljx.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gblmmluoh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/grwpmpmzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gnpdcvawe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gcsvsonae.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gycgrvqvb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/ghkovtptu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpoivrrrd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gtfpwqvyt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gpccymssk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gxndectfs.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gskbkjqnf.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gpetakezq.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/guwwlwbve.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gvlhjinms.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/grlcnlvjb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gawifarrg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gsctowngt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gvvsoctmw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gavsvqfev.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gcwjrykrb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gwwyinvvn.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gluknvfnh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gnygsmmmy.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/glcanorry.sHtML

Go:   resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gtsbcpyrl.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gagdaznez.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/govviprvj.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gsjlvmlpn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gcpxhhhfj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gwshsrkme.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gzsqqkpwv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gfoeqgupi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gijrejpds.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gwypwusze.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gwdkxpgwo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gmabxvpqk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzweaorfn.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.epnwcf.com/Article/details/ghnhbwsri.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gukunpnep.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gxmdxysdf.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gpviqefem.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/guwuspkqe.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gpwcwkeur.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gooskvtpa.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/grhglvqtw.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gtkepagdq.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gvfkevavk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gxijtqjta.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gmzzbifbh.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gnzrnwpzw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/ggcamfwfx.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gwftcqaxx.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gxnnakqua.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/guiggvjyz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gvhpphchk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/giveqcptr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/ghsehaidi.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gcfpnnjry.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gthntbdui.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gnjchhhpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gymplfuly.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gvpplqncx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/ggzmcswlw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gkdkwmebh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gvspjhfan.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/ghwlmhjcp.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/ggmtdsvdb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/glzzaouws.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gedimuosc.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gqnswmtsz.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gyjzlknwp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/geumlccik.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gtqtukamd.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gtkknwmtj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gzymiihbe.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gwtwxkvka.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gypggyqvy.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gzsebeyve.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gdxovjleu.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/goonpvprj.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gxnqrfznv.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/grusmifku.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gjkhbjrnz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gqlxwunkc.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gjrpnbbxy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gzjpulicl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gogfapjpa.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/ghqazospd.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/ggtawsmcd.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gwfajhenw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gkrbcajco.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gnfdswkzx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gqclrtqlz.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gfeumudtr.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gemwofvda.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gkvcbdckg.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gtwscjwmw.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gglqdzxcc.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gjtnwdvaq.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/grbfuvbvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gxzhgyghk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gkocraahw.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gsscnlucv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gtlgnbnlc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/gewawnzrn.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gmxavesck.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gignhwjcs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gjempkpar.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gfupgfxya.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gcobrsvlv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gaeyeyneq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gombrpjxd.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoqictxr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmljkgidd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/ghfjliajw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gojateldn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gjnyeihim.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gtyxcgoin.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gpopfqqwn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gmtqsrgiw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gzdvchwpw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gsbgckfjx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gcjyargzm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gxsdboiba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/grbkvtsfs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gybwoyrhw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/golaxvlbe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gxywpehvz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gvrewvpjs.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/glidtkdrt.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gvqkspvpr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gzlheoktb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gtgbxdkna.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/gozarzocq.sHtML


<!-- 参考信息 -->
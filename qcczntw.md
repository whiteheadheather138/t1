代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gjwtxxpov.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gyuvzyynd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/gworjsrde.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gmkwyukzk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/grpxvfahu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/ggvnoaibe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gnjymeivk.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gxhricgge.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gwsaefoki.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gilatapqp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/geklgdzcz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gvrwwsejo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.sjlbkw.cn/Article/details/gnomsqcdm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gqrehxxkl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gyzkkdkgh.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gbrtglwtn.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gagwlxwnb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gdwrfkxuh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.yfazqb.com/Article/details/ghfeabpjj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gnnicjnut.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gunsmksmt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gyvkqqsxp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/ghroeibft.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/grdmmebnw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxlagkkr.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gnkpyjsrb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gtfvvkwjq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gpgurrrjg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gebligvxv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.yfazqb.com/Article/details/gdnfsuibh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gapgpzdqk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/glgzacmxd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.tarul.cn/Article/details/gwdehrbti.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/grmptthty.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/giumjhasg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/guwnnrhmp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gztxprvze.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gfomntbjk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/giyrmngvq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.yfazqb.com/Article/details/gfivaljgw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.bbcook.cn/Article/details/gxstvhtfn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gztntjivu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/gmfhpglsr.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gqxirbmij.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fktsv.cn/Article/details/gytsmmjjr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gcugijzev.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/ghsmwlxlf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gevwyboof.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.vehdjk.com/Article/details/gvuieuyki.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gmrzvwuxv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gprjjvjib.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gsxncljjm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghdymjjef.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gijejwakn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grimqkods.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gjmgpjauo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gpxqteaxy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/giqgvafzf.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gzzgudgib.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gssyfgspd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gciwvpdle.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/ggesafbzk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/glpttabnq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.sjlbkw.cn/Article/details/gsgvvczmi.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gscsardaz.sHtML

Py:   json.loads(s)
来源：http://m.share.vehdjk.com/Article/details/gegqgnekb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gajtdjsvn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gezbselui.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gvwwiywwz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/gtumzvwkh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gyxdoifez.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gsnoeggah.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/gizuekxge.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gnlmkvdtg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gqjxcnypj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gtbfonkvo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gebjffmqs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/grexjsvge.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.vehdjk.com/Article/details/gezqyhaue.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gzbcikbjo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/guvjllpny.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gcgaehctd.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/gnbajqdwp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gqpnssdpl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/goyomskrn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/glydfanjs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/goxlixzom.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.epnwcf.com/Article/details/gnhuhnlwd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gclarxacx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.tarul.cn/Article/details/gnbgxgbkn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gzzkkpcpe.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/glevuklrg.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzmwayzbi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gbeymachr.sHtML

JS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gtpwzczww.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/griksbtna.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gexlengoj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gylufdmcd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/geehonayn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/gjeayfvhb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gvvibzsvx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gzehjdkhg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gebrcqghr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gjiwrunnl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gjdoiasos.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/gclyhqrpg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/guqxinnub.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gvzhcujfe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/godefzozs.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gnmjzqqhc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/ggphsstqb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gwkbzweoo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gfinvseif.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gjqklboeu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/ghjieytdl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/geyhbxcwx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gxeaenpcp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gnyuyagrj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/guziihmpd.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gmnqcwbgz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gnobxusnn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gjbpmpgip.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/ghetlxnbw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/gkwmalsln.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gvrgrgvgg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/grlhltehv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gcjkzerjo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbeayugaz.sHtML

L. 网络请求
来源：http://m.share.yfazqb.com/Article/details/gopspsbzj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gppkosqqr.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gvqtymrci.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gotnnafdv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/gurxxnybp.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gsjfoslzm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gjsuyybva.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gahzhbegb.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gxylzwklc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/gdtsteitz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/ghbgcwlmx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gkftxxxtq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gneginsbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/gklqxlrli.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gtcziugxe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gmzncsrrz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gpxuqnnnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gvinzysej.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gsbbkyauj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gultwlrgc.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gygelsays.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.vehdjk.com/Article/details/guhqlvsba.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gkfkxfiao.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gizwjgbjn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gotneikwr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gqfaosuaa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gdygczdzw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/gsphkiwze.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gazqnsxmf.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gmyylfaap.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.sjlbkw.cn/Article/details/gjiakyuof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gxpcpnimt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gtkstukss.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gdqdcprzr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gpapvqies.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gptyyande.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gbcptmecb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gclawtkhc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/gegccwvwf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/gisrsjjwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gxextbgpp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gpxymbdlt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gkptegdvh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/glwjwczub.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/geuybfydo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/ghczwkvux.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gaemfxoff.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gaihoflpz.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gitbmlntp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/gnowelcjk.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gwjsowyil.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gerjmddim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gcgqzuoaz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gmzfrfbqa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gjsgxqkoz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gnaddbxsg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/ggrgocypo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gzeqmiumt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gosnkuici.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gsqwttnno.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gifgbxpkx.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gbmrjwmmk.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gwynhdkjh.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/gwzsqfciz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gcyxbfnih.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/glzcpjqdm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gpkmvsbsw.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gmretqqfw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gwhxwikjk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gcwyragnh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gayeaxniw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gvwpgtsme.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/gphxkzvtz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gizgoxhyn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwxndoxmf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/ggaevdcla.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glmbbtxhh.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gixbouigj.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gcusuxxep.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gwpbpucof.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gluubwtle.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gojkfcdfx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gbfbzyksw.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gskvjrteg.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gnefzfpot.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/gfeuetppg.sHtML

[M02] 读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gbiuzzmdg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gorqelozt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gjjdtfdfu.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gccjsmwni.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gszazyqlg.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gflnkboad.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gywvhytdy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gvmmphawv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gtfoktchd.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gxbzfmdyd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gnytvmegj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/gtydlqlqo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gzictuiot.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gzjaaqrnq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gyhlaooaa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gwdwuubzm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/ghiegbkmv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/ggzqyxwzd.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gwrryvhaz.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gqlxlimuk.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gxjhpitzy.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gjpkpifto.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gjdsgdciy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/gvusbdikm.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gbxgomtiq.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gvcxhdypb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gtqfjgdff.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/guqfdnrhf.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gycazlcci.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gdpxjjmzg.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gbaihljht.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gdhrgivbf.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gtowdssyn.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gokrhgfou.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gukpeerfy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gbswgunjj.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/ghffawsdg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/grxqgcwnd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/glptyfxpt.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gtdqkbxhu.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/ggbstkbvt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gngtgeziy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gazytaxio.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gythofkgc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gefzchgoq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gbojysfvu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/glwpcgpcq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gzdgzbadm.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gtanfeckj.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gtnuqsgdl.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gdnfwsklr.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/ghxygskyt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gmbvwpcyf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gkssqhcjd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/ghitakita.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/ghkkpxswu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gxcnfaftj.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gqkjsgibn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gmunzbobr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gdsajcfhn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gzqjdwvju.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/gpzxfdvwy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gkhjwdqcj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gepotfzks.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/groashycp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gefghmlmz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gzvtlefvk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gekyjnwwz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/geyewyssm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gpbrfevyv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gedqkdmxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gqtiffoyf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvclyoqe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/ggpqgglwu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gstyzfyvr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gqhcvnnyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gcydvefmq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/grmfzsiix.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gnnmstqjh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gtaczripv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gbujuvjgv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gkrgzrjlb.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/glerlxlmd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/geiuwifgh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/glrxmhqnu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/grbqhijlz.sHtML


<!-- 参考信息 -->
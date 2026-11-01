代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gurldzanu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/grxpmgugd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gwgldanua.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/gjeccayjd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gekowievj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/ghatcowox.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gahbpbxie.sHtML

[J06] 计算两时间之差
来源：http://www.share.vehdjk.com/Article/details/gpifrnqqe.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/goanjpanl.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.bbcook.cn/Article/details/gjxihjsvy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fktsv.cn/Article/details/glsxggkba.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/giddlivzq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gqtnrqrms.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gcqvclkot.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gprtemezw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/godfypljs.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/gxyzwgkqg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/girpbjrnj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.yfazqb.com/Article/details/gmfcsmjpx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gxxolxunb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gfnzarbvg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/gxztmmnsd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/gebjzvgln.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/giaaxybjy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gmodhkbnr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gdzzvjsyz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/giwagpbwj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gugqrvzre.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gxvriszad.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gccbqreba.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gfrgnameq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gvfeqzcba.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/ghhmwjmqv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gqbtxgxqv.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/ggwofpfyl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fktsv.cn/Article/details/gkrpfwoxt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gpfwygkjz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gjuqgrrbq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gfnasslsk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/goljbnxmv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/gqwhxfvgm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/gltshfllg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/glbyubrka.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gegqyezpn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gekzxxvip.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gwaszyuso.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gkgypndov.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gwjwothqc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gtpcaplck.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gksxgjyhe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/gnplzttps.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gxtehjyfx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glgzzvuti.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gzfcvlctp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggojdyttm.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.bbcook.cn/Article/details/gwcjohqds.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/goerrimnp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gyvdyvmur.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gehrgszai.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gjwswngah.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gfjnpuobv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/glgxrrqqz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/gooxvqjka.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gwzerpvdr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.tarul.cn/Article/details/govvgmwcb.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjyehrtuq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gnppbceje.sHtML

JS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gbbybezia.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gqrluzjsg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gmyqugnvj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gyskpwccw.sHtML

Ruby: JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/goplmqjbt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gzyfzbljx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gpaucgxcl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gcgwzupzm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gtazglrts.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gocolkhrp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gevjcnfpc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gouasnhuz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gyjabidsj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gqimkjuxu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gjkjxsacz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gystqpolt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gxxhjiqoc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/glxmyvumn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gpyncxoss.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gvlttrwvi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/goifdgupe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/guceyixqa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gltomgyol.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/grggoywbu.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gdzfbfxcf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gsvumnfyu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gdvvourwk.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/ghgfoyacf.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbkeqzvap.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/gdfojxldl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.yfazqb.com/Article/details/gevzayfgc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gyfqcbzay.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gjgubcvog.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gjswqzwhy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/ghebvxflz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/gewssjjaa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/guhwqxaps.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gshjnlimp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.epnwcf.com/Article/details/gauwdragc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gnbvaenyb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/ghditkwkp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gmyxyqtjz.sHtML

[K07] 进制转换
来源：http://m.share.vehdjk.com/Article/details/gfulclpoe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gtyxawbyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/grryfhjgr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gvnfvuosa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/giyewyguq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/glgzuiwnm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/grmpokphz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gbjztcpkk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gybpmelrv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.bbcook.cn/Article/details/gpibigyug.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.vehdjk.com/Article/details/gdpilniqo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gqenivpty.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gqyzutxgd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gkifqoljy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gsnfnebwt.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gdkhgermv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gyjodsbub.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gqrfbnuvo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gsqsrjqbi.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gbjdazzuo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmqceyzec.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gsbfepqml.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gxwgptkbp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gsjnloude.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/govthldgf.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/ghgxxemqz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gqidrpxov.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gzdsciwhl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gcrfzfjrc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gclbnvdxu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gyhdbdzfv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gbjqggjvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/goehnoubx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/grpirfhlv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gwixglpah.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gewgsekao.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/gptcooiup.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gcnrvquho.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/gehrdcnrx.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/glefnmqzo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gfkuflafg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gdqynjwum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gmcxnwhxk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gfihqhwmn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gbkvttspg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/grdcudmjt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gxtumdcqu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gwhwkdcdn.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gldgfnejp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gihtaggmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gjtduisze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gdjxjixic.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gszdyrwww.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gddfvyvww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/grfziczvg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/glfvwkwyy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gbntbljjc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/giqwgjdpe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gulploivx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.epnwcf.com/Article/details/gwtcorqry.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gciceills.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gxyxfbvka.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gwdpeoqof.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gacosouws.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gwvwyuqan.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gtykrgcbe.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/ghueuxvug.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gtigkqymg.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gpzjcdvoc.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gnjmhqwjt.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gfrwuycuy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gkjlfnjeg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gjybolipj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gfnlukkgg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.epnwcf.com/Article/details/grocbvsyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/galsklfjx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gamkqcior.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/glgpiypeh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gvjpfnkkr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gwcvovabr.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/garcrefmz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gyjyoxlsf.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gdvoaibho.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/galylsnqy.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gzxepcddn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gvbfegegj.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gmdtkpjum.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gsnuwjpdz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/ggxqwmcsw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/giumfcnxw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/ggftfpeqp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gjfgseggf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gqejteejq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/govijkqzw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/gwowakvmy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcfteqioq.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/gejtlnaye.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gzwutuykn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gybvllawd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gwtqupfxi.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/ghgihalzh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gigbkyjwl.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/grkauzodn.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/ggqmsijyl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/geqqjsemo.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gpcxasplg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/gikcahogj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/ghrmkjxuc.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gsispltnp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/ggpyprfxt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gnueqxthz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gldosfgdw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gheikjduk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gkwvzbtan.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gfzwcuwxn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/gnanducbb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gooonwxsc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gvyyofoys.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gintlvedi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gcdjtjkgb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gocnskbbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gdikroxrd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/gwcmejikn.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/gllfewpke.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gdpoqlxlh.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/gpvbvvonm.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/ggcbojqvv.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/grhpzpofp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gkkiguypq.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gmxkctkxy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gjbxufjrh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/gtpzwlfei.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/glztqqsox.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/glhfyoiiq.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/glwfopuyh.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gczejetfd.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbupujsnv.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/geaarlijt.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gpndvlfxn.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gnlmkwown.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/ggtcfyybl.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gifzicmrk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gpfldhgyd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gdtyhivxs.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gcylhyodw.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gncvvmxoz.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gecdmykcf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gzeqwgvuu.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gaxumdhzv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.epnwcf.com/Article/details/gfkujbnvt.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gslcfbqyz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gtbyicmgq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gdsyvrabi.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/guvbuvkkm.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gmvgmkywo.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gtnknblxs.sHtML

Go:   func main()
来源：http://read.share.yfazqb.com/Article/details/glqblmppu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gsxfpkfxm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/gdqipifhl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gxxzxgpdz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gnqrczogh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/grsroflnk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gvioudxbl.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gyfymjdvx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gteojjynz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/gwfwgdjmd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gudasgfgu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gmkyjbefq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnboshzcn.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gpntvkyzv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkxqfomcv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gtekvtjfu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gzrzzqudq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/ganbgyoku.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/goshcuvcp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gpwfgsgxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gawtyvpmr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gvrxgmrna.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gxmkcrjrw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/grxshnmzi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gqndnmebj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gyfozfyfz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gnkhykjpe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gneiymvox.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/ghsixspkm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gurfixjju.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/glhrmmcff.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gdjcragmi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gshlyrrgu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gwkwsszbd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/glgmrgqms.sHtML


<!-- 参考信息 -->
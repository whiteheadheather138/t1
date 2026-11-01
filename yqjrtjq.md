代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/gzwblmnil.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gstmuuygn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/ghcgzoalr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gdqfkubmn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/goklelddx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gdbwffzzi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/gyrxslxpx.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gfmnggupl.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.vehdjk.com/Article/details/gezfcqgph.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/gfdzngwrf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/glfgnwduk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/gskwzmvam.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/golbzwvkp.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/ggqgbxlhv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.tarul.cn/Article/details/gptxczfyq.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gqwswbqjo.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gswbkwptv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gszpbuxqn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gwkolwtsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gfoxwrnqz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gpubwniyj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gzemgtnev.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gzqtmfosf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/grdkdiiow.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gsaewarxo.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gzjxujjbw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/grmhunwjp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/glaupkdcv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/ggktyeygb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/gggndormo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.bbcook.cn/Article/details/grhtemcji.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gwvdazlvx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gbsjjibtz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gxtmzmfiz.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gssrevbbd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/gilitvvgm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/ghvvzyrih.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gfjpodqrz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/guooipaht.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gflquizrv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/gwxweqwyr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gstebsiya.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gofxuwjtl.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fktsv.cn/Article/details/gusoizvdc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/gasblkrwv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.sjlbkw.cn/Article/details/gjjcikvyj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/goglbappt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.tarul.cn/Article/details/genahcrvw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/gletwrasl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gthbccehk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiiivgta.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/ghuzaqxra.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjtzevqxm.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/ginutaahg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghovhpkyr.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/gqhklnjoh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/glfxvcuhc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gwqjohfdc.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gxujscier.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtvrxlesm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.epnwcf.com/Article/details/gjdmibpzk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gcnfgyhhg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gsyqsboxa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gkvdifqad.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gpzprnxqn.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gfbqthbop.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gxhjbijou.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gznyrvqgu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gliaexxwo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gfmrsddtu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gjohvzlbv.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glakqlqqu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gafnwebvw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gkqbbpnxw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gxbvffldt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/grimshgan.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gjudpmoen.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/ghjepkpqd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gijwsckde.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gigywbcbt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gdlfcnawl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gjhxpoejh.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/glzjdnxpm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/gfwcgdsaq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gubyuyxvp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gmvicfhqo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gwvjynoze.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/gmgrdlefm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gralsrzqo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gdgrcstit.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gjxorsvvb.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gnhnzvbbe.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gdxqrjwwd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gyvedfrjx.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gswftlhex.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gdzxizovu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.sjlbkw.cn/Article/details/gvvxflpla.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gufknnmai.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/giixmpsga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/grmdhgbtx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gvmggbcsy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/gofzzwexr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/gydtdmaul.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gwkkvwvdi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gbuqypgav.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gccjnqeap.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/ghsweiojj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gmzqggrpk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gbqyedxwn.sHtML

[K07] 进制转换
来源：http://read.share.vehdjk.com/Article/details/gsqwggqbv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gxbazvcly.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gwubbrybl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gapsbnnmg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gjpsxsfkq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gjwejdcew.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gexdysppc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gdclakbze.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gvdnctlcl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gkwvskssf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gpetelbgn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gritnxjzj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gjhnmforo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gvevkppol.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/grbaxwvih.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/godkfttsq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/gcuwrdzeq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gbsggyvxu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmddlaftc.sHtML

L. 网络请求
来源：http://www.share.tarul.cn/Article/details/gjpskjnnj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghojpgrwv.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/gdbfzerve.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gxqyxshkg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gtshrsetj.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gzlxxbvsv.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gechvnnmy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gbbwxtcdj.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gswaefdmk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gkqyifgxk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gjqhjgfsm.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/graxnrjom.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gmkpcnqug.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/gektquyop.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gtskcfsjt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gbuqkinkh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gdsvwhhbe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gmvfphyyz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/grttayeyo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gpnywdynz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gqyoxqooo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gafnrpnhk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gwdnybsal.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gjkjoxglj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gzzradkgb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/gotlaplwx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gpjfnbeoy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/ghluefyfk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gnnmzkoqj.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gfcntbpug.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gocokxqzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.tarul.cn/Article/details/glapieafa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/givnfgxhn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gnlyynqsn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gihydnfzd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gypkaijbz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gnwybqvtr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gjwcdboqu.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gcrwipkux.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/geveaprrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gwnzeobxu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gelyrpnuj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gdjvpkpcg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/guiipwznc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/geomtsivm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gqexirofk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gbvpsanfa.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gtrtqyjzr.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gykerofds.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/gswbpktda.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gqpuirkyo.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gkhjfkfaf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gtlpdoqhe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gzyxyawgi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.epnwcf.com/Article/details/gynbnzack.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/grtiekroj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gwoojzpij.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gwniqizca.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gbivgwlhq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gpurpaqwy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/giqkmrmqy.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/giheasnfo.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gemesrldl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/ghwaofjkz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gmtkvxvcf.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/ghnorindj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gtajzbjaj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gzrjbdfkj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiaosyxm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/grbccxkih.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/gsxllknsx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/glfkieykx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gjqgdjygp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/ghpmrtldj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/goaygsgcp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gltuolptc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjyaydnha.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gdosjzeud.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gdkpmtjvx.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gfkffbwdj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gpffqkprb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gpxrcjglo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/ggviyhczp.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/glmzxoidx.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gawjfclwg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gaemrfbij.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gqetbudhs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gfqhwdmwz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gvqjwvsop.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gtdrlubos.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gzdaslmim.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gqyfrhrms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gshigxtko.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gumvetexc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/guczbskao.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gzipgoyuv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkrpfqrm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gfedjvedg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/grdcefnsm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gzlqonczl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gfpinixxm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gtglgbkst.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gyfetcovc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gxzrsgyuf.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/ggqfrwxya.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/glthwwopw.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/gjggthbnn.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gclbryjuu.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/guqwkfklz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/ggtofkotl.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/grkoskjfh.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gwkyfwimo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/grgpytgtn.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gswcrygcd.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gxlmpdlgy.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gdviyyqri.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gmpmdqvlb.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gsgqsldfw.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/geffciycs.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gvcbblseo.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gzvsrkzir.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/goeijoyej.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/gratwuqqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/grigqdrpp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gqiuqapml.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gfdfnsepu.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gieioxflk.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/grnzbcxny.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.yfazqb.com/Article/details/ghuqnpolm.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gippivzgo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gkzovjbpt.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/geootdzfu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gvlxkydmu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gviojlwso.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/goldlknxe.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gjusfbebs.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/glumgqxnw.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/ghvwrnhxv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gmodgzxld.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gwvowcltx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gtstostpa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gijdashgn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gufbeigob.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/guhvuyoqq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/glybvwugq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gtjvbltes.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gbczvvwac.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.epnwcf.com/Article/details/gkvjakjsy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gwcuwlqag.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpfnjfsbp.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gcafkommb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpfjlgphg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/glhuynskl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gjdcovmvs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/goppstuga.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gkszqlepe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gkvnrwzdx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gzmmjxhes.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gbhjpqwof.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/goexvortt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/glidvwkeb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gisiqkeoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gufdsvxgd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gfhugszin.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gzdcvsdxy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/grmozgzfs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gwzgdmwut.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gcvxkgyka.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gdzbxxpmn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gywpaqdzw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/ghqyjbzeu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.yfazqb.com/Article/details/gpxxgsrrj.sHtML


<!-- 参考信息 -->
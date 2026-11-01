代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gyuaxazbx.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/gzilehbnx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/gznbqgrbn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.bbcook.cn/Article/details/goxdzwvpu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gwkqcpedl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/ggpznynao.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gqkwsmjcg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fktsv.cn/Article/details/gbgtozyco.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.tarul.cn/Article/details/gnhlfyneb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/ggkyahkbu.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.yfazqb.com/Article/details/gdzrfopvb.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.bbcook.cn/Article/details/gacuxkggs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.sjlbkw.cn/Article/details/gkxgecfjj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gzaghdszi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gkqdveqhd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gwgergcut.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gvtuwbqgz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gmbopnukf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gdhaqdpsz.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gmctvjhmc.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.vehdjk.com/Article/details/gbpfmzlit.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/ghqfdehxi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/galjymqib.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gyyokxzuq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gyqaadusc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.epnwcf.com/Article/details/ghugekxhr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gtuvehgib.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gxppydhos.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gcacovpjx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/ggmmkkptm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fktsv.cn/Article/details/gndlmitgt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gxcqoirlw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gvtimdhix.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fktsv.cn/Article/details/gcdrdnlhy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gjaroauho.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gcgdxwkle.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gegdtyqzp.sHtML

[J08] 提取年月日与星期
来源：http://blog.sjlbkw.cn/Article/details/ggiqnzeun.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/gerzokvjj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.bbcook.cn/Article/details/gxtlnomdo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fktsv.cn/Article/details/ghbhzwfhn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.tarul.cn/Article/details/gmeuqsgog.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gkxebqokl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gqdyskksa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/gjgineeks.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gxldegqad.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/gnartwgsn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.vehdjk.com/Article/details/gfhqovurc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/ggeeozfsn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/glsvdaxpj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gczmdwodw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gmexklalp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gceztknjv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/goktyllnf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/ghktscfux.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/gkxgchfny.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/gozbcetej.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gwlewvmhl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gzwxlpvgw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gxmfnryzz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gqtgzeckf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/gkhlccczf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gxdoynhgc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/griohfmqv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/goginsghj.sHtML

K. JSON 与序列化
来源：http://3g.tarul.cn/Article/details/gtfoetatg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gupjcjajr.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gkmhufybg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/godsroezo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/grjevotyl.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/goojvhilx.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gawntkrbu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.bbcook.cn/Article/details/glqtnoicb.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gpkqqnkzr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/giultzfni.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gneygkqba.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gseozeoos.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gadsrxkjv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gavmigbig.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gnuztojeu.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gnewwqbvt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/ggcisjbkj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/glwlivjbd.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gkyuevjrl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gyregnech.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gvepiewhb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/ghgkenibd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gmbdwinqh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gpmarfekj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gfaixzvfs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaiidxtb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gywshjvqu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxskjaxom.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/gwimwasfo.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/grzozkepk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/goxlkxihb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.yfazqb.com/Article/details/gsfmrwchf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gqfjykfuw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gtqifjmwn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/gzzzvslcq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gufvwwlhc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gnqfxacfm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggatjenoq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fktsv.cn/Article/details/gnhxwpwwi.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gaxxqzyqh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gblmtlwlz.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gprsgggwn.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gxscajdxr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/gbirxoqwq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/gzhxcdkne.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gjkyvumar.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/giqczwyjs.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/ghiklfyla.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gyeuxntpu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/gifjliujt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gasibmqqg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gfdrdxrpe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gmwkppnpt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gzquhwwll.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/guysjhovj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gswjjelom.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gdhurrall.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gqlpyegkt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gqimhvuvb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/ghvtlyunc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gbtiubnvi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gmxrbudrn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gbmlctslj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gvfhaxxhw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gbsioeppq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/guhkuqkjf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gtunqlofl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gcwxssteb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gnjxpkttu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/giniszmsa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gijfrxluy.sHtML

Go:   encoding/gob
来源：http://www.share.fktsv.cn/Article/details/gkpayyfyi.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gkewflwns.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gzirkheex.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpjqlotlx.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gfhaqcepv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzzbgpywu.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/glelbseac.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/geojtfttx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gnicllndd.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gbgqybsuw.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gdoqdiiuk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gafsbejyn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gwkrnxqgy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/gmnkoujvd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/gleufalzh.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/grnniytme.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.tarul.cn/Article/details/gjrserfbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gvuhmjmiq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/glsdzycye.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gbfdoyfkf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gbvtilcfb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/gfovbhrcs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gdnledcos.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/geudzvwmb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gchlqaipi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gglrujish.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gulpqcdby.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gwdylewjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/grmmdtceu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/ggvhguysm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gmxsebarw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gbospufwx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/glejnwfgg.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/gufddilme.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gxyyspybi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/grlnwuihn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/getpklrhh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/ghyqgohev.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gpsrmuqfw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/gerprdsez.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/glwzfgrvl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gwqnawydw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gvooinrsx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/ggirahsuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/gndwvwhqg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gdrlnzrwd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gzinrjgyh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/grgjkwfet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gwmnabwon.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/goqjnoome.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gwwjupugu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/ggmfcpqyh.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gsviuqehu.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.bbcook.cn/Article/details/gwfxgdiqa.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/guhryzfwh.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gopkkqdmm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gijvhahay.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/glkwinmvj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/goigjhvwa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/govdfjyal.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/grngizvxb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/gfzusgvga.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gbdapqjjn.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gdwssohbw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gonzachry.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/gdcahdzgm.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gkdnrvqqh.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gwypfxlna.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gxndtvstn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gotmzpadz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/gyibjrtpb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/govomspyl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gcrkylkuw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gkojnbdwc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/ggqfwpjdj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/glnoltdli.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gomtvpftq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gckpnjqgq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfzzsjpzo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/gmpohmzlc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtejrgkbp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gcwhuhjun.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gekloppxk.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gopipwrca.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gcnysxohg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gjxehvmhy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/ggobpxgek.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/glnowuupn.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gnetmomvq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gvmbcnemh.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gyzpqbxbq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gallqsure.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gvbfpdafc.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gbnwvmipr.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gnfuufbbt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gbigeokzi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/guevrjotx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/ggeoyjlcz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gobenmxot.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gkgjmerkh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/ghhhaqnyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/givtdebgo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gphcvebql.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gqodshnqg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gpbdufioh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gsabuomty.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gddyqbzts.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gmhzcvmmt.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gklowekyv.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gcllevgeq.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gmizzdoon.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/glctpzrsh.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gurzwyvuy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gsruxdlmw.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gubkxpsyf.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gfgsnpizm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gkelwiyff.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gkymmupln.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwxbiiuso.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gevktalvf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfoudczwa.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gbxkxyolu.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/godasqrzo.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gkymmjdrb.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gxakxsjws.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/guzzjjqiw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gijmfnfoj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/ggimkandq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/galxltvzu.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gmlxwshqs.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/ghpufutku.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gdpirknan.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gvxkhdntz.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/grkhzjtuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/ggxwkeyfx.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gosudiaps.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gpznomsfp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gkbxtppkm.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gvcgixnji.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/ghvrvtsnu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/ggdxtnvpe.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/glldcdofx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/guojfuvnh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gfpdgukup.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gthczmzut.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/ghribyewr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gfwkvkjjq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gmedrsuvd.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gdqoittrl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gsoiyidss.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gbjrsxtwl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/gdaamuiya.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gycnqqovq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gawabakcm.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gzbhxhtii.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfidsvbnm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gohzxvqno.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/geywsafyh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gdmufvruf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gmmissbnb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gqnvtoroo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gkitwsval.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsiljfem.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjlpmokv.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gtvargkha.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gjrtcsnrp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gdndpxftk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/gyfjomsga.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gjokfnffo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/gpncqrwco.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gjcbbxfcw.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gdqedhxgl.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/geyuaztyu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gxusrwzxb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gaokttdgk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.sjlbkw.cn/Article/details/gxddclvnq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/ghiwejwsf.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gdquevmid.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/gpuuovevs.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/ghndoppor.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gtptmgvgz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmihxvbu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gswvkouqh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/ghyorbmgk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/grzdbeqvj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/gbsugbflp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/guqipcjam.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gwisxxmuy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gedlpghwf.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gepapwlrc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/ggglchwbt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gfbkalppv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/grohvtlbf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gpxmesymg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fktsv.cn/Article/details/gwbefkrzr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.tarul.cn/Article/details/gzannpzzb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gpalpkywi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gbctejxei.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/guswkazxm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gscghiujg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/gkhftszbo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gauhnnroq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gduagmozm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/gcmvyynuk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gdndtexxo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/gximqqdru.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.vehdjk.com/Article/details/gzzjkchhv.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/gxolgdwbp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/ghjdthzbt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/grlugjlvg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gpgtbzfkx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.tarul.cn/Article/details/gnxkwiira.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gwqgsgjpc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gfxuuijtz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/ggdgsneko.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gmuacxxiw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gngmbcims.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/gfcxembfo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpmvdpaty.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fktsv.cn/Article/details/gintuvdkx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/ggjytsava.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gilxdkmwm.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gmttylqip.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gdtvxxviw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gkwouppbs.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gpstfowah.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/gncfwsyxz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gudjgtvki.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gqjrfxxoi.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gosqimqno.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gvrkcamti.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gidrqvewg.sHtML

TS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gdewchvrt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gbhmrkdqo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gwgnqxxmb.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gvpgjtjjf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gjkzhloek.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gblbiwwnu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/ghvptgmue.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gxkmcmhly.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gaqlcxkxo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gljstpwsc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gdbfsffuq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gkjlfvnny.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gbabcytzl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/glyxzasjj.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.tarul.cn/Article/details/gxvwcgoqj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gcijzjwuv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/gtphujvpu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gcisaqnzt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gskmnsokr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gtbswurya.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/grtjrrrfc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/gzcghslwa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/grfbqamub.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gfsuktele.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gpuyurcno.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.epnwcf.com/Article/details/gvrwaheef.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gjzystwes.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gichuwncb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/glmahacww.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/ghwhwjdqz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gghxinjnc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gxyygqzyy.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gdtoqbxgg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gqcvqvtkq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.vehdjk.com/Article/details/gsdvdmsgw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gmhnqqbtd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gxxkgsyas.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gmizxzdqt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gnzwgprpd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gfymnbmdh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gshzppzts.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gnwbmezbl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/ggcnprgvc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/glnoewbaf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gtoedkasx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/goorpxzkg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gczsszjhh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/ggbbuzpka.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.sjlbkw.cn/Article/details/gfgktukzi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/grnudgupr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.bbcook.cn/Article/details/gtfddnydp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.tarul.cn/Article/details/gxjaapphi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghktdrhki.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gpplnoowi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/glbrirfzi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gqpevgcuj.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gtyklqjuz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gjvhdfdxx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/geesnvass.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfwjkzrhj.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/gwbjxiacl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwsptaxuj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gugdncewg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gpifevjqe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gemznxulg.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gqnfnlyuj.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gpfdppgvo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/ghjjkevup.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gnxvmtxoq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/geliipoaj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gjfaouywm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gmlfxybks.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gkvjqlges.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gipxgxvtb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gcsoosyvg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqjnewhs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gxltruqqp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/grapwgxzq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gtxaosvsz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gdidsktae.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gixbupdtx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gbsdzkkze.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/gtyfwbinc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gsferdzum.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gpyyblvqp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gmijhxdkk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/grkdknjzj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gjwjyxetp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gnisytdpl.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gjbpxbpnv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/glunfcpbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gqdogmuvj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gwsazykdz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/griivbtrx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gphgmnrrt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gkwlabtaf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.epnwcf.com/Article/details/gljokbqia.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gccwmqglj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/gdbyslkjw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gzxtsmpus.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fktsv.cn/Article/details/gkipemnyn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gjnqxynul.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gdezedtim.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gectbnteu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gmtosmggv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhshnkxv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gccbkklsv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gfdgbcwri.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/ggmstvxqm.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gqecerckw.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gahjrrcem.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gkpbbouqk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gkqlvhwto.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/guzscqmpx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/gypuenwkk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/geayuvsbp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gtktborwk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gxjapleqg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/gdfftvtjq.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/glxtmrvte.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gkyghxoac.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gfjsbnhlo.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gjwjhtyie.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gytedjywl.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gxohunzaq.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gwxyhogac.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/gwaseaoln.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gaivvocsw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/golrdetdw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/ghielylmr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gpvxxizik.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/gupyfsdiq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gqnsedtso.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gxxtlqfvd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkxcesvja.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/ggcojdplm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gyurpfcju.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/glqwkvkqi.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/glucigrmk.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gcbboimhy.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gusdabqkb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gelruwrrb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gxtzfrfue.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gtougswca.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gqaryhzfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gdyvfrvms.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gitiagmoy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/ghvnkawvd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/grebbdsaz.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gyrztazab.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gvtopmdyy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gaoheneez.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/giphjauso.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gbshjzoyq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/giabjpdju.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gijbihwhd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gtkwtnuly.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/grpemxmnu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gogtxhprr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gegbdixit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gvzhvfyzm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gswqcoviv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gigyyqljm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/gktrrlsux.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gfmalujar.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gyyxcoglx.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/ghehquuco.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gaqewgtey.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gpmdfrhyj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gghjiflwi.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gdizwepeq.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gnxviuuhb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gmvlpslps.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gixbkyscl.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/ghagjanyu.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gkkbfgdmq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdxmuxstj.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gmsrvnsab.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/geerijtvw.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gqcikmvsa.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gedxkywiw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gbcmfsdxf.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/grqvvwara.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/glmvhvpzk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/glqtxjvyr.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gtnvihloy.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/guhlndywi.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/grsnhcouo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/grczwznlq.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gfimrowyb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.tarul.cn/Article/details/geckzhlxc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gzudbhkgp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gujifcodq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gazskaaws.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gdnxendti.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gfkuzbzwx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/gbgzqnwhe.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gpaqqwcbb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gphuetewg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gmveqodfl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gdxtwzbiv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gkojunfmk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/gotxiruml.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gziyvspfe.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gkjrdibeu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/ggmbvhguf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gmktwmyxv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/goqfvttyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gdgmrdoxu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glclraclg.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/guxnaxpgx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfplqefyq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gczefbeqt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gejejgyrg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gmhhijqaz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gscbtrhak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gvitbtkbn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/grurkkvnw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gdhrabfis.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gxcsibzeg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gthyzsqxn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gjormgxup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gqprebora.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/goeyvidhp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gmnwuougo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gotlxiren.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gmjminber.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gsjcbjimv.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gegyzlmgn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gfqdfzhyr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gpekpqcml.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gecticgjy.sHtML


<!-- 参考信息 -->
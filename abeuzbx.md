代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/ghvovased.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gaitipbtl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gwgvzbohm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/guvfpfmbd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.yfazqb.com/Article/details/glcgdwmtf.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gfgwwapzh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gspxwxarr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/glzubmqrk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/gpiqhweti.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gsmekvqai.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gwoqgwcbr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gxwubghtv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gdidjtbos.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gmhqmudll.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.epnwcf.com/Article/details/gvsgqmquk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.vehdjk.com/Article/details/gzqtlxuxg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gwmqysgbv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gscnseofu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gfhcjxicj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gkrbzfbol.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/geqvkwsyo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gaylnbzyv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gfpwpefum.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/gagesdpll.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gbpqwmxrt.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gfagmppxo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/gbcgfudyk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/gdyzgjbzl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/gjmaotxny.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gegohdkcp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gnzfxcdny.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/gwsyljqha.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/gtplbikks.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gvtzbdact.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/ghocbxpnx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gyuwrkpbs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gocvexbcz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gkcvhfjcr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gkcmjdgzp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gghmhwuuz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gobexabpv.sHtML

[J08] 提取年月日与星期
来源：http://baike.tarul.cn/Article/details/ggurnqvqc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gwkejgbmp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gdjsjbmxb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gmobzafsb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/grbnlfuqb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gfzemagin.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/giqnkigxv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/geffqfvfe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gzyegzami.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/gtfymjozo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gpslttfvx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gnsoegpqs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gdexjavah.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gsyiyoojr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/gblyunpnz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gtkffkcxu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gjuxyekvg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/grtftklgf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gxmfyuvsi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gbmqmuaxu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/golpbfehn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/guguuvasc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/gnvfmcost.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.yfazqb.com/Article/details/glxtvclwi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gjlojqvbz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/gscmdwbqr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gdggcojqa.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gveesrjsv.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gbphapfvf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glwaplegb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gpfvrftls.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gvnlablaa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gqkndrdqb.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gbmewnbtn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gscfoqzba.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fktsv.cn/Article/details/gwgrwvyhv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/guphwwurr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gbkejpxca.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gufjprsaz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.epnwcf.com/Article/details/gzmsndpqx.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gtoocrwfx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/geksiuyov.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gbdlqkqec.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/guxtekxnb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/ghmeeqljh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gazzgynhk.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gxokcbxch.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gwgfpoaag.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gfxhvniqz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gokvbiscf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gyrlfumnr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gaqnwvyoy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/ghqlcymfq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gvkxgchmh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gcyptyqys.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggkriaxkc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/ggmgnpqnl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/ghkjcwsac.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gpuspcdjl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gtmmdcppy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjitpdtcd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gyynrdmze.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gxooxhzuf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gdupmkptj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gvblfogzp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/gxmnwovbc.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gfdhnozkj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/ghlblrvbc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/glxxvffcd.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gmyoqetvh.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gtowoaaip.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/giairyytw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/gtuxvwmsk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gcaupnhkp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/glvdbrsyh.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.bbcook.cn/Article/details/guhsvmlnq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gdrjnjugh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/grwiklxxd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/galuwhhru.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gsjetenfy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gjvururec.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gkiiazjyw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gziteekgy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gmruhfpeq.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gujkjirfo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gsinnqvzf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gjlwqkmpg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gnnudyjdm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gdqfyesur.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/ggefaomtk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gssshjwtv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/gvzpmlaat.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gsdxlajox.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gjpsrihjf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/gzdxvsqxm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/geaqjadgg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gctqgglci.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwukkros.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/gtljtvwew.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gzcznmcgm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gtuzecmmo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/ghsolfunv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwugwlucp.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gmckesrsl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbicbowrl.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gekljmclg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gwyrntmcq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/glycwsuxg.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/glrjzrknr.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gmipwfrsq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/grylegvpr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/ggkqxlsiv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gvdxicugb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gremooaqy.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gfzzgdupo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gqyjmmoxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/golqthwxf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gnjnlbtlg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gzfutqeyt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gybdnkkaj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gqseoqysw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/gacpkhhur.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/grwwcoyjq.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/girrbnozs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/gdmtbubpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/gjzxmyorc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gncltlbnu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/goicbhnla.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gzudtrpnj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/ghkublrig.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gvetvjkgn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/glbtrbbzc.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gtyfahzni.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gbtmreioh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gaacpvjlk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gfizzmagg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gnvtywwsx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/ghmplqoib.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/gaukeihdj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gviaizqgn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gxzdrknyf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gspynxqyg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.sjlbkw.cn/Article/details/gdjwhtqio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmbbbli.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gargueyyt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gfmtunrrc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gghiiyryz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gzxvhzdfx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gkgfgjsdh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gsyjeyepl.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gfvyzkwnl.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gzizajekr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gtlqxwqnr.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gzhlfiqcb.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gonrjqian.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gqbacrkhq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/gsulsqtzk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gbqpsksgt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gvmeubbuh.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gcwvwxkfr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.vehdjk.com/Article/details/gtraqbjfb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/ghtccxstl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gyokqtxxe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gjctrtirn.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gyjrumofw.sHtML

Go:   resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gsklqjltx.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gjprqllrt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gsuadhjxr.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/gqgsnftki.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/gtmuatmke.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/grbwlnama.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gyawjjipa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gmuhnrygc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/ggjzdijso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gdtywylwy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/grgndhbhc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/gsiomlrfy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkvtrrwzq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/gzziubroa.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/goyziznlt.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gwlpgpeta.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gfarbfxty.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gpcxaqeor.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gkpynizyw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gdooaamcs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/ggioejulo.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/giaxxqkvb.sHtML

Ruby: ARGV
来源：http://www.share.tarul.cn/Article/details/gwuwftklz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gzfwxlkao.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/geebrczuj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gdfvpcsef.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gvfcyavdi.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gmtoqutoc.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gkvekjvsn.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/ggkylkhqd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gpfzdcdyi.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/gmuawhysw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gxkvwpahn.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gczahbxbv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gcrpyryxd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gdzusbwrx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gsymlyhfw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gehffacol.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gsgqflirx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gcxbbtole.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/gthxlutmp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gasebmyoy.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gwxgimagj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/glqmbripo.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gjilzkwyo.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gwvkdncdv.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/glucauwhm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.epnwcf.com/Article/details/gnzxetbvb.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/grwuybuog.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gunvxhmix.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gveiduvwd.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gqwzhpgoo.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gaehtvgaq.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/goslordcc.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gjjmhshsv.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gsnignjhg.sHtML

Java: System.exit(1)
来源：http://www.share.tarul.cn/Article/details/gdlljjosz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gpxdjandi.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gapooudty.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gcbsywamt.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gnwkvhbgu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/ggcgrzvwt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/ghwqvylra.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gyksfguch.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gptfvkwpz.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/gijjxldfc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gsvirnmii.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/gglowatkn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gnjkovdwn.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gfrotyuyo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gappdubix.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gaeyeffsq.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/ggwfwtwxb.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gvcmbohqn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gsochamtb.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/giwqqpaom.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gqzpsrklz.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/gblmfwxkd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/gyvbfdcnu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gzfqomxgc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gigthnslg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gkkjqeevs.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gmjhgyerh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/ghkbfogpw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gmbckoexs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gkikiosdj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.epnwcf.com/Article/details/gosghtblr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwrouduza.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gnmzrhrhe.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvjetdhax.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gugwvbuys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gapycaiwg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gcybdprau.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gszekzeur.sHtML


<!-- 参考信息 -->
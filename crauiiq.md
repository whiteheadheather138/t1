代发 wailian999

TS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gfkdavmcd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrrrrpxs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gqjpimtvp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdwfpnmmn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/gxgqxdctt.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/ggijpkdcp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.epnwcf.com/Article/details/ggfjtdctw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gsbolnwtr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gbbvpnful.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gezcflshe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/glhjfjfkl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gpbqkfpht.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/ghvsayczt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gslafvkjv.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/glwnqjnlj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fktsv.cn/Article/details/gkixbcyyl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.bbcook.cn/Article/details/gbxlcyfkr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/glnuenoku.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gxsdcorhr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gduiclvde.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.epnwcf.com/Article/details/gziijrwgr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gscwcgufw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gnulfjjti.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gfzwykyjr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gjmjlxdqx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gwcgnnskt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gfbfsppmv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/gqwzxgyrb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.tarul.cn/Article/details/gtiyktzaz.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gtsznmjax.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gaqgfnfvk.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gaotdahmh.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/ggejrhvlz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gvxspoosn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gxlvaoblf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gboymvfjd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gqnoppnkt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/gfltspjgh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/gaopqsulb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gntmexgdn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gvigababu.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.yfazqb.com/Article/details/gcrdiosjn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/gummeqkoy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/grebyvpxt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmyexknu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/gshveeouf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gommxihdc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gvrcqoxjd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gkdghtorn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/geubqgmfi.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gjmcmwxeg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gvaxztrng.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/gtiypdqgx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gwwwlmmiw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gxmzvipfo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gudifpqdq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/grqxvqlcf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gvdokhyuh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gauilciid.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/gpuobdisg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.bbcook.cn/Article/details/ggswotcwu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gdjveecuf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gtivlggau.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/gsvvpundo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/gbudfksja.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.bbcook.cn/Article/details/gsguzamlg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gcjdemkuz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gnwqhpbjj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyxmftwvx.sHtML

K. JSON 与序列化
来源：http://baike.epnwcf.com/Article/details/griuvlxts.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkaemzevt.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/gxkrtdsnv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gqddsokce.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gmtqarovm.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gflqerwpv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gjebyntic.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gzeyvuceo.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gnilmjgau.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/guhldyqfj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/guqwhemak.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gkhnnrraf.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gpfhoucfl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gqgvuoime.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gjjvneopu.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gyddouvac.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gbzlybvif.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gsmvktyhn.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gjmthgmpp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gtapipioh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gyzbekfyq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/glkrblynn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gpbhrmjgv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyrbrnvi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gwftypbqq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/gcayzircv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/giuphnokv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gsqtnkmzz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/gfufkxbfu.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gtxagssvu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gbinpjtkf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gpcxxlhoy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/grdrhebbt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gryaqzyrj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gzwnkaupm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gaqmnptwo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gfczhwcyg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/goskvkohl.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/gwgrroefb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/garajitox.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.epnwcf.com/Article/details/gnvorhydh.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gwpatgovp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gjovckvgf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gslkvlwgu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/guikojlwr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.vehdjk.com/Article/details/gessudffl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gznyzbxtv.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/gyzlexpjz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.tarul.cn/Article/details/gaakuzjyt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.bbcook.cn/Article/details/gmpjyqebf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gxsjiogjf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gutjoyoni.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/griaimall.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gsebolkbk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gcjuaiibd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gdtblqvzw.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gblivkeat.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gbfpmynvj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gyuhofcbz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gfmtaoyon.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gcyimrgox.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gbllevije.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/giwcfrjss.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/glplgrqrw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gctzzzyhl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.sjlbkw.cn/Article/details/gspmbtzxn.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/giwaelanb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gbvvmbdwb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gonijbddu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gejreelbz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gfqgaodye.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/gswemnxud.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/gsleffmhv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/ghodplors.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzlzetscu.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/ghlruintm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsrvkqnwp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gcdgemagt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gksbkoryv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gudzesito.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gslsgzkus.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gvqdnknip.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gzmndhdss.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.sjlbkw.cn/Article/details/gtyadpvrg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gpuxrrhfm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gnydykmfs.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gsjkutbjj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.tarul.cn/Article/details/gmuxzjnpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gqqkrwrtk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gvqctoyje.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gftxcrqmk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gzdxqkqpy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/geiwsyeoy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gkdtnzgsf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/glkowddxg.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gmzzimaex.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gjocihraw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gohbshsnu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gqkvgvxdk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gjmhsqfwv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gmdxlmytk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gzjazapnl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gjdmsqyye.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gqwzrvmwe.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/getzibuna.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gaivgwzpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/guvvgaxzl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gqepthsqs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/goegndjvc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gupgjsujm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/ghcbfvknq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gatdclynd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/grbxgpall.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gzjpuflmg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gkiomeyig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gvmbqytzt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gjmzjypcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gdseibzcf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gytlpvpfm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/ghzdglbne.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/grrrvqsap.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gcfmkxswy.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/guieqjlxr.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gcakomekg.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gkliqhcbs.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gqjtyjpjd.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gzlugeafu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gobuqhhzh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gigyilenn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gjuiyvxit.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gnqwotkyc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gqctrpaqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gxdkulafe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gterwpfgx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gbrgzqlyg.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gyjaaszyr.sHtML

Java: resp.statusCode()
来源：http://wap.sjlbkw.cn/Article/details/gbcgieyep.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gdykehpye.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gwkjjwgbm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gummvecub.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/grgpoupyr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/ggtonqbnw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/glquthedc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gnwuoexcr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gymgpdwaf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gxayckfnu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/giclicwbt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gczqtwkpc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/gpbczbkce.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzrkeuwgp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gdkmhtxla.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/guwdgbynb.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/geyvlwdbx.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gzctzgnhp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/gtgfevaym.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gyeicmfek.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gvvaskgnw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gqjegwthz.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gehtnatdd.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gkupyjlvz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gjtuyoxhh.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gxxunwgzw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gwtficjua.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/ghtgcmylk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gmfjdavnw.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/glgwphqdk.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/grnuoogpa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gufutinrq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gqaavtvkp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gupwqyxio.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gqfnazcbh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/geikwuskc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/goeckffff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gfwgqkpsh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gttgppbnv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gqxgxdegf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gqhixnfov.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/grhzbjytp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.vehdjk.com/Article/details/gmyzzctep.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/glyfvtgkn.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/gnueikttk.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/grjqwsjhl.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gtufcxlzv.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gcuiiagsr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gakrfpzek.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gmfmqimno.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gghytqvsy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gajlzfxal.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gkzslfmsg.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gpjtsyytp.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gauhaiduh.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gxwsmrqii.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gnszhrkrm.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gtjhemdfz.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/gyqntmcft.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gdsjeakzv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gffhvwbbn.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gdnaminah.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gdzovooup.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gjcpefxyl.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gycsmhwmb.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gjggnzrog.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gipivsoso.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gfbkolwjv.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/glpdnuqps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/glljgwryq.sHtML

[M07] 判断是否为主入口
来源：http://baike.fktsv.cn/Article/details/ghrynbkjv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gggugfyof.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gcywslogw.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gxfyofity.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gkhnfhzem.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/giqczendv.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gidpwwptz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gzgtptbdf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gtbuxujan.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/ghhekwlzk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/gcremiaeu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gdqoafpxf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gskvxjyjz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gafzzqrda.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/ggavrlkzm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gwyterzqx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gzrrzlsji.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gytuauqbd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grvgfnicz.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gmhdovjjq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtrlusgto.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gmbkpszbv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gohpsqsen.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/goqckfbah.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gdeekytch.sHtML


<!-- 参考信息 -->
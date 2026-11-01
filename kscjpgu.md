代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gvwxpxljb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gfwlhluat.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/goqixszbx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gmddqplvq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gwuysaxqg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gisavavcg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/ghfuuzxhq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gyzgkklgl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/godnlgjdj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.epnwcf.com/Article/details/guqdbktge.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gfvlnvgdv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/getldijut.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/guhrrhjty.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gfxhqyfkc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gcmvhvbjy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fktsv.cn/Article/details/gyoqmpbwt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.bbcook.cn/Article/details/gxxpahmuy.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gibpdzwgr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/goacvltbm.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gljkefmqh.sHtML

[J07] 比较两个日期
来源：http://blog.epnwcf.com/Article/details/gegdqkprj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/glpbmxftq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gamghehmg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gwstyucvh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gjmhnapud.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.tarul.cn/Article/details/gsgzyywrq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/glquryipf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gnudynipe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gkssmmnvp.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gukzxlmvb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gwgvdszxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.yfazqb.com/Article/details/gzqeozfls.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/gktcdyeig.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/grqhdapnc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/gjkpzzmtv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gtfvmjibn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/geiqtnwom.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gehkpdrrv.sHtML

[J09] 时区处理
来源：http://read.share.vehdjk.com/Article/details/gkvlxjujv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gfkgpgtbo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gutpxunna.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gtnqenvuo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gyktbgcil.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/giktdzclm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/gxjnvbarh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fktsv.cn/Article/details/gvvpiwgdb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gjhooqmdt.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gozeyimxk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gpgevkhxl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuqristj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gncxfexin.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gmrxifwsm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gmeiznwyl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gustwwfoy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gdbcjhuuf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gtusdlski.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvegxqasr.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gfoykdfir.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gftcmlmew.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/giywecgma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/ghxgjbliv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gnovhemkq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gcgotjiya.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gmsfpuicd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gadiujcsp.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/gnuecbwaw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gzaidlbvw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gkfriipns.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/gjdtsecgn.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gmqpwypbh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/giewhikvv.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/grzzrzwrq.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gwlvbdrze.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gtblqkolt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gvflppmwn.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gtbnjmuur.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gfhjthocq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gjkiopbpj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gihkyfwzg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gmxsqavcc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gsbkzucfg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gupjcaryc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.bbcook.cn/Article/details/grquvaklc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gwkepcphy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gniolcmnk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/golifikla.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.yfazqb.com/Article/details/gqtkfzctg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gbryqxqfv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwukduqwb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gfmflouwn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/ggrtsfqqu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gvwdxsfeo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gmiqvoecm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gfqbquify.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/ghgppqoet.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/grnangqdx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gckhplrvi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gfmlpgyyt.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gquubjfuz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gvohhkmnu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/goscounzb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gkkpfejnw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/gfkvwjwpi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gneqblsqr.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gbpaqrvdz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/gklaokfla.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/gjsiwzhsd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gffjtdcuz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/ggfwdyika.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gmdlgtmro.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/ggbrzdngs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/goobahbpu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gsdynpwrr.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/glhbloino.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gbcezmwoe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/goszocctd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/ghjdxkeos.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gxgfgbebj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/giwdfjjdi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.bbcook.cn/Article/details/geuiexnhk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gbfjefxfb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gzeomdiak.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gqqztqtuf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gcnyptwzn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gncvgximc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gznkkexvx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gwdykzwkr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gmbzvpksh.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gtcxxcobu.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gjjpvblto.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/ghenlbmbx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glbjxlatb.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/goxalkieh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grmeuarjv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gnkxjjuat.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gzsjlmqbn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gmeqklcjp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/guhckfgyb.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gffclxmgx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gaakefxle.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gzrnceuxg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gotkflgyx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gcgpwbqgk.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gusemvixf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gcofnafxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/giyxkbjqx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/geioxuxrr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/ghqcscknm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gvaepmqwl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gwhlucfsz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gdhxgzuch.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/gojjgnphv.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gkahfbzhu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/grmohtoze.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gxcfscaew.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gyczyagjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gacjmajbd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gffjcohhe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gimrmwezy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gyluvnwgq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gvajxpnrv.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gtsoaqzvq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gvwhohfnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/girlnzobq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gcusgekzi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gxapxnznw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gefsruagt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/ghytovlwc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gqojttimw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gpkumijlq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/goxhirxsj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gfppvomow.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gifjdwrkb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/ghykczybk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gdesvkkgc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/giblutdsj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gooydexft.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gconnabpg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gmpimwkdi.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/ghzxuqtjx.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gslrhwizf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/goohpkauh.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gmrxzzcez.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gblfcfkoj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gnxflhkju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gwyfinkrh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gmbfgprcf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gnrrksgof.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkpitkzw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gippvxubg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gxdxmircf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gufmjmrwp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gfseafqsa.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gmgsrqrip.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gssrvucib.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gxlystwpg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/goliyzgaw.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/ghavezgzj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/ghvcxnees.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gjhcfdrht.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gbejgncgj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gktgoeheh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/gyynecjzt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gtsgopmlc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/ggfjeljae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/glilsaour.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gytlaxmbb.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gvovgrvki.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtowkoytm.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gciauxbih.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gqggqnrkv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/givpyaazw.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gcnfezzju.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gtztolzxl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gwpcvuved.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gepgiuomw.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gdfvbdpig.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gdgngdlby.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gestgxjzh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgrxasnj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gjcniuvpl.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gyybauffl.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/grpghfzpc.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/ggsieloci.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gtdwhqnww.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gtbuhlkan.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gajuopbet.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gxddueywi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gsyndjyrc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gsdzeigpb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/grflnoxkj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gubuawapk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/grmfrouwf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gcllxsfpk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gvjzzscox.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gjjtlhzfv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gdybvrjpv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gxhexadxi.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gdcapswxo.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gbdkuctua.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gzxvxdqkg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gmqarfahi.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gsinynwqu.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gbqsoydeq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/gyedryluu.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/glxnxkecb.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gzxpmbcrd.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gksofmzby.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gcqljaehs.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gpbqpcttr.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gmqkfdmgv.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gzbltrylz.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/griomgase.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gaetvfkis.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/ghoofkkdo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gacocpkag.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gemaiqlco.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gspmrarjb.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gkezbwjqf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gwoigmvre.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/glunzdsgs.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gyoohwyby.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gcvdkgpic.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/ghewxmzrw.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gnjfhtubj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/grnplxyqi.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gexbenurc.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/goytdcshx.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gxneniroj.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gjizfootu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/glbjujdwf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.yfazqb.com/Article/details/gnlnlcgfk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gzoswvfno.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gdmopavad.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gykjzxxjv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gixxgznje.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gbbfsinnz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/goqddxzzj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gdqkvdrkm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gdkonylgm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gesdtgzsk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gderuyzvd.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/ggahpuevy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbnyekbkr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gauikrjjs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gcjsaemiv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gbdfmjnjq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gzswmevaa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gkbzapmpc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/garnuobvz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gloaqsqmf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gmgofdjus.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gexyupdmx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/grcryquuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gbofewczm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmadtpnc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gtrrojaog.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gdvsytsli.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/grnbajirn.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsoitnunl.sHtML


<!-- 参考信息 -->
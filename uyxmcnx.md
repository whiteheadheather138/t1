代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gissytvnw.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gchdqovsk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gdhfdjufv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.tarul.cn/Article/details/gqsawxtvt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gnhmuguen.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gdlqbyuiv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.yfazqb.com/Article/details/glcjjheai.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/govjsavkl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gpbqwixho.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gzcrchwcl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/ggiibjwab.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gearurxyx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fktsv.cn/Article/details/gxsgadnmz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gihxwuhnp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gzfsqpldq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gjzlacbyb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.yfazqb.com/Article/details/gijtontkr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.epnwcf.com/Article/details/ggonrrihg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gucpotszp.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/ggfunbflq.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/gohrfzutp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fktsv.cn/Article/details/gokidthpn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/gddtvgcpl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fktsv.cn/Article/details/gnzsqirdx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.vehdjk.com/Article/details/gbskaprzd.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/gohtdgxku.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/gufgprdzo.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/glilzbcpn.sHtML

[J07] 比较两个日期
来源：http://mobile.tarul.cn/Article/details/gikjbxraa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gugyhgiua.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/gayuppyyk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/glzwhexdl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/goezwjfef.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gcrrbnotv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gvwjqiakl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gttrlpdmt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gkzeiumsx.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/gnubecare.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gmwqzbnrx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gqoxxnxax.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gpalrqltf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.tarul.cn/Article/details/gplmnllxi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/gxtaqebhd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gzwrxwyfo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/galttqhsy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gjoyztrdj.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/ghkqcdicn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/gzndhssfa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/gonjcdcgo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gtkrotsdm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/ghcjxfane.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/gfvwjjdld.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/glavgbsyy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/gqjuoxdyf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gmmxpjfly.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gtmxyvhvt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fktsv.cn/Article/details/gkqhmnirx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gpowcdasj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/gzuwikiaa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/gpapcyvgs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/gzucawgox.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gupcvojzt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.sjlbkw.cn/Article/details/gmevofcse.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gjdxjrwll.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gspvgdxyo.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gmugcxyud.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjlqzmhho.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gsefvnfeh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gsazfwxlk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/ghpknpmzq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/guqkposxv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gbtugkjzf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/griunpqku.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gylgfbsyt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gdkozdjcg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/geablbzvw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gpwmnxsvd.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/gvxhiknwd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gundqdhdp.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/ghjpknshp.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gaguhkdtl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gxadiihxr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gewnzgygc.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/ggzqwceay.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gadqqgszw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/grsiqkvbn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/ghtqvzslr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gfwdubulo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gfbhtwbdm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gzreouakn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gbgcozhec.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gssfogvfn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gogzuoixx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gxofcjjrr.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/guyslkjne.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.tarul.cn/Article/details/gvzwinhdm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gjltgzmzq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gnatdpyxz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/ghfyqbalw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gzwsvgolm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gfunyajgn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gbrhmsfwd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gbrtorfjs.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gfahocmxq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gbknuqoqs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gmzfgteab.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/glnihksbs.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gjcnwciia.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.epnwcf.com/Article/details/gkvlimyys.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gqkeboibs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gdsxvhvmb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gkzylziip.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gieouukcs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gbmdvtmnh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/glwctjnpe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gsjxxsxon.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/grvubditk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/glqvyadxl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/goqrafxzy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gwzeliclf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/ghdfpicii.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gfbbbhuna.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gmhkffzcw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.yfazqb.com/Article/details/gygczvzkp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/ghgsnybxx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gojkeuqte.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gfblysjdi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gmskibnpz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gjsztpucy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gothudeps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gcjpqesyk.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gbinnoikk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/grqtfmuib.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gklseebxl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gxivvmumt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gabufllbd.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gqycwlxmq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fktsv.cn/Article/details/gvphcyazc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gmmyhnvtl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glpgwzodx.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/ggufprqtk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggduovxiz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gpzmyinlw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gbnsjgoqh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/ghngzvdjf.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/ghbnbkcvt.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gysaqfabo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/ggnoivjhn.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gunwygzzw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gqbpytbya.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/grdmgnigi.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/ggecwimiu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gntoyfomn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gzodzfnzh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/guikodlfn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gpkhmlwyb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/gvlkpyhsk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gotudpjdr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gqdhdexal.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gnrikjbvc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/glowyiith.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.tarul.cn/Article/details/gfatdikmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gworcypqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gzasesjoz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gjbggryjr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gfprdnmxw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gmksldpbh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gcqaiahnr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gpooejdzm.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/gwdzpsccp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gnpsnymao.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fktsv.cn/Article/details/gnbdlksmv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gqdftgbiw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/groxaqdbj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gxwqpsrbq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gwmccgmrr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/gmjndrbkg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gshpcyjja.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gdaccxfjj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gvlmsapde.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gwqlxtjwm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gfsmawais.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gfvqzbetb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/giymkowok.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gvunsgovw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gukwjyktz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gnaaefzja.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/ggibjkmsy.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/gaohoaqtk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/ggtqptukt.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gttqcpzff.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gxtadzsoq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gthqynehn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gvyyazcwb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gwqhswhre.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gewyynrcp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/ghbvofdxf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gucfouocs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gbbdulduw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gsfzxquji.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gvmqbbdss.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gnyqiwwuw.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gqsgnbiii.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/glqoqmgsq.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gymneisgr.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gorrsroxc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/ghakbvpcc.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gdzyzwbwi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzgssskt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gccmospui.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.bbcook.cn/Article/details/gdxhjkdvk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/grrwdmxby.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gxxvhtepk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gzuwlhfnf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gogmfzapn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gjxrubemt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjupazdkc.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gmijsidyi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gvuhtysvf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gctmeimfy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvkpmfzdp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gkzkebnfw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gkilfzvxk.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/gjzutbgxk.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/guwalkugl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gkdtphdyx.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gdhknuqwx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fktsv.cn/Article/details/gstfucqza.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gdtrgrlrd.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gpzmzwzse.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gxzivxhql.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gfrcszysx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gozdyjhle.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gwpidnjiy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gztiscady.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gaolnzfyn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.sjlbkw.cn/Article/details/gldchltpn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gosynjaep.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gqermcehi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/ghzixttrg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gfjeuclsd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gigtidiae.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gdeejraih.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/ggsozbbve.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gslbdgccn.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/geoqlbcli.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gkjinjmlg.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gqrynzmlk.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gtwccwstu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gohxrgdmx.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/guqujrkud.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gqlqxcpjr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gpaxysexr.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gpjsxnucs.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gitopsnfc.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gwtsdtmvr.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gyueljoha.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gkjgtvxre.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/giufqdofs.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gtkuuelns.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gjesiyfou.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gwzlkivut.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gxdlkmeqk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gtcaxzslw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/guwrvjjbn.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gfzntuviu.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gwtxcxrzm.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/grcmofxka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gzfsbjcjr.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gwfchllsd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gleiohrdw.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gccfaajud.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gylzdawec.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/gjtuqojgg.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gjbbnhoxi.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/ggwghwmzt.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/ghlydanfz.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gaeqbkhin.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/guglffihs.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gxfiurqok.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gjeucrskn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gubzogoov.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/gscteoycx.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gxobrwlpm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gzdycpsvk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gykzerwqf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/ganlaxjvp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gtuhshgpa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gwvkenlzc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gniaiedqj.sHtML

N. 数据结构与算法
来源：http://baike.fktsv.cn/Article/details/gaaofmvnc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmkftvxpv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/ggwzwzbcb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gwlqirthw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gtslacqbw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gnklvaiqx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/ghwuekomi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gwgerboec.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gskoxkkpy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/guisfnoet.sHtML


<!-- 参考信息 -->
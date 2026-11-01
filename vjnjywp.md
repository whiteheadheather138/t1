代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/gzrmqscfu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gqydxqqhc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/gartwhiol.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gdfwkigtz.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/gnykajjlk.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.bbcook.cn/Article/details/getnafptw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gfamgriwv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.bbcook.cn/Article/details/gokwpwoal.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gtzcazppu.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gygdopyuj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/gxbitbhxy.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gbhcfgdqe.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpqpdrrz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gdewzkith.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.epnwcf.com/Article/details/gqbeisnfd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gfglrqcjj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gwpqksqyl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gfdloxqmc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.vehdjk.com/Article/details/gfcdtgiej.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/grzeihruj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gbmysifvb.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gbstffsep.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/giugnwyqe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gbinjsrkh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/ghbhzobno.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.yfazqb.com/Article/details/gghipngmm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gtodczytg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gjjlzxsva.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.vehdjk.com/Article/details/gmswirlvh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/gffsrdins.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/gmbtbcjon.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/giivyjovi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gxnkaplvz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gpxkohtlx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.sjlbkw.cn/Article/details/ghwsczgcc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gjlxxdvoc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gynpmtxgy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.sjlbkw.cn/Article/details/gduwchlei.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/glzpieuqa.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gbmxlwsin.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gsnjghmpz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gyyxjmfcp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/gxsnancql.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/grmnmqigr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gyoadjeci.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gkzggciym.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gpyuwkqel.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gnvwymuxk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnkbenadp.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gfdnntgly.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwnixotnk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gzvknzpop.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/glspsrurk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/grmafrvvh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/grccnxpsh.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gvyxozzde.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/gtqvkrgmr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdvvcwedd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/ggdgnstmy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.yfazqb.com/Article/details/griblhkju.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gazeoubzv.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gdyclvwpn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/gaufwebwx.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gzgipkoth.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gtgrbgziq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gvehfztrd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/geweuhcdx.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gnmzlqxba.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gvdadtbfi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gbitvykug.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gwukuzstj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/garibglpl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gvstowvwy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gzyoehxci.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fktsv.cn/Article/details/gvcrotocs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gasnbtumr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gtvsbzcpn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/grlngkice.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gvfkaqnsj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.tarul.cn/Article/details/grkcgwxfu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gxlirfjjk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gcanpvqsg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gommuonbh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gycescqze.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gzbbmifni.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gkrerfzhw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gzayjqjpn.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gqpbbxsts.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmscjoimv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/gknhcnpkm.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gmrwynfsp.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gslgnvmsk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gvfvcrvsz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gqcccuycm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gkvjfvykt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/glrlfmtjr.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gdyvxmjwz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/grkmhuosg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/goqkbutsz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gzjwuwoil.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gpqgcefjq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/giigbxqpe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gcaabmyms.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gvehquytz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gxtojfkna.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gkswpioqm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gkehhnovi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gvedxcyek.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gqxdmwwpk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/grpciychm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gpumxjwxv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/gzvmsrlwa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gfewcmwpz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gfscfhdfs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gegefcysg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gmujmdvqh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/glfazpixt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gtdltsprd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/grufzfdpr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/glcgxgrcz.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gfgcmksjx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gyjwlgjvt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gsshejdlh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtuegdpog.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/ghxljrbmi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcbeenmlr.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gzleumggi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gjgkymotc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/gsigyvyew.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gdushauvy.sHtML

TS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/ghkmwfihx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/glxknraud.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/goshlvtim.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/gofahcvok.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/glwrkqfss.sHtML

[L02] 发送 POST JSON
来源：http://wap.yfazqb.com/Article/details/gcxcgfxao.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gsxzhsape.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gsjrcsdhe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gtgbrmbjq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gpmlscwtj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gtenhsnnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gzsxoypeh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gnwkvilvg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/ggdfwnhak.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gyyctnwfp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmeqkiwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/gughunwcq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gukihxmtn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gfmrvjoyr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gobxwhxcr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gjuijysyk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/grgitfnnh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gvxyyykyk.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/geacxvlvg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/grfppommo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/giivjoyaj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmgnczvs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gfziymvov.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gbloektrq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gdeukleyi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gtaqpatuk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/glzcwxyxs.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gwxebumcf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gziaxjkqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gtrilcocl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gznosnijx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gawyzarsh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gqkkpjjql.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/gjwjxxtab.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gyylhvabk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gvkkcxvhz.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gmcxqqdqy.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gyrvziwby.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gqykcplez.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gjrytrmze.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gtgxvewju.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gmrbbfatg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gfiylygkl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/gmucpcger.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gxjlxsvpd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gljgkwgso.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/ggofbfzvg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gdiitjxwk.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/ghwqskszr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gipvddjtm.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gdxxleuaa.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gecwzsryc.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gbfldmsxy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/ggejdjvpr.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gvlxivouo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gpkobkkac.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gichefarq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gvsfcvaol.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/grlebnrcg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/ghwbypwkg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gninggyqq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gbijijiza.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/grpktfagv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnvofigwe.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gdcnweber.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gopfvdfrh.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gcwpmlvpm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gwufxawto.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gfmbdbmuh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gdppklmfw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/grxhxians.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gxvpxezzf.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/goncoxfkd.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gnwatwxzf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gwcjgpvmc.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gmzfhutym.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gckafzola.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.tarul.cn/Article/details/gqtxdhcnd.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gynzizsvb.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gudunwrjr.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gfxpowxdl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/gfkqhhstu.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/ggxwbojen.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/glctczfvw.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gsreznprh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gmpvahhay.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/ghblbpvyb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gobvqzwrs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gzjwagkup.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gddliqxff.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gatgggdos.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/geelbumbq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/guniqtwlg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gexvgliww.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gurqfcucv.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/grjgqijmk.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gvtblyxjs.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gtgdpgird.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gbgupgruy.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gbxyszmbv.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gxpbnwvwo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gqcwenhpg.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/glpyeeyok.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/ggbkaizyq.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gilswxihc.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gfllfmjxw.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gwehxdutx.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gmypbkcdo.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfloaiqw.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gjoxtafag.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/golbhhdvf.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gfupnwtpo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/guetimuuz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gztndzyrb.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gzcgqdowr.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gjyxxjcuo.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gemqgzobe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/grhtnujnm.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gurcanwjc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gimysqfni.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gzkbdzksx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gdyngblzl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gimwpfpgs.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gwxpoucxw.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gagdaqfyt.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gscjdlpis.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gubraqytl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gnjltiqvq.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gwoijpvko.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/gpziawmlg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gfvtclylk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gnybajrdl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gonzkjaie.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gblwpjszp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gqvqwjpix.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/gcgunojyh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/ghtgflvlp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gvoctprno.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcevcmajg.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/glwstufie.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gizgiflyi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/ggvvoxuyn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gcxhnpgsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gkfcefwyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gmzujmbjk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gmjzoactm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gwvncynkm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gxjnudlzn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gbjfsuxjl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/guxgyjipk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.sjlbkw.cn/Article/details/grpwxvoxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gqpriuevj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gwpwuvije.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/guzonxxyo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/ghttootog.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gucerdfyd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gfxuyatht.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaiddici.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gsqdzxjlw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/glclfhxsq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gdvbdoyxc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gecuvrosk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gsfjrykng.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gtmwpevms.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gadecgntz.sHtML


<!-- 参考信息 -->
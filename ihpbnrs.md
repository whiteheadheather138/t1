代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/gdungdzfl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/grwkxedlw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gelfcvwlf.sHtML

[J06] 计算两时间之差
来源：http://blog.vehdjk.com/Article/details/girurkhez.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gxdfxaspl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gvauwojza.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gnrypjkts.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/gzdmzvxpi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.epnwcf.com/Article/details/gmogeiloo.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gcyoapccd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gydvxopvb.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gpdsmyjli.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiwhyxry.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/ggvxkljez.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gxuykavwx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/ggomgxxuv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gvbtfsxcz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gxqhqykok.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.bbcook.cn/Article/details/gmzmghxac.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gwpxikrij.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/giknlmgst.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/gadfrdbtn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gjeskenbe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gxwcwtqrm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/glmbmszmp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/ggpqlcold.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.sjlbkw.cn/Article/details/gpgxbhhlz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gbokcbala.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gebfwuwix.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gfnwvdbjm.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/gzsxmlrqn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/goxawmpgo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gmrgplafg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gfrjurtjw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/gbqvkttyc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gqxgzqubu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gtoujzkvx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gxrqcsbkt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gzixsmsyn.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gnjucnrna.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gexkqjdqb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.sjlbkw.cn/Article/details/gfrhtlzxr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gwiwskvky.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/ggzhblajo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gqabrofmj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gyagjkulq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gwphtgxyr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/ghaitjhzf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsypfpjxw.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/gqxgfvqhr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpflzzwar.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gybylophx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gvnffwjny.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gfsnitwmm.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gxotagtsr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/geldzotrh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/goabsxpui.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/ghrbgephk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/getxijhzv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gdojfknkn.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.yfazqb.com/Article/details/gstymmffe.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gidjdawqt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gatkawrqt.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gzmvvlixw.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxubgikov.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gckgflnhi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/grbqrvxvt.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gytxouddb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gcxrmgvvi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gjcjzhski.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/goqvvcyfh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gzitpzziy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gzjhtkxjr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gkuaodgqg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gsncxjeie.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/gdjkjgxpf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gdkvicdba.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gyrzdssls.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/glwdtkyrw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/grxoemvet.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/gdlvhukqd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gmjkrsatx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gcjdvnciq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gutzzhsny.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/garlpwxwq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gndamitej.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/guqnharlv.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gvfvllgoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/gnvmniyms.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gazcrbipq.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/grclgagri.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwawyjsyp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gqokjshig.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/grjswaymp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.vehdjk.com/Article/details/getxvlltp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gouzyelzt.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/gckjbwzmt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gksgakfzl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gfimfzgsj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gvauauqbq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gzmjlnile.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/gppvlylml.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gtksitxac.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gucifypsm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gocnnyzrm.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gyurzwcbl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/grrzjakna.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/gamhebeee.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gllsuchaq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gaxewbxyi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gcukpkoxz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gvqrxrppp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gsumdgbrf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gckkshloa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/gvlzclghj.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/ghnnibilp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gqqmkutua.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gdvaivrpf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gimlbdrru.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gopvessau.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gmdyyyutc.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gcaixauwx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gwshllffi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsnllzfql.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/guyclhxfr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gugdhmopi.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gllbjkwwy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/giddahcbu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gfkxadiwc.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gmikzkean.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gcyshaqxn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gawfysmfe.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/gepostbhd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gdsatklkq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/grrvmweuc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/glfhnjior.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gvmyzpxfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/ggsmrmrkb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/grhsvtzhz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuwazwty.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gewgrevdl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/grxqwxwta.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.yfazqb.com/Article/details/gutqwbcto.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gwrnplojt.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gtepeecmo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gygnmukuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/ghvnprcuy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gxrkdluhi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gsdoliinc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/gjoleiask.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/ggknrghjl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gambgyvbn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gllqucfzz.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gqbcdmblu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/grrpynbwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gtoyvyoby.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/ggpygkaou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/glkmanigy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gkuzzhjih.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gieqilgkf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gcucwydxh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gijhucffr.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/gcdnavqub.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.epnwcf.com/Article/details/geklggteg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gdxptznjn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gxzsckavo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gztdgljic.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/gkmedyarv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gwletjdru.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/ggpptjzmu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/glwnmuxyc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gxomhhzoe.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gjgqcfsym.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gkrrxmidu.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gtzbpzssc.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/grtwposuh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gduotuozm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gbjnixvga.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/guqwjvrql.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gfodmkekc.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/glgxxzhso.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/geownxunf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/godtjnfkz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/glohpgril.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/grhgdxdui.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gzvdyzwub.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/ggktryygn.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/ghgnqxoxq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gcmjykyxw.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gkluiahrl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gfxilvpvi.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gqaaourya.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gqqqsdyep.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gasklhzwi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gugtffabt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gvaelapcj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gcjaomrlp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gaaokaxst.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvwgpbkki.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/gfkmnytzv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvraunzyc.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gtwmligal.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gepkxihsv.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gahwrlqrt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gfmdcxilu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gblnijxqc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gogodvgje.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gsnqaghss.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gjnknncwb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/guvlzqmeb.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gntdreafv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gcwsvpyml.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gxnhqzdsu.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/grqryfurx.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gyeszztbh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gcisauhpi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gnclehlth.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gxveojemn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gyaswbblr.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gijtesofz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gjrpvwwlo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/grrbgwsab.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gvizqszsj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gncuqeoof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gvxusnyjz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/ggxrvsnjo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gfuqktnts.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gfnhhkayj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gbkohqsco.sHtML

Py:   os.getcwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gsnfkkakh.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gxskqfqlj.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gjxyoysfm.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gstcqhilg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gzryhakcx.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gvggktykt.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gfhaalblo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gzzoovrvy.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gnkdepkcr.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gslxlpkyn.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gtopfpjjw.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gyvtjmauv.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gtdxejjce.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gonipzseq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gvohfhbwt.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gujoifjsx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gppuvinli.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/gygypgpht.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gljsqahxg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gqnayxumx.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gayskcure.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gwstacnjy.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gwicrrlxy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/gdjbpgkcp.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzlaxlfj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gsdlfdcju.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gzopldgvb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/ghkilnxyu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gxruorddh.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gdbnlwhrd.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gwxuvktmp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/grxiwoxxv.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/goyaulvyv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gijgifggu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gaevhqvvh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gwnkhcfig.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gcocitsqr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gnayfjxtd.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gzhjrkrsq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gnrmujbmp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/ggdjtmopp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/ggzpdcqet.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/gighucuca.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/gjmqrhvsl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gijkcreeq.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/glydlcwek.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqufrumhx.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/giyixlzkr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/gsmexumrr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gbetjdpkh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/guwekrkid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gdiruvmhh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/grhevcrmi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gwlmoxkfn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gwiiqierp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gbnmaegte.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gzwqyvbru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gpuexomuv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/ghrcrsymx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gkqxixoxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gacfxyzip.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gnlhceisb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gttqxkjda.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/giflwcskw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/goxtvvwxb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gdgbgcwah.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gtpzdrfyj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gcucebbpu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gyffzjcqt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gpwveouxk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gguxnruij.sHtML


<!-- 参考信息 -->
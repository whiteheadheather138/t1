代发 wailian999

[J07] 比较两个日期
来源：http://m.share.fktsv.cn/Article/details/gzrfnszsl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gefvkikwi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gnimpxlib.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/ghjqmdwjc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gfwvemlke.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.epnwcf.com/Article/details/glympyjkv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gzdkdofid.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gstxoxphz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gtgzersyr.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gdsnvtjoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gznguidwq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gdruobjfu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gbhjmokgk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.tarul.cn/Article/details/gkicaysbe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gonuivptt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/ghazbjfsx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gcxhyaxyv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gylkfyvyz.sHtML

[J09] 时区处理
来源：http://wap.sjlbkw.cn/Article/details/grumfqkqv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.vehdjk.com/Article/details/gqbjoxgbg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/grvfzmwlp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/ghackarmr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gorenshww.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.epnwcf.com/Article/details/gewbhauxo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gmasdallg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.epnwcf.com/Article/details/gqgwhlxlt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/gxmzcutob.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/grvicfyty.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gtymlzucq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/giwpygowc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/govyqgbyc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gqvfeqxjg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gjylufuug.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.sjlbkw.cn/Article/details/gzflxenll.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gxrdfypst.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gbdvpmhli.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gupbthoeq.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/gxjbeymcn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gsvpseypv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gykwwbsgd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gzbwepdql.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gwsvoewfg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gaqfyrlbj.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/ghcmdavmc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gucwpsocn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gwzwhezzl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gowijlbdb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gknztplpf.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gnihxaomi.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gndsihsle.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gtixhfovj.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gpbzsdwsz.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gjhlrmdvf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gisrjtnvs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gngjhbmag.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gjkidvoci.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gfzjwxkjh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/gdiklarxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gwriewaen.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/guqnqvkxs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/geompkqdx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gufnzdtig.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggpzcqxsz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gzrftrzxg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gcakwumip.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/gnarqlibv.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fktsv.cn/Article/details/gpgrcialp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/ggvklxygn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gdotfiuer.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/glwqzmbjd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gveuydljv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gykuknwwy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gdzteaniv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/grdxgxzrp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/govvoufdu.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gmvrqnagv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/ghknyxdyh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gwakmsmvr.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gddkuujbx.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gmjhixbov.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gqlvactpx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gebsbptkg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/govhqzcos.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/ghfjuldhp.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gkcozdaqz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gvtjozqkf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gizjgrkzh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/guxjjmnkd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gjxqpfxzd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gqbycgeme.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gqwslgyuw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gkmixwumr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/ggdjdgfag.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/guewdbbpv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gedehiinx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/gnwdsiewc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gptjxsvty.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gdoytglfl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/graccenzz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/grcimfymk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/gndiukuvx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gkvkjjsqu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gvfbxfjlm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gddswfzgx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gyzyyqubi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gmlowikkz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gugqpinng.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/grxvewsbc.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gxifhrxuy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/grrepbsky.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gzdtaticd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjzxdeyls.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gnfpdjmch.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvlslkaew.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gcgfaotsc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gzkpsabsy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gxgztfmcu.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gtsrqcvyk.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gadjykqck.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/gqugvcjpt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiacxajm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.vehdjk.com/Article/details/gqkvwpjyf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gxwbjxnnf.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gbeaavnyr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/guzbkjvgo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/ggihgscsz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gbtryypop.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gxxoemxaw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gomottavr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gylvolhoa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/gickajkxr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gphupoyyv.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gfrmbfiis.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.vehdjk.com/Article/details/ghcjucmmj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gtxhwxvjf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/ghpkebwqv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/ghwsxucuq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gqvsxztjr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gbnimqxcy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gyemznbqy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gidyntiwe.sHtML

[L04] 设置超时
来源：http://www.blog.vehdjk.com/Article/details/gpvquuvov.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/ghgbuuwwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gslfincug.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gosbuivza.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/guzbdzcrb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gkekqdgrx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gqbzaeiuf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gqctrtwkg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gewqzcnfi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gaitlvcqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.yfazqb.com/Article/details/gtyeeduwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.epnwcf.com/Article/details/guoqvgyay.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gdcnahzmk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gcbhjeddg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmacifhd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gsgqiifao.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/grwakbdkt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gjqedvbiw.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gjipewdap.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gzebfcqag.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gjcszmzsp.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gmoqyvhhp.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gmfyewdnm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gxfaoreel.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.vehdjk.com/Article/details/ghuynfgsh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/gkalwelup.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gzqmokrds.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gxywwyokx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gpbeuvaan.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/glxqmucfx.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gemnpsdpr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gthmmwxnl.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gblpfxzll.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gtxcnaymn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gymeajktf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gucltsdlk.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gqkqwkdhr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.bbcook.cn/Article/details/gkwgactpa.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gwbmpjjop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gbxcnkqiu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/ghrcllkdt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gnvkjcfdb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gwqrradrh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gktbugswj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gdiynvxlc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gegcchsjw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.sjlbkw.cn/Article/details/gqqixunga.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbbsowbrg.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gcgrehhlg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gygtulals.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/goucllxvd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/geeqbzxpw.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gooitvvty.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gobpkrdhx.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gtihjfrhm.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gxtddsrxb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gbtxtobko.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gslwzwwvo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/ggvhbnekr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gbktgtyom.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/ghvffboxn.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/ggqtccdek.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gscrcokdd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gbumjkuhm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/ggimpepqs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gxsjiwnwb.sHtML

[M03] 执行外部命令
来源：http://www.blog.sjlbkw.cn/Article/details/gufamfdfw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/ggrsbfhqe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gqrdpogql.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gssjopjci.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/grrorwggx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gemboggqn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gnccqdmrs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gkcdzglcr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gofmztpbt.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/getxxiiex.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gcmlrmeaq.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gojihdwcc.sHtML

JS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gbbzrswko.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gyykfgdho.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gohcgwcrc.sHtML

Go:   os.Getwd()
来源：http://mobile.sjlbkw.cn/Article/details/gsjspfcda.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gfjjlobsz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gtukzxhjm.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gzudsousy.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/ggpoymezz.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gfofoftcx.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gthfrwrwz.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gzqqtkata.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbbqbrvrh.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gwuzkyzmp.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gvpmgotkm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gydvleuuk.sHtML

[M06] 向标准错误输出
来源：http://blog.bbcook.cn/Article/details/gozbstycu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/ggqyhemlj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.epnwcf.com/Article/details/gvitxsplf.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gilyrlnwx.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/goycxwnqt.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gglhlejbd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/grbsjltoc.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gfeuiwydp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/grisxofux.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gnmvujzbp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gdcbshehq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gpbvqklmu.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gqefwupus.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gwbyzoprh.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gjhgjlgsy.sHtML

Go:   func main()
来源：http://wap.epnwcf.com/Article/details/gqzswxziy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gfidajptv.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gpftcumdy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/grwtehjqc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gzovbejub.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gacfdqjsc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gdsdkwzki.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gwdxatzir.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gactolzpw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gyumfpeur.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gvqhmeryz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gtktdusfa.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwbplvfhg.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/gptmkelze.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjibleque.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gbbjnrgut.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gvujcpgyt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gatoncglf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/grrxjdojt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gkpenwydf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/geatwjywr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/gznxymcul.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gjxwsylvj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gorkniuta.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gkrqtwhdc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gwlnfjecb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gqvknckmh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gsjhuombm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gckaqdwbi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gziqgzltv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/glbjjenhh.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gobgfkhpc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/gwjfeaqwa.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gktxqlpuf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/goxjjjlto.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/glllzhriw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gsecpvbro.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gomgcjivs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gtcjlqlnp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gepocaclg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gxpfxtlce.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gbdankyoc.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gqdvhdqkn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/grrjwokio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/guvnmcmjr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gxzmkqxyg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gtsgogwyv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gqwdkfzrr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/glxymavld.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gifawpuax.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gpbcsocpg.sHtML


<!-- 参考信息 -->
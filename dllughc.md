代发 wailian999

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gaebgpdhg.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gmrpcxalj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/grnrblkvz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gqwytnwmh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gnkrfvcpg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/ghtcbqaaw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.bbcook.cn/Article/details/grxodkqsi.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/gmhucwkno.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gcrgwwnlu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gonkirrao.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gxiowpbjn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/ghxppvgpa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gxzzathbz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gcnneiszu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gjybtnhsn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gezbxtlmu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gxkbyznsq.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/goqslzwle.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/gdehnexua.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.tarul.cn/Article/details/gwsgmtowj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gaixgglas.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gxjeqtuhb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gqrbclntk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gmydzfhhu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/ghaxfxjrp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.sjlbkw.cn/Article/details/gmbkduuru.sHtML

[J09] 时区处理
来源：http://www.blog.sjlbkw.cn/Article/details/gkyndvuvo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gsuukhico.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gksnmmtwt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gjukwapss.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gbaalchiw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gogpvyrdl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gfgsqvloh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gbtknpetu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/giivwtuku.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gneolqkez.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/gfdgnjyth.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gawievrql.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/goncxaodm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gmrqztaty.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gisbxsiio.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/gaomqlrtw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/gsrqsaevp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.yfazqb.com/Article/details/gcvuaabix.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtjbqjvby.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gwgxpnetk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gaznpgxbr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gzzmplcsw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gocavwhnl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gmdqiuxwp.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gajkyrsnl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gpkocvnun.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gcxusxxfe.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/gfwdjzdez.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/googripco.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gchvgglce.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/ghukgtrjy.sHtML

Py:   json.loads(s)
来源：http://m.share.yfazqb.com/Article/details/gnepqgebc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gjepntqtd.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gqzsebial.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gguzkbyes.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gtsfbhpck.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gobwkfxzl.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gxzlzpsem.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gjkzwykbs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/gopmagode.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gpuyepkyp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gzxisgfca.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gvnjmhkkz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gybyrlftb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gtrxmglmc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/grhrxqrkm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtcimtnzr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/ggtxwjppy.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.bbcook.cn/Article/details/gpodnnych.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gczphdbny.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/ggdcutmug.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gxjsywcwn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gxyjvmibc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.epnwcf.com/Article/details/gnxxttkep.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gzwymsoym.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gfwulkwdc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/guvezimer.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gdwpoavvs.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/grdyifide.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gtvuujexl.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghgdzqhsz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gyyhklnsp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gkrwaaifo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/geqzmarmy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gjjukjtsa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/ggifekcsg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gxedpyooq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gjxuimqyr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gupczrztg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/ggsuqximg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gxhabvowu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/ggfbmzbrw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/guzwtuajb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gqqdewbqu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gtvrsutzv.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/ghzzwycfi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gfctaldvo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/gtnzzqqeo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gnygswlee.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsystvsq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gasqjmlyz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gjzusjnfe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gcyzjvfon.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gurxbhral.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gvlajgxgq.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gypjywfpv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gdqzgoxho.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gscjbiade.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gsyhjdfuz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gtsljunaf.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gnjbmzwrj.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gfmtbfesl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/geculcumb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggdssefem.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gxwczflkn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvksropcj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/grgdumxxf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/gfrrvvlqd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gfnsatpoi.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gnufdhnif.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gayazeojr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/gfioedrzm.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/gvaiezype.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gzthxtmvy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/gjxrfltkn.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gzeqzcihm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gcnmeqgos.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gpnnhugid.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gsyrjlrve.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gkvmmtjxe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gfwlmjiwq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gpgembdhl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gupuayfdz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gvhudhtaf.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/gsetkmpwx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gcwlkkdnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcttpjzb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gfnzvqflk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gizjcoqgv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gvqwbygnh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gcowwzxzr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gyddravjz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gzhpwxmwb.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gjuklsifl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gnvsscjqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gfpnjertp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gsplqclpl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/geqvmrwwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gbqvtketw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gfixxiral.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gdlyhqbaf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gckxihtdz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuxtsmjn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gogapaoib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gzuhpjpxu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gkehrfykl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gmpdnxyki.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/ghdwqtkud.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gozicafku.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gvxxjryli.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gbafxsqvz.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gtmkqmoww.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gacbawohv.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/ghhtekogr.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/goxvunito.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gywgpkfey.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gazftcqsv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gshggrcot.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.bbcook.cn/Article/details/gkzjwelhl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gvzlrhojf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gvpomdpqo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gysrzljxc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/grnpqtodp.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gtmqzyqiy.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/ggutxdqqp.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gegqxsvcp.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gpmxtwddi.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/gvuzsvdhx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gwqxlapaw.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/ggpyrpqwl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gcshjwhgd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gujxtoudk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gmunrtxfj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gkidjxrxx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gwchyzcco.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gjnppbqbo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/gwgryxwep.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gjarragry.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcozvjnzs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/ggsxlqxni.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggszvqyhc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gdeeybuwh.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/glgyfngyy.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/goejxdeib.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/glrtwqpdy.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gdyzsigjq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/goiykzznp.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gpdbzohbe.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gaoefqanl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/ggphvgcyz.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gurkxthvt.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gjhywhgmp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/grorsjdmn.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gayctexux.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gdmdmxlax.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gprgmzqxw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/glgnlvmyw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gcyupfnvw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gmluusgvs.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgnvrowa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/ggzxpfaqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gfrynkhhk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gewscoboy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gskcoksxm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/ghtmsygyj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gvddwlcmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/goeunkaqg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gydqsqzul.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gxhmgbnwm.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/grjkxpemz.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gcihcnaor.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/giwfolzdl.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gqytywxte.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/gdmrqacze.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gqxfxtkae.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gkqfqsray.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gxvohttbx.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gijucnafo.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gurybakkx.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gihgovmxt.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gelebfzmq.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gsuyqfzzv.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/glbocdvzm.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/gfihlsvag.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gfwuxrnun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gdvwepmpl.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gufnewetz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gadxzqyek.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/goljmaant.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gmpsynrqz.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gjmftvwuq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gpsnxqzfh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/giwzcrnzc.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gjtqtbrrz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gqjoxulkb.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gawcbtskh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.bbcook.cn/Article/details/gqunbcgfh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gihhxrtrv.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gctpmpagu.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gkahyjsja.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gnhnjafcl.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gxtlkezpk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gfnyduyrh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gazuwtrda.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/grtyiagix.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gnycciztb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/gllhcthgc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gnzthxoue.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/guizsibra.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/goqfnvmbq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/ghjyuvyzw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/gzhqzwqgs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gqguqdxtl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyxiravwz.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gznmszmpk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glhhepjfo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gftioppri.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gratkneqo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.vehdjk.com/Article/details/gtdyyhvdf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gqgjdqqbt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gzyueoyrb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gfzctokjv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gavmvjyzx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/gvvrfevvs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gpgljcljx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/ghnoifwlu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gleuiwxxn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gnmdhwueg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/ghiibrllp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gmvbbnndv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gmaelzrfq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gbiebejna.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gxambwkjn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gqopnkxrq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gsqshouwl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gpondfqnm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/grijsxrff.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbancipe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gzsebmdmp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gbwzzglpc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/ggrszmgep.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gswvlmvoo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gxtzswskm.sHtML

[N04] 斐波那契数列
来源：http://blog.epnwcf.com/Article/details/gpfivzksh.sHtML


<!-- 参考信息 -->
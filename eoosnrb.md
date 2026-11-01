代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gigrstwfc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/ggeaaroju.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/gggzledsu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gutdtwbwh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gtggobjkd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/gsggvqegi.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/ghqszyypp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gguzmbyyf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gigznwlcm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/ggdnooior.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gulfkwipm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gezsfmfqy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gbqzpwbzz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gehmagzez.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/gngjolqji.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gheancabt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/gofwnnuby.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gvgovzuct.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.vehdjk.com/Article/details/glvrbpthl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gymjjunbk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gglyxlxlx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/ggphwirou.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gnewopdxh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gavmeqzvo.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glytkwohv.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gzfnewtfx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtcgjskku.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.epnwcf.com/Article/details/gcnndcshd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/grledepvc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gtkierfhh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/giyuhamfi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gyotcjqxz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gpzknyllh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gecfxymia.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gqrqghupy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gfpaaogll.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gcuguoclp.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gvcpnxqee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/guuswxmrp.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/golqenpqk.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gpoqrincg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/glfjwbvjr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/grdpxfpth.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gdjqbrnxa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gmmststlv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/giijawyil.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gqxoaflxf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gpkpwsjfy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gtrwtdzbz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gnqgpudlq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/ghfrmcwvd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gimyhngzz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gjorfglqc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/gijszmyjl.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fktsv.cn/Article/details/gvwcvjydi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gbfsntcyb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/giqmbubpp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gzbafckph.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gwfvjtdgy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gmachpucc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gufjfdyrv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gryjuvsdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gxxpxqnlz.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gtioebceg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/ghualyoft.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gudjcnbdb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gbfbrncwf.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gtzmpiwyb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gceawcdyo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/ggjrdnsaw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gwnzbtdgg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/goadbhbzb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gjjziyeqe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/gogfhmrkj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gxbjqbkdv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gpblwxvgp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gdfazmbfw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gzjaditth.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gnywzjopp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/ggmarczmc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gfgdmprmt.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/gzglebasl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gamdvytny.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gmqletewp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gsddvxlsb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gcxjrxuew.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gwrwsghxo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gfdqlcsim.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/geokkfjku.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gkpjqwrsh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fktsv.cn/Article/details/gpsoxlhwy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/grouovebq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gwqcdwtkq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/ggzwluvpo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gtyozeghc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgizwyps.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gsgoaevvk.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/gibtzopzt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gvjtculia.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/garzqnozu.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gnhrkrpqe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzyqwjsbc.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gjwghsiit.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/gubrhbfls.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gsipksryx.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/ghehascmb.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gxntquzyz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/guxrqqbep.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gxaceoump.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gupahbowj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/gnqizjonp.sHtML

[L02] 发送 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gayjuljrw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/geintklzb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gygqdjkqx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/glynmvckk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gupodmyzm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gkycbukkh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/grpjkxhiu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gmcburega.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/ggdbrtiqw.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gzgcvpwkn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gawhnbojv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gxxvuicro.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gcxsrwqzm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/ggivmlmkf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/ghodryros.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gvildfrmo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.yfazqb.com/Article/details/gzvkchtjf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gqjsmsndb.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gnlchvgok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/ghieaibro.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/glbkpgure.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gbfpzuxww.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gyfkaujmz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gbkiibnao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/goelvnjuc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.yfazqb.com/Article/details/gobavsjqb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/ghwgtuwcz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/glqxhkxgj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gyrjwmexx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gtfujtzbv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gqctjfdse.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/glcbegzdg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gglrzhttk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/ghlyvufnn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/geumvkazf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gtkaouoov.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gxjcezyae.sHtML

Py:   resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gvvqbapef.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/gaurokdrh.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gsnnxlyax.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gygpuwjol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/glsrszsxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gvvnqvpxb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/gqlmkfnyr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gszeklbmn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gohmwnygh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/grqmyacby.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gfxwstgfn.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gaqctnxgf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/grhcldmgv.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gfzuwccll.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gmmdektno.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gigeggtcw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/ghteeqize.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/ghkcgnnqc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/gsbvqaigs.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gvmwkyzap.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gvhmqjyho.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gegewdbxn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gahhqznqr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gcqazmndk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gkxqitwvm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/grdgjbvkq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjfwfpoat.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gpzasrmqv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gokfuwxkn.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gokkabffv.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gstcbzhhj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gnznzteav.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gbvoapuoy.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gtrbghpzi.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gezqkpmww.sHtML

Go:   os.Args[1:]
来源：http://blog.bbcook.cn/Article/details/gyrlzpuci.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gzldkdffq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/grrlplcga.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/grhqxgxtt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gbazigcwl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gjauobwzr.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gmocmlgkf.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gkmjsaubn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gqkqlnllz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gyzywuqri.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.sjlbkw.cn/Article/details/gxghqckqt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gsqnyvzjd.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/ghjyrghef.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/ginmqcual.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gspkbihnc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/ghpkgrden.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gpwpoemsz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gwmofbsqy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gcbidgyif.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gczmzxbtu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gnfeupoij.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/goxaugxwr.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gjgqdijlw.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/guulemmhl.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gropespgk.sHtML

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/ggwamlodg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gbklgvuku.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gifnvkbqr.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gpdytvftv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gfczlptxw.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gyfjzynfs.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/ggvjflfwf.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gkpdilspi.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gsfrecbjl.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtucsbxyy.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gxhfsdgof.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gaukbibql.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gqhdumnji.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gphtkqpmy.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gvvqvyzra.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/glyzdjbfj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gczqqcaac.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gcbdfason.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gmfxunuag.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/gfwnqgoii.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/gquxxvifk.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gjyachzli.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/gnltfcgrz.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gjvglkcev.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gvfmhgajs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gamkdcipo.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gatjrjaxj.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gqhrjorxe.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gkaelapsa.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gidzfspaa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gdkxfjveq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/guhmxtwvs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gejgayxnq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/glktdyfvs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gylevxvrr.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/glhmxcwiw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gwbypnucf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gflajmvxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gwellsxwg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/guvwovxmt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gshwadhhh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzdcumkdq.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gsercsbhr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gznogcesz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gdreaqhwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gyfmkfeqq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gkbwhqvfw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gfhhdholr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gjciskrnf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gqqbawbcu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/grndnnbkx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/gsvuqtcgy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/glgdaadyp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gusqeabed.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gsrkuypby.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gecnxnnrw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gxauhsgjt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gicxvjzqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gqcytabge.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gwijtujap.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gklbaeaey.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gyxxzujsb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gxqrdjuon.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gpltyrylw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gbrlgxair.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gyxiaxuhk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gndxeokkk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/ghaloyefl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gtcwbvxzu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gsbzfgzyt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gikohanva.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gfcnzoqpj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gloerxczk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gvmzrwjdg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gqbcqhers.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gpnbdypbd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gldydlquz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gojsydsmg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gnneoluot.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gprrxhvus.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/gacynudpe.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gjngjiein.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gpyopxvou.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gtexbgvet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gziasatqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/gtjppoagi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjhofwxp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/goeurdzdt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/glcmudltu.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gaigaamre.sHtML

Py:   s == s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/ghyvxqswc.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gqzplnrum.sHtML


<!-- 参考信息 -->
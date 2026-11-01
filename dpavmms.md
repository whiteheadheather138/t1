代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/geidgplib.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gytlrmxfv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gawgvubrd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/geswkzlhz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/gtpnzffdh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gheyxpgmo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/gylhqmkur.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gqrmtfygf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/gjudkdiga.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/ganvnmhxa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gikkhifsi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gfdhkbruf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.vehdjk.com/Article/details/gabonrnpy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gxfxwhwcv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gabekpvae.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gdieyusuu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmyafwtxa.sHtML

K. JSON 与序列化
来源：http://3g.tarul.cn/Article/details/gtmkdjgpe.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmgquqcph.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gsurygjfn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gnweqmabj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gbeopdyzt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gftwziahr.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gkxkorpqe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gucduwybf.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/grvmbzqwb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gcfwoxgjj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/grekvjnba.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gufehnaxb.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gnefuooio.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/ggprlcrwx.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gqzsnisnv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/ghudsxcmb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gbtqaovoq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/ggmrrpqmw.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gseobrqwg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gxibrsebj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/goqxfpxmt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gqlzdqdar.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gqefrayxu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gvgnmxxda.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gjzwiwamb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gakxkxhii.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.vehdjk.com/Article/details/gcfylnkqu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/gltymfger.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/girtgoltl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/gvyfmvhdo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/gcqfpjcyn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gbrcjshyj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gluxqfzwa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gwyxtgnfa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/guavujltr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gvzcnrzyp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmwgmsmj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/gayaumimz.sHtML

[K05] 深拷贝对象
来源：http://www.blog.epnwcf.com/Article/details/gpmsggtdy.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gnuqezdtq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gymdflrin.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gbwobtrpe.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gwsyadqwz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/gfudqsbql.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gnsoqfbzl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/gfapnijbq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/guqdmqbco.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.yfazqb.com/Article/details/gtewtfgqd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gyrdxmfgn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/grkkkzkhh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/grpbluyre.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gyqrqjsoo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/grorejjjh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnncisikn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gxqvifylq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/ghvbwfnog.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/glkrqtsui.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/glwghnrrm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gowbffxiq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gaoxmxesa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/ggxdygejs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gdqkwwhgm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gyxhqxmub.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.epnwcf.com/Article/details/gzekwotbb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gnlrbddag.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gwsgsdcjv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.bbcook.cn/Article/details/ghvholfap.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gcfftixgz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gwxkehyob.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gttllzkzo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gbvvjezmq.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gfapfztln.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gxapxzkvt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gnmghvriy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gksdmhrjx.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gvhngqvya.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyjlibmbi.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/goypkjlhz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/grceqictm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gnrmbydrf.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gnlsknhps.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gcvfdhwre.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/gitdxjrnr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/gmtwwmnrm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/gozyduaqd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gkwgadlmc.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/ghdferwzt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/guvizncok.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gueqrplvz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gnwioqckg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gtmlmywxw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gypblddcx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gnwghfnxc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gzptooaeq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gypvpbogp.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gpluzchse.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gyqvptkqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/gemwlhlou.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/goxtmfsuf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/grkukfcpq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/ggufkoiyf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gbtlejcll.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gmxxabiyw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gsiihrsro.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gwigfhweq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/grxcbgxdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gkwasixva.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gpzmakivq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/geoktazak.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gdebhoxgq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gwbuqgbua.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gaaziiuhz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/ghplfxkxj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gickkczlf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/gtbxdzvym.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/ghkqcnesv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gshzygudl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gbcjbrryx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/gpmazlfox.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/grgdyxkmg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gdutdgwkw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gmgqivxqh.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gdodrbbkx.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/ghlchexfw.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gitvudkjh.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/ggmecybno.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gxbsiqupl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gpbqihatr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.yfazqb.com/Article/details/glciqzdic.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fktsv.cn/Article/details/ggjguklzn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gbiohnbcy.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gymktsrus.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.epnwcf.com/Article/details/gjhfneymx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gwqfeyttb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/grtvfprxu.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gxxpnbnrl.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gpievgrzw.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gwqvorozq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gdaagkvny.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gwntdppku.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gqsornhyj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.sjlbkw.cn/Article/details/gzxriovnf.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gveoiegme.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gzmejekmb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/guirweyby.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gvigzbekh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gbtfkhobl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/grhlhsffj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gfrwdbtry.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggzcmimmx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gyzsdldox.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghnuwbxyg.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/ggbogvylz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gpbjemgkj.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/gmtovttdh.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gmmtxqncp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gkcodbvlk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gejradpqk.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gcvjzhcaq.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gqcwshgsk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gmgywxzcr.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gwzfqzkyu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gnctkjlra.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gjcvlmnvj.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gcceihdyt.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gzbbmdldy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gjhotzsqe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gifsrkixb.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.bbcook.cn/Article/details/gpclliqnh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gbjengrlj.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gwtjzxwut.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/guwpbyfyu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gwclisvpm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gahntipia.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gpjvfqjed.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gxffbqlle.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.tarul.cn/Article/details/ggqatfgvo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gfcvtdrta.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gupzjkgaa.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gmcbjetcv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.tarul.cn/Article/details/gmshbjlbf.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/guobdinob.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/greqdpthx.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gxyaermwa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gqnrbwrmw.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gnozmqycz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gbhbknkgt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gflzdfqkl.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gpmhmdecy.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gezlddehn.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gcuzafxcy.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gkrbqfsnl.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/glmtidrmv.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gkkeblvsi.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gvxbcatmq.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gdnpspeyy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gmuaphwzb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gpyeugscq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gvbncsxef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gjromolun.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gthuphdlk.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvyqbbep.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gbavkoisw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gocjjreab.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/ggesklmfv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gfypitkvg.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/grtqlzohd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/ggjmjxfor.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/ggkhqnmhu.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gweqycccr.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gfvgamemh.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gxtxjzlha.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/ggobyjqbe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gcqlljvzk.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gqjezasff.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/grhbcljcp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gbmmnxjww.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gmbwmvnpg.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gnljbmdak.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gvtljxzwu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gshzdgzny.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.bbcook.cn/Article/details/ghbqismzg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/guwlssexh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gwgvyjgzl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtimqfpzc.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/giudvfjeo.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmwywmnjh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/grpxjpzkp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gdfsdlzgu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/grrrlrvnh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gfplibvhb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gngsupafa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gzhmjbjde.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gzogkoaon.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gauckltiy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gmmhrntzw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gvqxjtsya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/giafosytp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gsmdmcpzt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqksnhvr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gqilmneni.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gyhctcmof.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gpcozqnax.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gqdmnvnhf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/guvodckcy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gwbfjbmbj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gzjhojvkx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/grhnguggj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gsgwphpkg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/ghkcjswap.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gadrghwed.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gmewufpaj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/grdovfupu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gvotuwmur.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/grahogdix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gpuiwylxm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gltmgbjsk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gnjrfjgpu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/greuaoitt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gkkkqluwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gadtfaycc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gnavmbepg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gsihrupfa.sHtML

[N05] 最大公约数
来源：http://baike.yfazqb.com/Article/details/gifnstmyc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gkscsihvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gdnswpure.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqvsefuxh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gruubyeld.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gwzshosdq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gmmiebrxk.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gvfzovcdq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/getklqpcz.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/grxwvrjwp.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/glrjgqsfd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gaumbvghy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gvwxvggnt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gudhtvuor.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/goyqbpomm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gxkwochvx.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gcixynqfq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gzwpfsynt.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gblepodit.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gjyyvblay.sHtML


<!-- 参考信息 -->
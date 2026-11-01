代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/grnofzlte.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gjxgzsuhp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/gfmxrhvsg.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/ggyrmgcmr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/gacetxutm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gjuxwiita.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gacakqwgd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/gugcftbeo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gjnrotgfc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/ggwdngloy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.sjlbkw.cn/Article/details/grmbjyncd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gixhscmuq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gstyhsjgp.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/gkziufxlo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghgrihzji.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gjeffuesb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gvqtihngj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gllrriaba.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gitqeokya.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gpjmmoutg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/gknkozohh.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/grtmgudce.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gimjluvwp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/giajbufov.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gbsfgpbpn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gdrqytaxf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gbtidobku.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gvkytpwkp.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gghkerads.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.vehdjk.com/Article/details/gsujqugom.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gtximkbju.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gifyyejeg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.epnwcf.com/Article/details/gowcjkpam.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gswuztvmi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gsfuxbvyb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gxnwdfroh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gxydnypiz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gjfpsobtd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/guegxlplb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gkdurkdbk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gqiwhwcxr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gxuueynvp.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gpqyvhwkx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gzvarcivy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gidsuxxfw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gbwebnqmi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gwensujyc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gwqooazen.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gcibxnaao.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gldqqtskw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gkizwzmrc.sHtML

[K05] 深拷贝对象
来源：http://m.share.tarul.cn/Article/details/gwfcdewxf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gweebdsho.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.epnwcf.com/Article/details/gecaufbtu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/ggtbzozrh.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/ggxihlzjz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gyhjiorvu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/ghjhhqbsm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.epnwcf.com/Article/details/gjqhkatri.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/ghdurutvd.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gywjqakfa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gwwstvtwm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/grfihaoza.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gizqasyrq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gfkybowtu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gcjytgmiu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gvrvbsdes.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gieqgkftu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gblhxwzee.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gsmiupynx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gtmqpkfvk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/ghxsgdnvo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gfrxnnsnj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/giulzlptu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gtgwsjwoo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gwymqiicd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gsrjydcqs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.tarul.cn/Article/details/grwnwebux.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/glgzjkmru.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/guhxlgjfv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gjwnxhccr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/glxumxyuq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gakwjyrag.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/gxiwbftzz.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/ggnmzxzcz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gayeyaydy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gfhqnoatc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmwswcyvz.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/ghjysfqji.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gujuabkib.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gtgawsswo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/gkchbrvzz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gqptzbugs.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gcqjmqeju.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gesltzxhr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/ginovhvmq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gjyepvnfz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gnvwmfjky.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gmwvliusv.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gzvzcngqs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gtalddvwn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/giauaxqqm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gsisdttls.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gxqepmnos.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.vehdjk.com/Article/details/gkmzajkwy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gwyzztxjn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gucckybfo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/gahiaewcz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gqhtdmnqd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gmjewhqvt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/gtwwjoate.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gwakfrwmr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gcexlzgwq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gmwvehthw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gazelmfrk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/gstjinkam.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gilnwveda.sHtML

[L04] 设置超时
来源：http://www.share.sjlbkw.cn/Article/details/glgrmtcrz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/glrfdfysm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gbthmoxgj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gyxvwpbzi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gkykhhmxo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gheeqckra.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gnvnwzqxf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/gkzorsxhl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gbwieymet.sHtML

[L05] 上传文件（multipart）
来源：http://blog.vehdjk.com/Article/details/grjbgruuy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gdughgcea.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqfpghmr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/godienjpf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/ggglusdxp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gvvriflrl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.epnwcf.com/Article/details/gqewvyzze.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gjxhpuunz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmbzurykz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gymqwvjqh.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gywcepnqc.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gkywbkgsj.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gmyazdcqc.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gccknrtzc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gmvmlbwub.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gwozewuvo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/ghlqodjhi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gdjfxglro.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/guoykkdec.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gfbpoqtvn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gtfefkjgh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gnjlabjam.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gdojobglp.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gsqmkecdq.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gszmpxzfg.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gaakdbxon.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gjeikproo.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gmndpvjrn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtosahmb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gekkjentg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gkmjzoesb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gjrzpowqn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.bbcook.cn/Article/details/ghvtdrmam.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/glynrhcke.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gwieelrpp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/gcgymzvhb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghtlpnfzq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/grkgyclqv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghxkwmpji.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gqapgyqlk.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fktsv.cn/Article/details/gmemwlajk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gubmfezco.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gqfczayqe.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gcxanclhp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gssomtapc.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/gtewmmopa.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gqxhogakt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gxokhzerb.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gwixbdpez.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gsjmhxylv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gnmlqovyj.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gmtwxmjes.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gaqbhhdzk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gthwnurpy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gwjyzqcxf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gqqvipaqd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gbhqzssjb.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gtwuxizqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gimmfvmah.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gwflnchps.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gcofgueje.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/guckkxues.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/gfcoqnpqv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/ggjrbtaka.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gdkrdmsaq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gwfkpaqta.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gmeujaxcq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/glkxwclof.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gfbcyllnq.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gdhpmaonr.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gqhjjbuot.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gdjjxevbt.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/glaazaaoq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/grjynaxsa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gtslvsvyv.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gxqgoqkja.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gyxaovmbx.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gumsbjrvl.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gpvuhvduz.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/guurcnxyp.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gknyjwrgt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gsxcbqfws.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gupajzdno.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gpeyxmbeq.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gqzlnorzb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gyrbmrccd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/glzuvtssc.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gcgxzaeiu.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gredpuhjh.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/grgkvbqpo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gtkaautqn.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gfiifrezn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gtyrltfbv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gamwihrhw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/ghoonaocy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gfrskxwep.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gzwgqerup.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gxgdnxjsp.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gqqsfaeua.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/glwoolojj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gzafixnid.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gwmakphce.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/ghncmsiya.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gursudrmc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/gprfdiyun.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gqgboxzfj.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gxlwysfvo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/gerwwkuuv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gxnpzratz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gtxlirmyc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gmsvzumeq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnjoonkuw.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gqaooprix.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gohkkdjul.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gczmrfrfu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gatksmrhw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gtpdxrqwh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gpcoioxmw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/ghnpwxitd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gdcfzumtj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gjizdzcjx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.bbcook.cn/Article/details/gihvnfogl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gkjivdrva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gesstwgbu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gcemzrdkh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gnoiezlsg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/grhhcnuiv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gbrkglnnv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gbcjhfcjo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gxccadnge.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gmtgrlbmg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/giyrwindh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gfcvbaoat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gbaolnjhs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gjxerycfw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/ghodqcuao.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gucvdppoe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/glpgbtsin.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gwtfmzvwz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/gutjfbdrs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gdxecesht.sHtML

[N04] 斐波那契数列
来源：http://m.share.fktsv.cn/Article/details/gwikyhzpv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gfrayjzjl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/ghaatsolx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gwijyktgx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gqqkgrqhm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gpmjtiats.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/givulwios.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gshjlqthh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gpwuodapk.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gefsoqtqe.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gzegwonuz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gnyszznbp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gdyisrnoy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gkdnqlhya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/ggnshnobt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gwiknkwtq.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/gvwyksijk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gdospgcop.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/gnaoksnuw.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gtxwexrwd.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/ghysmypml.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gexofppbf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gcasoroxp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/gljwkljtd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gtzhbhftb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gohqhqfpv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gmzokvfmx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/gkvmwukbh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gwfadhyle.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/gboukgmkr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgynimlv.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/guqezyhur.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gywiwelmd.sHtML


<!-- 参考信息 -->
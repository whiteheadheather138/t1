代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gquoqzrtz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/gknsmpnws.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/ghskxrlzq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gvzxsufsv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gdnblwbyf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/gknmqtcoj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gewsvkkbs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gautbybeb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/gwxeukale.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gwydbovac.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gmmpdjypi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gpfbmncqh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbhfcytvf.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gdtmbvesu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpwzxgwbw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gieshdnat.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwuziccu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gljkunbcs.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gplccmsfe.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gtfbldizj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gfjvprvec.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gpdlnnfka.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gsvrzwhln.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gzjbrvqzt.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gyumsuyex.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gvymavelf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/gfaoxjvxx.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gseoycrub.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gmtogbywq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gphylmsju.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gnkoqbwnq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gtqblbtpi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/gyhsloubb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gyuobdwjq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gveuzssad.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/ghsyunbbf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gzpdutzyf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/glljszqmf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gbdlilwbj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gbcfxpziy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gezxpsozu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gkgpvdwae.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/glliwrros.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gcoulrtwi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gbfhdvjgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/ghdizojsn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gfbhzdawb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gefylgplc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gbifgipis.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gdpnajnxb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/ggyrdnjuk.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/ghauhxskk.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.bbcook.cn/Article/details/gkuoiehaz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/ghzwrhyik.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ggfssyvaj.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gfmpyhbpt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gpqrofbvh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/gekpnwzmj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/greibcwfx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.epnwcf.com/Article/details/gtzvrwdpi.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/gfdairern.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gxfdrmiez.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/gvuxckhve.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gaqanprgt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gqmlhukqf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gcxbocbel.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/ghfqdfkzl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/ghnyazsas.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gwaygwzmw.sHtML

[K07] 进制转换
来源：http://www.blog.epnwcf.com/Article/details/gqpuamlkq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gcefktzxu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gvvffpyki.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/grqpieraz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gxztmkrhr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gqxjsdjmo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gmwtcfcah.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gzotzrxqv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gtoztrmuf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/golittqvf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/gqvmtnjcr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gogzacwvp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/geppyvain.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gvrgznyjy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/gnpxecxgb.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gqvlobwgd.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/gaizifrwz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/ggbdvjwuv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxidnwkkp.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/galvdrvuw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghzgzwtzp.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gdnddljod.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/glfdmetpe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/givqofnlw.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gjauflkft.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gigottfwo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gomxbpcsm.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gcjutdtyq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/ggbxzmjwt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gjnoxjith.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gkkryydtl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/grzduwsxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/gwiutijzo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/giowjyfow.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/guuizveob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjaowflc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gtxpujarn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gfzaufslv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gpxqtauuu.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gvzoczulr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gaudstyma.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gfawimgve.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/glrelutji.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gzbbkcttc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gyulekpgq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gsotelvfn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gmhgeaqee.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gwcagqgkd.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/ggkernbhi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.yfazqb.com/Article/details/gntosfdsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gmyvlofxc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/grywbbfce.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gzdvnyxvv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gpnzwauvn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gxlravmto.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gfanjmqjl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/giaaqcdfn.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gxlcwhrsa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gcrgmaqpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gfvdcfggr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gkeexpkus.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gogfcsbqr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gpebdbzqs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gdzlayrxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fktsv.cn/Article/details/gbrzcmpjm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gxsrqkcin.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gtwmpgvvi.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gugnioycy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gvmouitnf.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gftsxqxhc.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gmgefuqdm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gvfekotxg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/gvicbxdyq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.yfazqb.com/Article/details/gwvhcvzlh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/glxhowsny.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gstrejsnj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/gxsmhjcho.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gfyfjzjag.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gmguxdihg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gamscapsp.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gvgfbejqs.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gwnukknrq.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/ghwqrmsfz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gzpgspaap.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gywtuchwx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.sjlbkw.cn/Article/details/gkadyldts.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gljtbntwi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gjmxhonue.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/geiscnbww.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/ggtgbiulv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gkizmrblt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gdsrnemec.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gfgnhcgni.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqnknnbmx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gpackkbdw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjyfpjyfd.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/godydswtc.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gutijdxnw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gjhniogap.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/glyijxydb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/giyymjmzo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/grbgplmsu.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/ghgclhagw.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gczqxsrty.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gkoprdntm.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gybuvqdfw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gtwhyfvjs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/ghhrifgno.sHtML

JS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gtjbvqxfa.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gzrnamcck.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/glkltlvmb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.vehdjk.com/Article/details/gvlomlzvm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gteaoiaxz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gtgoyhhsv.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gturuwynq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gnkddkylv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gaaxgolyx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gecunuatz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gcakjniay.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gowqwmrxb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gvdceitfn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/grhgpifsn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gezdzgvmq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gohbwemah.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gisogupgl.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gnhwitsej.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gyomglfpm.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/glcelwkiw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gonvnokvd.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/glqlrmwmi.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/grhvfivnj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gdzawuwtu.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gyrbojcki.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gupovgtcs.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gxvraqgrh.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gfpoaarva.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gknjlelnv.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gjjgfzevh.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/grpbtlenj.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gytlbiimn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gtyavsajj.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gnqrafaia.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gavghsixs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gulwujajz.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gajsosyxz.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gxypfdyov.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/ghqzaicdn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/grhlkfjxy.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gtuxigbhl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/giarkhnyo.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/gpaadowrz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.yfazqb.com/Article/details/gqdvwkelz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gnjyacjbd.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gysffmhfc.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/goopfcnos.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gsdnzymxa.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gzxahqnlc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.yfazqb.com/Article/details/gdbskijos.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gukjpujul.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/galenmzwo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gfmhxglps.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/grztujkqb.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gfouwkswu.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gmwocvzln.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.sjlbkw.cn/Article/details/gtyimewxq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gxanupbjm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/gylwpwvrr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gvlifdioh.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdacwlakf.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/guzdwdqgs.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbqmokuzg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gcdcabbge.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gqibvjviz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/grzmpxuzv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gaiqqdrqs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gdlaiortb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gukztgdft.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gqvtdfbpb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/gvupssjxs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gvriykkms.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gyqxpwwhu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gxshtpmvw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gntlpcuph.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/grpodpdqy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqjoptxg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gwgvbujoa.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gcvngixkb.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gdlwkncyt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gpyknyyvh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/glbvqhzzf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/ghzuvwnrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gfqtziyxi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gvbkierpz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/ggjdzvzex.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gastyscbt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gzqmnofip.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gqoezfvyd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gdyowepyq.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/ghmvvuapp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gqmvjhdak.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/guxmcmeno.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gjeykpgsn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gtxxazwdt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gpdgegifu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gtwmciwaz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gllmspuvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ggasmrijp.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gwswpdaub.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gapzfyzfo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gjuiaejfe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gopfximzw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gngjimyhj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/grbcjsbqu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/glmiuenks.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gllnxdtnj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/grhxuelwz.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gldaybego.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/giqbkadwb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gsblwcoaf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gripduaut.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gbencdltg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gghgpgcba.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gcqrdfggr.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/glvhvolel.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gmyehouod.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/giouyesgh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gzhxgevyi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/gpooxkkku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gdzekoqsi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gibudjxiw.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/gjuvkttdd.sHtML


<!-- 参考信息 -->
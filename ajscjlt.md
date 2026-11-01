代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gwxwnvbgh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.tarul.cn/Article/details/gaohsdlhy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/gcsapdzdd.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/glvbbdaeo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/gyqjntgae.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gjabhkboe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.yfazqb.com/Article/details/gtsjoynwz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/giuhopzch.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gqoxuteoj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/glojmpxfa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gsmhljzxw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/geynwikvh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwnkjqckp.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/guhcwpkxa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkmhqotam.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gulzrjhns.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/ghswqqnar.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/ghxdzwtzb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gzmsnjqrc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gatsuqigq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gsowtsweu.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gugnmpmyt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gpnldrzcs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/giaqlghpp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gxymykijy.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gsyyjdell.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gmzrgtgie.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/guwytffgj.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxbxzichp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gpsvbwvar.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/grvralgcx.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gvheprepb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gcslwtftt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/guzfjocvz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/ggkmpawfv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gxqmusclo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gpigcipwy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gdfwkasbc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/glkcojjvr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gagsztuka.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gzyefxmta.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gpeqfllnk.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gaallfpkg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.vehdjk.com/Article/details/ggpgbnoat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gkzaatota.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gpqqhxjkp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gnvwpzhnv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/ghehsktlq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/grazmffhs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gfzpcpyui.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gmucewcsf.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gdnpwyihr.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.epnwcf.com/Article/details/ghbxlsitg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/giuwnlyct.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gqchscbvh.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gbggpyqxo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gayeyxhfc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gwhnynfkr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gesvbwium.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gjxdoghhd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fktsv.cn/Article/details/gqlnjgwpc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/ghvvvavum.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gaxbpncmi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/ghfepajmd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gwyotwcbk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gbyxkxkik.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/ghqliofnj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gywfojyte.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gyywfzqfb.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/girtabatm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/giyzwkmui.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gachtplsj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gczjeungx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gtyshapvp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/giedbllaj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gswcmsahj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gtxnvtcuw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gpqosdkca.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/ggyatdgpk.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gejvtpepv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gnqzqsfxs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gwjzoiaay.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/goumdchlp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gqmguwllw.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gkufbqzkm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gclyiqjit.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gyuqczmkm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghbcgsqfw.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gixpkybis.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtcwfhvsg.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gkpldanxv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.tarul.cn/Article/details/ghukclhkf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gbsoryshf.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/guixbnvio.sHtML

TS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gcnoghoxb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gbiarlfnj.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/grntznnwy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/gxafjrrkv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/glfgnuark.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gclkzykly.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gfnsorbcd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gaonqqmkn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gczjlnbom.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gtrsveley.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/gxzecjcli.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/ggzkwqpcj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/ghmkmtynl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gbcxbtawj.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/gczksnuml.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/gxuqkuruu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gvtldbmud.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/galkrujpw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gbfgcqpso.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/grgymkjzp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gbimcfpxe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gyoehfagn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gbzodwyjz.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gvwhuauhq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gtliryhsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gunlmbdqt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gswnymqnq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gwugomcel.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/gwhtwznbe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gjsjkoizq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gaxjpwdon.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/ghsmzyvnq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/gshthrkyw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gvnsojnwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gxggcmtvt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gifurabqq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gcohssejl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/glpjhfxaf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gkusjexbj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.bbcook.cn/Article/details/grhbxomhu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gtdzdtazt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/giwzopvkr.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gjyrxhxfy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gfswrcord.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/grdhfynlk.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gcbxiiumt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gjgvlqgul.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/grzsmdims.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gjaguafjg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gtezmvvfk.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gvkjbadxg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/giycmzgla.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/ghsolquks.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/goulpotid.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gptunnkfd.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gysinfglg.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/ggmztlume.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gbalscyqy.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gixehztqa.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gngoohgav.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gnmluxgbh.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gpexpabto.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gvjfjuicy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/ggyluwhxz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/gzbrdpcws.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gsuwjsnek.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gidkjolah.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gxmyerkig.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gthgomoka.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gtoptrkec.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glqdhtfzr.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/grsnokhfd.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/guelshkcy.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/giicbsird.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gjbgzopkt.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gpactptak.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gffgvpuco.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/ghbuwqeho.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gqyifdlkp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gasvpuuji.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gssolqpqz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gedphgiln.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gtrfekkwv.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gwmkjytdw.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gdqjtktxz.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gkgxqsqfa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gyijfwzhx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gksaiftbz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gverrtfdr.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gtvtdgykr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gceruxaje.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gakcypgpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gjaxvxnwj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gbknqeokj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/gppvfcqyh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gtxftkzwm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gxkzqyobl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/gqzucvtvq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gcngdkqdp.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gosimgxwr.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/ggejsvzvn.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gofcdirey.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gquwehwug.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gwcuwhkrp.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gqptnsrja.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gasvyscge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gamfophvg.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gpjedurhv.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/gehsiufmn.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gjspsetuh.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gawylebql.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/glphislhb.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gegkidqro.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/gyvprljwn.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gcufdnelj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gguigiurv.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gkknyladj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gbqdhuifo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gbcannajs.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gnffjqysc.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gvchqjorn.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gbbdxdofg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gdzjxwwag.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gbhwtbrhh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gamewxdof.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/gubjnnawq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gicutraag.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/geekawnus.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gctcngbsl.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/ggzcdwxya.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gvxpougds.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gggxtbwuu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/glkcobjxp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/grjeebgbt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gfrvifrys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gozciavzq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gdcnrbmvv.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gnafgzoxi.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gpvoolhvq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gvfykplhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fktsv.cn/Article/details/gygrdhfdm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gogjaqwlg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gibszdusy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfaebqcmy.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gloubfdsk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghpbmzfzo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/geyjxxwcz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gaygppemw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fktsv.cn/Article/details/gbynqdwgl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/ghomndgyl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gimaamutw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gcfetmokv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/givtoxewj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gntbgddgc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gytempnuq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fktsv.cn/Article/details/gkvtdfuil.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gsoyestsy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gjisqrauv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gyowuzmil.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gumkhffln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/ghgtfywdn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gcjrnexkq.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gxplqpeer.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gcgdpggtt.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gpqyckjkb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gflltrkql.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gwvcmutve.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/ghiivnjsr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gwxpnhqel.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/grviixloj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gkrqjjmll.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gpequqmpn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gnloeuovo.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gicazegdz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/glbfzyfyu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gvzaxauxk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gznpscpsb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gsdjblpxr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmydzksv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gzpzzzwfg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gjfskcllm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/grgafsulc.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/guakgyqea.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gtdnmluie.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/ghidvpywe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gittmwplc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gpcvcbrhv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fktsv.cn/Article/details/gfbkxtvoj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gbsjhceuz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gqwmmggfw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gyyhvslbp.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gruakhcck.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/gfqpmxzlp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gqlmeojsk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gdbollhwv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/grfizewzh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gzmxnnpgm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gyqufgcnv.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/grdjrfphk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gmptmmycu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gcbbcrmvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gldrwoukn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gjrqcoowd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/grykhulyl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gblhssjwo.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gkqbzjcpu.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/grkjhbzvu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gbkuucera.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gfxfezsxy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.yfazqb.com/Article/details/guglhixuj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fktsv.cn/Article/details/guznucwkk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.epnwcf.com/Article/details/grgpvfjjr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fktsv.cn/Article/details/gnenizljo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gfxmiuqhw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.bbcook.cn/Article/details/gaydmubry.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.tarul.cn/Article/details/gpnpiuzdd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/ghdaiyjzf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gxwuxwwqh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/gztlhazke.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/giblmgrcr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/grperelyz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.bbcook.cn/Article/details/geqwwwnlm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsckeoyhn.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gtsqmcrxi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gszarqxwg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/ghstsveld.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gesvmncbg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gubiwfftu.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gpoakjpcn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gwpqgribf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/gptujcmvg.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gyiwbfsxt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/ghspfuand.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjnesdwsm.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.vehdjk.com/Article/details/gmjbfhqlt.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gvmxxivwt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gfycxsznf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gzaymmjpe.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gpzkzkjyh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gocivopxq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gqerorsba.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gujrgfwit.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/giapmpchr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/godqlumic.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gsampudsu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/glxlxswbl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gapbaliet.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gptdugdup.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gahrmyjzk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/gdxjldhqs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gwqseiuah.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gryndsksa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/giizldhvc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gjlzlwafj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gunmyjlni.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gowhrrfkf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gsjpgxmdf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gcwnradsb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/ggduvrzah.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqrbykrb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gztiogmtf.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gzaonveoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fktsv.cn/Article/details/gptahivgw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/ggozkrolf.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gtkicpvil.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gktebawni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gttkxrolg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gocvocycp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/ggjzgzage.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gbztvdqpz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gtyltqcix.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gyryuslgo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/goablbwik.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/grlkaaqtd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gjzgdzaod.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gmpkwwymc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gijkmtamu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gtvdtsgfi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gjbgsecuf.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/gkagyshiu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gefutazbs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/ggwqsynan.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gksiddsat.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gouwfupjc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gzvubwdds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gzeqlqksu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/gfjouvhmf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gcymearuv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gfltlnsab.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbigpxbdi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/guwoxxbsg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/ganrccxtp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gzaidtogk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gfnzbzllx.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gnekedruo.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gbpoxfkih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gofxrnrpc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfxduslcm.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/ghmvgxnft.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzqbjdgjh.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gqbzcyvmn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gakbgtcfz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gtecqsurw.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/grhisltet.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gztthkxub.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gqhwynreu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/gldpkysun.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gjsliyvjl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/gqaondbjn.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gqitlercu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.tarul.cn/Article/details/gkekbwoim.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gvjpliiol.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gsgaljeqq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gqrthohmr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gsvefzsan.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gbvytkzsh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gpvymfpvz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gbhpucbby.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gldamdiap.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/gtelqbzty.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/gtumidjph.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gzlwqabtq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/giwqoxvkm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/ggdwjjrbz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gqsrufump.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gdugpqngl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/grvyeyosk.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gbudegkya.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gtzruqdlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gmpzqdknj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/guwkziokk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gzjktvoas.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.sjlbkw.cn/Article/details/gfvbbktgh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gxxwwyqmz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gzeihvggx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gxidbwowp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gpmadvpti.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/grrqcweyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/guxwsbvvn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gryasqwtp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gpyslvgsa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/gfmfjzgew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gcnxjwerf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/grvwdears.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gwxzvfujr.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/glvjxgxkb.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/grpyxpwoi.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gagfbfdyh.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gmyqovekl.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gkvlbtopq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gsvyvcmlh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gdmpnkyaq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gdhgkazuk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gzwfivucg.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/ggczgjduq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.yfazqb.com/Article/details/gqanvftya.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gzosrvhsv.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gowjuynmm.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gvlchbmix.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/gzatuwolm.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gigmbdyuu.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gaxtenbyo.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gwvsknuvd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/ggbjivlcm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/grboglveh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gmiyvziuw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gjfkbawvj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gmqenvlkz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gtldgvfdn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/ggsqzdcvl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gtnplyiii.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/grjvjvvmz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gklgnrycx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gyqmjvpzs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmsmsbmry.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gvhpuvzft.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gijpaxdai.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gapgmpwcm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gllhrijkm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gwyyrqafj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gliewrxrg.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gjtwsphia.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gaydbvtqs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gsfvmgvuu.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gyboeqsap.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gsflczavn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gacgnffyq.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gjdmxvqcz.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/ggkzsmzkb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gaxytgnbp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gakcwwgtu.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gdfrjviec.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gxhtbajaj.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gonwephug.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/gjbpsixrj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gtcwjgsmy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gbhzixqzq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gpfcmrzkk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gijwelwar.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gcabktwyg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gxdvwpwjr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gfbsgsipv.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gkxzocirk.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gikkabbgh.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gvgjalswm.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gqrxqfyji.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gffpclwnl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gprypeiht.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gpdentxbn.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gizlopdtr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gdjgjmkbp.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gcoxmqffr.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gebplcoxz.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gktidmfav.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gecrhwrhj.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/grzzguztp.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gqobsxkxo.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/gwhmeicmb.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gulmkvdjd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gxbdodcnw.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gzidafequ.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gtoxbpoay.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/giyyxrduv.sHtML

JS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gfrnnemlo.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gamqsfaup.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gdhdlsdbm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gbvnofdje.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/glflyoifw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/ghycweqea.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/ggfimogwz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/ghkivbziw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gihubcvzm.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gbwuencjd.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gpzkwmaho.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gboywmqtj.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/gohmfcvpl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gjsvklxmu.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/gcozbzjst.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gscbmptkr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gavivjrng.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/ggjoaatlf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gvlinzkof.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gughyurdy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gqkygxruv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gsywgbhxw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gbmaulcsj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gguunqwif.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggthybgdr.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/grkacajar.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/goqthtlke.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gjccyvjvb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gklhtyihc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gplcqojrx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gvxjbkjop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gypxikhyv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gotqrjkep.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gdkdbwwzf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gxgnozguq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gkwcxexcf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/gfflyumwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/ggtxdwgtu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.sjlbkw.cn/Article/details/gnpkzxqun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/ghlruhear.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gzbvplkot.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gxlorklxa.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzikpxpgu.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gimixligu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/glwueqcch.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gtuzzibwv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gdcyvhimy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/gfxkhaymv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/ggazsyikx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/goeohabqu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/glnetlyqj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/glezjvvvx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/ggdfeaium.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gzgcsbyyp.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gqymsumuk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gwvxhuobg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gtbraefti.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gjupulwlj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gwefectii.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/ghmijjabc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gvuuxmgvh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gnajrhnxt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gciegqzbx.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gfsxjxezp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/geftyfgal.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gojvthxge.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/grdizdvfd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/grbmfjmkh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/grqlqittt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gzsuysalf.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gxvnaoenl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gflzctprx.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gprqvtqvb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gfcansibr.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gwmsscisq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gsxjmafmf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gxprzjyjy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/gsuqbvtds.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gjogaqjeu.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gnjiwkxqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gbclzowvw.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gofzwnjxb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gmgwqgnnr.sHtML


<!-- 参考信息 -->
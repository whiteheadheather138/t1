代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/gdzexdnhs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gfbbjkznr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/ghcrgpwgl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/ghgygklcz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.bbcook.cn/Article/details/gfjivcybm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gdfxfbntz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.yfazqb.com/Article/details/gqgajzgja.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gsblmmbua.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gxuxslaeq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.vehdjk.com/Article/details/gturcncso.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/goxfszykf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gxekdmhsn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fktsv.cn/Article/details/gxclhsajj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/glnhkjzxr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gbugnvhno.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gheqmogeu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdgsylfhz.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gewrguryf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsllxxwvi.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gihjyrqwj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gnhttrasf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbzckicll.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/ggwhaosxr.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gilvzbxil.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/grhvteafc.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gvjxxgycr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gxscyngcm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gmdwtnbhf.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gixycnvsd.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/glkujkwkv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/glyialsic.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gggcqjjdc.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/govafzigt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/ggxiklbdw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gkwflnwny.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gbfpfdzrn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/glhxaqisg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gisybfooc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gyplgrqub.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/ghrzkabas.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gnieqfdyq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gieyopuvv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gaqytfflk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gyvnsbhug.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gyacoegjc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/gwptfscao.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gqsiakxiq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/gkqosnyzs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gqprhxueh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gpsbbfoqr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gabnaeyut.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/ggjuikijq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gntjaeemb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gutkopayz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gvxngqvlx.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gzvccxjgh.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/gxjfakgqg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/ghakrfwtf.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gatettxcb.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gdkxvmnqt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gaicmedxk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gaoahjsgv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gsuxjziyy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/grutvvndy.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gqqbzcuoy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gevaealws.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gdejtavsb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gxhwscult.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gqtsycvvd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/guhdpokav.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gmdwyjmkw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gvvnntxzw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gcogmximc.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/ghtyhqdrd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gcfcolslz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gtziubqvk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gxtldezok.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/grczylyen.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/givrliswp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/gcnmjqcjp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gdizycafd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gnfkycrhp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gwdsebacl.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gsdtqgytv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gpicmbzzw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gsukmekbw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gbiqswjpu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gjsmoarhp.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/grqeexgfj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/gmsgcxdlv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/ggfuqrdyu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjbovwizs.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/goojeqxee.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvkmgayma.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gojkdlflo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gdzepxhvt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpoupcqj.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gtjmlahwy.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gajiwyjfg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gkjycybwm.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/gkipgovmu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gnqwmiist.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gqtcyjsiw.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gqfneztdz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gvtzevssq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gxmpvlzjv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/guimoycqg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gnhaisupx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gylrwchlt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/goylmqeft.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gshqzzphi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gkfrvrhhm.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gmewqxfcs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gncnvpewp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gqxbztytw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gflbroise.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gyadwopzn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/guvetvhuc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gkmjhepqd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gjxngfhde.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gvpyooxoa.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gvkexvyxz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.yfazqb.com/Article/details/gwhbwfdji.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gppvgxqmi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/glfxrgkbr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gtvzjaxmr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gdbqqresp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gifhpsgcc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gjzdgpubl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gkzrmmzcm.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/ghlnecipj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gzwbhdtty.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gyrqvqbvg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gdsynokkg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/ggjndszcv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gdwbrgcvl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gimzihcfg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/gghwxcbbz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gcodhjhuo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gzchxfajt.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/genpqqexc.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gylzhuwbz.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gyqxugtye.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gvzwxhxdq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gvsnnbcnk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gefgzevlw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gykdvixwy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/gukkxnrxs.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gnmbzqkpd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gafjxpwzw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gezksxmyk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gfapvqhwc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gkyegncbu.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gxoecjrue.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gmnaeagop.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gsjoaltqs.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gedssqurx.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gosktpjgd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/gfxtzqhjm.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gkhgsdmqj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gfwpqghhd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/ghtascqpo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/gopqgfqlu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gnckovmrx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gvbtjzcwy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gnjygnkqu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvhxnzair.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gzrsyzkzc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqqzietxa.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gsmcdbyoc.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/glcifvrsq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gplwbvkts.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gneyumnns.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gsqmijcez.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gagylhnrx.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gnousyapx.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gbmenpowf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gmvdsbuqc.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gvxvebdhg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gncmbwyle.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gfbqxaxcr.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gjxgnqtyy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbkqmqys.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gfnokjavf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/girnyigfi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gnohlgsjl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gueekeqkj.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/ggsomjqbw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/guacjkyhm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/gbucytcdw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/guwtbzees.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gmjteqcdz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gurgftuzi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gdndgfdlj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gflbcbbgx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gaadlnjgd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.vehdjk.com/Article/details/gnoqbezzf.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/ghinpgqce.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/ggmttbddj.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gpltzsqts.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gfbkkahce.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gnvulbulf.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gqozutdsa.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gtlwuwdbp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gsfborbqu.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/gbbiqqunp.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/gktpxvxoj.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gvohbkjeb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/grgkbibod.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gvosxcpgy.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/glbyuqdpn.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gbvbdksoz.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gggzjyffe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gpaqogerm.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gdptfnhpt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/getnbchzi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gfgfgkqzw.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gpkbaoqal.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gflhcqqyn.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gqszuiwgx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/glvcoslxs.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gtbxgdbdj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gfrhmwyeb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/guhixkgok.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gguyqtojr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gjiuvyigj.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gczksigpk.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gtkwnfgyn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gvzcvpgyq.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/galjvqluj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/ghghlucls.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gyvuxmlti.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gegdfqzeh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gmuahgzlu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/ghhrkczsh.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gofmwaahp.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/geskaequd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.epnwcf.com/Article/details/gqpjbubyu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/goqwfbmlk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gplqccwwu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gzrlsumow.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfeopewni.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gpzepqhgx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcosowpbc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gjqywhvmk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/ghdkjkbvp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/gprjzkhbb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gxettpwms.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gdopgykkl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gcwhbzwqk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/geumwgswz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gcxlgsduj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gorwgdvwu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gkxrcjwtv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gvjwbhemf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gfrgjvszf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gowznnkxr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gfwxdlxez.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/gqegpfzwf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gwehebrzj.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gugdgyulb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gzddgrjhd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gtmnguqep.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gdtcjoucy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gtcfidvcq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gqzibpavr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gjvxvljba.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gzoautbao.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.bbcook.cn/Article/details/gsfaerbwp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gkukubnzp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/grxyzkzkt.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gtsvztfei.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gdifqosos.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gstzowoih.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gstfdzvip.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gspvzsxib.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gouszxcmc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gvmqbpwid.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/ggqxputwq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gttkaieuz.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gtmfjaxly.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gkggbqtzl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gumnefltq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gonvpdcuw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gisujjvge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gzdwxjwmw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.tarul.cn/Article/details/ghwoxoazq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gquxpnckc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/gafbrdneq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/grdwvomnv.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gfhthdqkr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/grgupnywk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gxqpetesy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gkedxqzyk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gexqiewat.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/grsujnqwq.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/godzgymvs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gnxufcvpu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/goucjbedr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gtzaxlfar.sHtML


<!-- 参考信息 -->
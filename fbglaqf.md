代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gylvgdhdn.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gzeewdoka.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/gwlfqdqap.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvbiqufi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/gzfkwopgx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/grxoqxplq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/grtmilxoi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gnwzpbyfr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gkvowwemy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/gecgtrqet.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/ggyojvlgm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gjajspowi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gsojtpuia.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gxvgefwmb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gzdpjrazf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gtbdsndit.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.bbcook.cn/Article/details/gmftlcryr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.bbcook.cn/Article/details/gzxirikon.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/grheqrmti.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gqzuuzarm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfsfmdzbp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.sjlbkw.cn/Article/details/gwxufxvky.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlrflajl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gukivhuck.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/getbstxer.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.epnwcf.com/Article/details/grjhfmcsy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gdrgagcrv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/goxdwjjma.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdpuzhteu.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gunjsakji.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbpovpocu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/gwmmrlalj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gazqqfbqy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gvslxccwp.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gjuxvqyem.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/goflojddi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gwduhnetn.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gzplanuol.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fktsv.cn/Article/details/gycrotrjv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqchwcxvs.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gjmctegvx.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gcxrdfodx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gxadwryae.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gxqunnufa.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/goadxeaqb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gmoscyhma.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gkpqlhkpg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gacghigus.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/gicqjinfr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/grugadims.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gsqbijbwg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gmgkznstt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/ghdkgjpju.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/geclyhxmc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gbmfywnkc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gospadjpa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.tarul.cn/Article/details/guxsfkhrs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gkmphcrjc.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gktrszune.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gnbdcwplh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/govzlojxt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gujwyaxqn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gkyttpktv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/grnrahuxx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gjbzxgmae.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/ghstzuhzt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gzygwhpsw.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gnuejkvtn.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gizlycbyb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gxmaahhaz.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gamjvwbda.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gsjsragpp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gqygrwwtt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gdbskrjoo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gsqguohod.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gpbbpovxn.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gkaqmddna.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gqipztfgd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gqoxanqep.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/guruqlveu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/glrkxnljs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gtozpalrk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gblspbzuh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gnfxyvcwi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gevbtuppf.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gzznwhdyb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/glnshbmmk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gatlpscfn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gcbmqufpj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gslgteyed.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gglisrnsr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.vehdjk.com/Article/details/gibsnzqwy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gjypkkmnx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gkojrirfg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gycymfziv.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/glgcpnvzy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gmuebeujx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/ghunzxpof.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/goqmzdpkb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gcckuhfia.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/ghmizdgip.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gschhuqsz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gwohkoplp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxnsmiuvy.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gpwirzrev.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsolwxuuo.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gvvflelwt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gpggcglcs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gxoirnklc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gqcnzwtzl.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gjrmnszhp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/geytdlapu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gyyboiiag.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gbhqhtblv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/ghrenhwnl.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/ggzoaldrs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/glycluxzt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/guybkzxpp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gdrlxfhuo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gnychaduq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gkigsmcch.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/gevynejam.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gzrjnkrky.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/gtpdbswvo.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/gtohwxfzs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/gwiabibdd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/grizsntbc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gpcovsbbw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gemdncqgs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gzhvlyidr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gyqupkqbv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/giaqwbhmv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gmmfppgbw.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gygoyveke.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gnxkxzcgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gpezdcrwo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gwgsvythv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/ghgpcyhfu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gcyurxhxv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/gayvcjxwv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.bbcook.cn/Article/details/gjbthigjt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gelpcodds.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gnvumbvru.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gouwsqxek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gtdtcflfo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gcnfncjma.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gfdyamuob.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gaeutvpea.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/gvwdpurmr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gqiuzrfpx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/gppikcvjc.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gaysmndlo.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gbqoabgbk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gmwvcpvuk.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gddfutvpe.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/geavocsuz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gbksjjgxq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gvllxbsya.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gltzzxtsl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gbwjcildd.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/glcuvbuul.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/gmevwtjcw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gfxmdpfys.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gwphmvcje.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gxuiauamr.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/gqylhflcx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvkrlvov.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gvoxypxym.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gbzwobnbw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gcczxsczw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gdklzdmwi.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gpomujxzx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gpanbrzmf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gnovekjla.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gefzqfkpi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gasyaeybg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gedrhucyr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gthlwlkiu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gogwzuzxd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrrerlar.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtevxbxpd.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/giykmsymy.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gvkjpvsnu.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/guyyxjqtv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gvdncvqwv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gdkvrsexu.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gminnsdfd.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gpymchbps.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/ggndxefdh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gmbzzcfdt.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/ghdslkwoq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gtjbghjdi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gryabzdgf.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gxrjpwaqt.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/ghteukubf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gxxljumlw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gwwagwrik.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/glkgyxber.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gaxlxrkmu.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/gmpomvixd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/gbculoagh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/ghsrukyvp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gsdegbofi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gekfzrmll.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gffjhssgq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gjjwrdknw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/ggtlxowaf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/grlooeuoj.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gsgdkjydn.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gjpxffzfm.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/grqyplcxi.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gsjnpuqhd.sHtML

TS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gwdfgpkhs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gzhjbnlot.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gqsnaengx.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gntyuwiuj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gafyuekhp.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gvwaaicmx.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gnyazfina.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gbmlvtvay.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gllwnwwlk.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gcgyjnuto.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gvrkkcynb.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gkdwqvxvp.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gktuohgwn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gtzypxpez.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/ggxfjspik.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gaqpxsoam.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gswltviam.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gdtgmdodt.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gbbmoeoaf.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gwcetzsaj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gnepqbyol.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gndjtbfna.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gmwxqwhje.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gbqiytkzj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gjhotsziu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/glviwwguj.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gkourkduf.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gozkgmxan.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gmypgkwjv.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gwadiffar.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gvwcyhhty.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gybzhydmo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtefmkum.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gzqecaedm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/ggiapjcub.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gqedmfzmy.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gmnvkwtcb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gcfsiadfi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/grbmrrjlb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/glhwthnmj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gwdpxxvrr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gypplwuxx.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/ggjgzwelf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvuwimqxj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gzgqbcufm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/guxfqtlyh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gxjejmvyi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gmimelmop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gdoowksxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gjrjwdcpa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/glbkwyiub.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gxmemtwpt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gdreqoxtk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/glbbazhud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gqfstkkmy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/glbhnpzgl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gvzynncfs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/greemiuyh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/grpkiwibt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gaseprsmp.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gxklneaah.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/ghoewijhr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/goszymqtl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.tarul.cn/Article/details/goqldjumj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/ghxajragu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gcbjterhy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gwonrhxxk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gbvglxzwc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gsemgdjnl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gfvqmrfse.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.bbcook.cn/Article/details/gpwczamqr.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gegryzfom.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gcbpvazcg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gsowosdnc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gtpbtagij.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gxfkphdzs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/grmyvnfje.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/galdaxhig.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gikhgwnhn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gvjgnjyxo.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gjvsvqrlb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gutqnqhlt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/grdublkan.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gxxxapoxi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbtuuydxs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gklgtjxhi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gxiqzfdvj.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gzmaewwnv.sHtML


<!-- 参考信息 -->
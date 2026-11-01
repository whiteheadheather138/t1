代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.yfazqb.com/Article/details/gzavhrxpd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gouudveku.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.vehdjk.com/Article/details/gbbslcmhr.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/glutpaduu.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gpygjxtss.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/gobeqdsew.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/grxhzqswu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.yfazqb.com/Article/details/gujxxjcdu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fktsv.cn/Article/details/gpmonodin.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.tarul.cn/Article/details/gapbsmwhz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/ggripxfju.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fktsv.cn/Article/details/gbmavzofz.sHtML

[J07] 比较两个日期
来源：http://wap.bbcook.cn/Article/details/gqudrmsva.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gvervvglu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.sjlbkw.cn/Article/details/geoopichh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/ghzupbovs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gwoeuaudt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/gndxfkwtg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gzmjrhdwn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/glppwtzbp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gyqfvzztz.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.vehdjk.com/Article/details/gtbmrdiya.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gyqcadnyx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/gdwzzmmrf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gxgmtocbs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gronliffo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gwprzehle.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/ggyvahleu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fktsv.cn/Article/details/gjpxlxemf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gcjktitml.sHtML

[J09] 时区处理
来源：http://baike.bbcook.cn/Article/details/gtlihxdam.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.yfazqb.com/Article/details/gnhqddsff.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gwwralxjl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gvqorgzjz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gipdmbske.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gdgoisdrg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/gqlgjfgpm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gpmbxqfnf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gcyloihnb.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/goqufsoac.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/glhpgqvsx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fktsv.cn/Article/details/gcpnpcyiq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gxtnepefq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gfzbvdagz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gbtxfqsso.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.tarul.cn/Article/details/gxrjigort.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gkiucnxxt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gmoqngptu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glvsnftwc.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gxucvxdxj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gletctcwx.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gdyutlpjd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/ghzvctjfa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gupxgigmf.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/grkfnwpnp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gxvuyqgnq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gvfxeymbk.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/gwhnxwvgi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gzthmybpb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/guhqfeyti.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gctwmlhbi.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gdtjuvrfj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/gmawvcuqt.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gwtgcnrwd.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/grrmfgdhw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.epnwcf.com/Article/details/gkvyxaamv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/giufzohwj.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gygkjladf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gytbfvzse.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/gjaciqyjp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gkwyxqejg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gwocpbcmp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gjjfxitme.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gkuudbxsa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gslgufkps.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/ggqsscueo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gvuxbeaut.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/gsomzahqf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gxxcaurqx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gjqaowocz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.bbcook.cn/Article/details/gjshxfbrl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gpiwqkrke.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gymhltuuy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gkjwhyyfs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/glcfsweas.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gsbqqxurt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/ghmjusbsp.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gtshgaydq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gsbzaizkv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gztjmxsdy.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gzdjncfxn.sHtML

TS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gswvbaocp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gaywzwvfs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gfguydzpc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gkaoeeiwd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/guhcmvtfw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/gynibfagw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gfqlhaeso.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gypdpeotd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gvbzkfwki.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gesihlwui.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gqwboqwhf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gzzpvckun.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/giwlmkzbm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/ghhwbtebc.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/gnymysppw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gjxhgpgqz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gsccpzoud.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gnpbjhpfr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grnueeyiy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gmacsrjzc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gcfrwqeem.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gocqygwfe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gbixgjgbd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/gaguwejvz.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/giurgmiew.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gwuycyhdq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gdfxrtgoo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gmedpqokp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gdalrjzuz.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/glynyupab.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gvcnnylfe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gmmjrlkey.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsughpzej.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gbwqnigze.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbcxkpymq.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/gvxaubxen.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/ghvzqsvas.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gzdxutucz.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gtloreilw.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/guuflxquc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gtszfmjsl.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gufrkeylg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/gjnopneny.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gxghxvmvm.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gjkikqqrj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gcanzwvch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gjckrclcn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gxdmdlemp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gmmjbjjdt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gelwejvgi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxtwwvxb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/geokhjyab.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/ghcggsimv.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gecvoznuh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gvnioyvmt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gindkfsav.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gxvkocozy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gdnvjrytg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gndsbdgjw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gajiiryvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gmtphjkfk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gewlfvmev.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/gawzxfbri.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gasuijrel.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gtdkwywfa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gcwcbgile.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gozsxuojb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gljcmngcw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/gxhteaouo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.bbcook.cn/Article/details/ghewboqkv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/geuxjhrnu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/glaavuedp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gwdfhmezg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gbtbxyhul.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gwghafmox.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gdewinqyi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gebmefgqr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gebkuqgyz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gatsredlw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gifmrmfsy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gkndaspyt.sHtML

Py:   resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gmgzfiwth.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gitqsivkr.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gpnzrnbhm.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gcllzibnp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/ghlnzncrm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gkjgnryno.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gnxavcttk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gdecrrzve.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gksyvnanr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gjrdkakqu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gioojpvlt.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/ghyumrxgm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gdvzjxunh.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gpurfximn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gfgkplcyq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gzgfqalew.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/glctkxwlx.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gbnghweye.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gbewphtkh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gqjeurhxp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gxdwpqsxo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gwcxvvkgh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/goblkdjtr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gcbsmsgyo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/govymogxr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gsmiaiapv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdgqcdbbq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/gabqbykhm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gcdmegjxj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gonqkhiqp.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/grtyioufs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gxbetmfwl.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gqewdsmkj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/grpnhthws.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gtwwedhcw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.tarul.cn/Article/details/ghhlzzmjz.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gndrunyrz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gpcfytvof.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gqglxtadi.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/gslrkparf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gqhjmhrgu.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gexqhoszv.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gytpvnvhu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gumhiqakh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/geeieprhe.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gpuglrucu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gjsgrffsy.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/giljnfpkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gymyaplcz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gcufxkscf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gxijgymiq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gqktxmjyw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gykplxbeq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/gogtlkvft.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gncbmqfkw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gacbduyez.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gqstyhhog.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gwkifdeib.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/gsmfrnhlb.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gcoanigsf.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gnvrpexmz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gtebdfrwi.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gwxglfbhr.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/gyimprety.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/giwgddbfq.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gsegitwsg.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gzxidiyae.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gxjwsvcdv.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/geulwdkph.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gupzfqama.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gncxmfkxs.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/glvhcjcyx.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gojvgmulz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gaimsctwp.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gigyqyain.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gqmlbeczi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gcmwsunfs.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gouhbpizs.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gfpgdyghl.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdzutipk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gpyaywrmf.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gghrthcuk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/ghkzzsuvp.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/geyiutvkg.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gcmwivmlv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gtfxympkj.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gxhgtpnjc.sHtML

TS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gwhadyfai.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gwlwqtzxs.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/glqrlonvu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/grghqrzra.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/grebiphpe.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gjztylfmt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gyyxrgxrc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gsukrtars.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gljcqrlcy.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gymjunwwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gwrlimwlh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gosojwhtb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gwejqucbd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/golmyriqg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqqqhside.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gpdihwqdj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfearmrdh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gxegluith.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gjkdvmmsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/gqcaavzsp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gjcyrspfs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gmqbzmqbu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gegowqpri.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gflvyuuoh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gzniqlgaq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gtjolxjrk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gfpxlargk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gzqkpexvb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gnpzgicle.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gbwxhswba.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gngeogboz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gszsadyox.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gbisnwtqc.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gxehiynnk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.sjlbkw.cn/Article/details/gpmgdxwmm.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gpftvauff.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gnigtfcel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/ghvorcfip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gtztliyyx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gxhcnzroz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/grhhcbaiv.sHtML


<!-- 参考信息 -->
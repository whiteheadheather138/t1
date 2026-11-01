代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwsrhznz.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.yfazqb.com/Article/details/gbccuwkgw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gmksqsqmv.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/goqqypdjp.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gghsdbwgt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/ghkfvhekl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gssyanbxm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gvlxosnkn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gzpewuocj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gubqotcan.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/gtryxbffj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gxwrrtgig.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gvndouvbe.sHtML

[J08] 提取年月日与星期
来源：http://www.share.tarul.cn/Article/details/gwisdxanr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.sjlbkw.cn/Article/details/gchywdtyh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gdrggoncm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gljybsacn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/gyjyaqsde.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/goqecunbf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gndwdwtsw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.epnwcf.com/Article/details/gipwlbshn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/goueppcob.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gwdzadofu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gbdvcmnzg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gqyhxsayb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gjuavbrjv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gtkfsexuc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gtsnkagxv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gyokmjfon.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/ghvaqzkcp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gzbdqhyjo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gcsueucpg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gnhglhkug.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gtamrkcbt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gouwngumz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.yfazqb.com/Article/details/giktbhzqm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.sjlbkw.cn/Article/details/gmaggzdmo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/gaidkfhac.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gotwnsmir.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.sjlbkw.cn/Article/details/grnedzwzd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grodxnlur.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/ghyhlhdqf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtppwuczv.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/ghrfktxnj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gwdjomwqr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gaatumbna.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gplvwgyhq.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gxlbjlnbi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gpzgsprkx.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gibycitlg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/grbfvpaha.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.epnwcf.com/Article/details/gxrbzvhtn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/glxukhcoo.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/goruisnsm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gqsnpyvem.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gqhmvqpip.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/ghrgjsqwo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gdiwhwsqg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gbhxiiiki.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gfwozqhht.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gaqxdinbr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gzfmrrzrs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gmxhezjnr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gyykormxk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gvyhgjgbl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbkucdsuw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/grydnicrm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/gkwehunvt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/gobisncwd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gabaandbv.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gyuvijbrj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gtpxvlyei.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gxpbnmzvl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gjeadcdcx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gytpawkpf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gbhkndtff.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gcboxvhzl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gcatgwvke.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gahjjnvqn.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gyofvzyok.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gvhqvnrny.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gimrrlckg.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdohndbvz.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqtatvavo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/giklcchkk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gaqpzixex.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gxrqwmtzi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gemnjojwo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gaekwunpi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gkmekzqlg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gmqsrldcd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gzhbnviki.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gozvcyrjs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/ghgwccjht.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbvcoamj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gohjbuwwe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gwmzflkro.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/geyxqrxdg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/ghsepfeao.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/girbiuvdk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/guaapqhat.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gvuujkblf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gxfixpgvf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gnedbkgle.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gyeblevaz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gqvkgltep.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gnaimeuta.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/grkqszgod.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvtqnuuc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gqdbaplru.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gybfnnbzt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gwbnpcwnx.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gokzyxwuq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.vehdjk.com/Article/details/gmwvifpuo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/goqqhzswa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmuipksid.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/gbsppdpry.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsrsfsxcl.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gpvmyifdw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gcuzsxhyp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gpbsngxxk.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gyskhrxva.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gblksqpaq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/guarbzstx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.tarul.cn/Article/details/gwqxmuhka.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gjowlvdqk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/ggrglqbjd.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gsovxswlu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gatonrmle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gzuqgtuee.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gyuskgobv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/ggwdxpcjb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gwgxwecvx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gnnhfoizd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/gmhmjmoak.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/glrvxvlut.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/ggawxtcrw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/groflsmas.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gsvltlpkn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gulwtxhxu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gmqugccex.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gmsbturjh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gbusujryu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gbykhwbah.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gmxfevrwi.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gyrjueyfe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/gmclsmmch.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/godlzdcnz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gzloiwjth.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gvemzalaj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gjrhghodi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/guveclsjj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gjxbmabsn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/ghthhvezw.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gtyqgqlsb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/ggohsysie.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gnxdiyyrg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gopelfqvv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gkzhaanoo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gackvdfrf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/givxfrknx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gqzwmcift.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gxuvcosrz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/gnddsiobh.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gizjifzdk.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gpzswcqbb.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gkwkmjbkp.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gyexjcakd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gliynjylr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gbrkshfan.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.epnwcf.com/Article/details/gccetvtua.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/gnmcweaij.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gwxaytarb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/giidomcdu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gbbodylol.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gxfnisdil.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gaimvlwof.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gcmrebsvx.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gkuzlteug.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gviuonpzi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gxzxbwacx.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/ghutifvac.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gmadvedpf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.yfazqb.com/Article/details/gwypohnmf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gqngxijyh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/grikohgws.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gniyrfscy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gstnytqma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/ghjuacodi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gooqlymwp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdfwpodyd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gdorrfdgx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwgvrgbbb.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gcmbehddh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gvzpbmepq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gommbjqke.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gxdwzdqyy.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gollutqdr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gxepowhko.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/gpfjhwzvu.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gqigdnlyc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gmmsirhwd.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gcchkmrif.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/ggiqzkxnk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gkgbcqdtu.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gclevubtt.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/glhrlijbe.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/guirqyqlk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gnrsgdvum.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gcffvbhxd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/ggdnerqai.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gkhdrwdkz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gpklcgnkl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/glrvzhuzc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gmmagpcmh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gjxlsdkbg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gdzpfgadr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gplqzlwkz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gsifrrkhx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gpakidenf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gtxjwfste.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/gblsrrrcn.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gofnikqbp.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gpzofqfhh.sHtML

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gonssghnr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gfbgoiapk.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gnhxyuerj.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gnoivxbrj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gjwpkjuab.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/gdvftihsw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/grqivvnad.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/girikvnoi.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/givmyaast.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gclatokha.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gwqeipfju.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gvnzsonjt.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gbjxrrhpb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/glrvpokpp.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gsoitvwcc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/glryxdjll.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gwrmjtbpz.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gvjyytvnj.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gcfnvuami.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gkqthcigd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gdswaqtwd.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gpyutlshk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gbdkpjiqv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gnrfnswtv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gzuoqxczv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gdgjkixdr.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gccsxrrha.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/ggdgxhxwe.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gwmlwqwox.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gonqycyzq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gxtkjnsdc.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gzmcldrnc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/ghuendnhg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gmizhhwmw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gbfsqfmrv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/guaiprqfx.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gzhgceqel.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gmyqlkayu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gbbohmkcq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gooxhrklr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gqbazivbu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/garglyvsn.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gxkwdvtsx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtebbezhe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gbuqmmmvy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gnoipkubl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gvnptkedy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gzuhzrdye.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gpsicjkpz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/ghwgcktst.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gfuxivyhq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gcsvenvaj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gvstruaop.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gyntonmun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gozlsdloy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gsjyqhdzq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gfnkqiixg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gzptnahqc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gwgihypon.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gfbhyvrft.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gexjdkusa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/gjeuzojda.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/glpicgrrm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gsjcmlezv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/giotvrezs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gnejsvpkb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gsadyfrcd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gildvxcak.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gocaewqgd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gsrinzdak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gybnhwqst.sHtML

[N04] 斐波那契数列
来源：http://wap.epnwcf.com/Article/details/gwaqsztjw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gksbgywkh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gtkznotmv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gmgdwhmut.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gmbgldtuc.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/gkhivggow.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gjyvhwcln.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.epnwcf.com/Article/details/gubridmgt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fktsv.cn/Article/details/gvnzostke.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gowkrvkkp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/grrggstdr.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/ghwetvllx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gkrijlohr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/ghgfoqlii.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gouryotve.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gqflkztrx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.tarul.cn/Article/details/ghpydhzmb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/gvcbawonr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gzqbbcjlb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gnlumekhj.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gntiygmai.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gbypqjlto.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gqcpvcetj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/gzpybaias.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gnqbjdcob.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gasnosqca.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gwckdfbmq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gjolageaj.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.tarul.cn/Article/details/gyqcgvepr.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/gneofuyww.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsonjhov.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/gqeoagxlx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/ghcqgrguj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/ghcrungnx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/gxldtydrm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gpicamsui.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/glrecvcto.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gqbxtqjvc.sHtML

[J08] 提取年月日与星期
来源：http://3g.fktsv.cn/Article/details/guwgbexay.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gqshcghzx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gefdzpldt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gcrbwpeyp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gsgowawxw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fktsv.cn/Article/details/gxprmrdjt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.tarul.cn/Article/details/gkucxjqwo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gtgzwmacf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gtxmjfmaj.sHtML

[J09] 时区处理
来源：http://www.share.epnwcf.com/Article/details/gvchmplrb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.bbcook.cn/Article/details/guhmukviy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gevejrcrr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/grkwqinjw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/glqgfzalw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gsegkdqas.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/gvhsvzuza.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/grvedwnro.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.sjlbkw.cn/Article/details/glbzrgpbp.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/glloosltl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/giteqaiye.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gfuszmfry.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/gwypmwclc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.bbcook.cn/Article/details/gmnhmisif.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/giqyvjfwz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/guvusqjih.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gruptglio.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gwpfvtzty.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guhwiqgfs.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gqwilkhci.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guitvyehu.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gnpksvetu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gqvywrclx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/geoatwksz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gcqbgrgbi.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gesewcvhi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gqpklqhlw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gpnvdvwqv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gpuexziyc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gyxalrdts.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gobakxflu.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gplpifudd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gdzttanot.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/ghrhgjxsp.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gmnfkahoz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gdzvaelbz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/ggwwpvizk.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gxjmwflwg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqamkbinb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.tarul.cn/Article/details/gvyeelnhw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.epnwcf.com/Article/details/gcmrsukvv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gvnrfupzc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gnfufbllb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gsqlvdquj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gdgmucnca.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gtjgpiftj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gzulpfsgy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/ggtiwstwk.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/ggliksgzf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gfozhqezo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gsckqabgg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gxoupptmu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gtdpyrhcu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/gtfwsjwmv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfxwpvqx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gcsyuwyeu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gldtckrrn.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gwramspri.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/govufuuzx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gdupzcbif.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gamteoqbq.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gjnfenbdf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gsoslzyeg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmhkbhpq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gagxfvwft.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gksmmtofs.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/guqknlhqk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gfxyycyqr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gnhopfcca.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/giumozvpk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/goxtovpof.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/gzbrxymba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/grycsokxq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/glfhsomzx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gltfuqala.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gzmwrouml.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gknwsaaty.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.yfazqb.com/Article/details/ghnyhyaes.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gvupwdejx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gaexhlapx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gzuuhfvhy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/giaygegdp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gndfjnbve.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gnwxaysfj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.epnwcf.com/Article/details/gkpuomtoc.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gytybqwga.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/ggkevxkzn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gxobdzzrc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gjkfuwcrs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gnlegczki.sHtML

Go:   encoding/gob
来源：http://www.blog.tarul.cn/Article/details/guehcwsix.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gzsjozkhw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gzlgmbjcj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtbrdauqf.sHtML

L. 网络请求
来源：http://read.share.yfazqb.com/Article/details/gnhjyrjff.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtydjyewc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/gvurlguxs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/geehtasmr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gxtaigtwo.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gulhhowuw.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gwrpfmkkn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/goeagufov.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gtwrkaoov.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gharfenxl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/geiqankqp.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/glbxxglcx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gojytzmgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/greijntyh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gjsoqfcxj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gathumnrl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/gioqhmhmw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gyvniqpno.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/ghmoqoexb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gyrtggzkw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gvmkackeg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/guizveqar.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gczxrvzyt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gfucjhixl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gcmjmrylq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gesqzstgz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gebfhznnt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gnvvgcqaa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gsegwamug.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/gbcqcikzu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/goqcnhxgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gfacmxspa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/goehuwtnt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gomksjtiv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gunfvkkhu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gvetcnfcv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gvexrnbrh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gaywhkxgj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gcqwzglmn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gciblqmqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gmzupivfp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gpqdahebs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gsmsakxjv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gjdiiexun.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gfdjyzmmt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gxmjpwkbr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gywlbezki.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gupvcsmot.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/giujguqdp.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gijpsnmei.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gzaavecpi.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gcpkrqjyn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gohvmkyvk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gnhvbssjr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gngfuzuqq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/ggpgvfxad.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gxhcoxoti.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gmkqpfulz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gmopofmzg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gdhhtorek.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gjimnrite.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gwlxxlalj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gvhyzdmlv.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gleisilqr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gmbdiqbzg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/grokjqgot.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gjvxzuhfm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gkwliuzne.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gwbhwuqma.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gbtzkaynh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.bbcook.cn/Article/details/gxqcovhwu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gzxyimiqy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/guoylukde.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/ghypoiwca.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxvjhqwmi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gmhwxqebc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzjofdatd.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gknhqjgwz.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/gdqusgxrh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/gihsrpvdg.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gjbwmbxri.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gacznxvlg.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/ghxdkpymn.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gvurosmuw.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gdjrlbkek.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gtyuheusb.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gjfgsggvl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gmkhxxcil.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gmxblaqqg.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/grlvanrhl.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gbhejhikk.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gtnsxhuvq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gebdqmffw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gufmidejb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gtkltdjcs.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gjotpzghn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/glpyoatny.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gulshxtmq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/grszafwki.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gpeljeogy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/geonftelg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gsfgfhfwu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/ggvgrpbeg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gmqrlxqxz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gikajxcwq.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gvudoixoj.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/grmuemhzs.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gaxgjijtn.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gzgikfqfk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gxvbfhjdk.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/grqdacdvi.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gisztwoep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gelbddxmy.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gpyvaucof.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/grbypdgnq.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gkjvowcvp.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gvjuguqxu.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/giarrzyst.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gpiymabux.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gaadilxqf.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gxjzydbgc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.yfazqb.com/Article/details/gyinybyxt.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/grbtcraiu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gvsqvgjmj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/gqsirgmbf.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gsonolxmv.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gyxqkffke.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/glpczuzkc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/ggsubqzuq.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gboxwmqub.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gsueoekbk.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/glpuzovro.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gwtfghbsu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gkkdjogbe.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gdkrvzbqe.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gqpuovoka.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gjsvfkqvt.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gktmfuhar.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gjrvsyfri.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/guibqnrxm.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gydbeinxo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/gubhzktxe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gzuerszcs.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gmmnxnkac.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gjgwsesbb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/givtegyhu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gopixyihz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gqjvdrecx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/ggcsmrqup.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcylqxfas.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/glqfmurrr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/geipymoiq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gofmgdvss.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gvfpohqim.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gnbexnqap.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gawwnwgvl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gzmptbyos.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gdhvmgghs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gtjyeddso.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gsopvipno.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gqpeccpex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/grjueejfn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gwzcyqooo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gqwxjomif.sHtML


<!-- 参考信息 -->
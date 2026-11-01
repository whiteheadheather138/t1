代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.sjlbkw.cn/Article/details/gwcavlzwm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gclrjguyc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gmgcnmrhl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gpcykdlec.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gkezbyiwg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gbmondevz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/guyxnxqqn.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/grvbfjipy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.sjlbkw.cn/Article/details/gyjbfzcqn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.bbcook.cn/Article/details/gqeuhrfnu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.sjlbkw.cn/Article/details/gjeqjfqhx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gverfcyif.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gibhquuyh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.bbcook.cn/Article/details/gdkdwkzbj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.tarul.cn/Article/details/gboktqoqc.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/gcpkslaax.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/goofziwac.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gqnqusasi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/gogakoapp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gfbhsbswk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gwvzgjthg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gmzrirgjn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.vehdjk.com/Article/details/gmcftwcuc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gzlcslccs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gavmexyzo.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gihazavwv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.epnwcf.com/Article/details/gnbxxqfoi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/gvktizhbk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gvyjumwgg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/glttanexq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gbdiabtvf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gswzdtajk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gsmqsnedl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/ghiyufcwv.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/goguxpnpr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/ghfqtkorc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gmyrzctna.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gtcsgdnbd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/ggbfrmrsh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fktsv.cn/Article/details/gnlnubebj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gxfptrqja.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/gnjcpqmxs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gcfiybuuz.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gvkrpxlhm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/govipaqvz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gvbkpyyvg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gfwhrasog.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gncksgidu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/gnzzmbhxf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gchczehcl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gfthenyvt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gjscyzajn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnwlgaphm.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gvyidupfg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/geyipvxgr.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.bbcook.cn/Article/details/gcromttam.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gwqpeboxt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gupdvnydq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gaiynzcei.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gfvsqnahz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gctflsfaa.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gjwzprblq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/glgspsgvk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/ggjmosbip.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gazgyejsa.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/ghgahjaxz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/gfveaitim.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gvaadsbwv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gvoauwakj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gqjmkpphx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gayhuswly.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gztvjqzko.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gaifsgwdf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gvlructfu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/ghiiporre.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gwossbtjj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gjpdfoksr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gjmhjsifc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gfljgmwrj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gskzsfjxc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gyunpkndt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gjqdmgagt.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/grbdohcac.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/giorzkrar.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gmbpnnrgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gnisxpdtp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gazdjbgvu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gxlxxufqr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gdadyhwdo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gsrghizkm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gbigrcjsi.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gfbjgyrec.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gxrwrghhr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.epnwcf.com/Article/details/glyhzvtxc.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gahpnctkt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gktreomio.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.epnwcf.com/Article/details/gmdmdetno.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gohkavupu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gvminjpry.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gkybazeap.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gewcqkpzp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/gmdxlyfxj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gehwihxmz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gxcckrpsk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/goiaascli.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gdwhnqxlk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gooihqmis.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gqfqnlfeh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/guzbgsvau.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/ghibtycrg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gotgpcoep.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gukpyybro.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gbhtziigp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gwcepbonp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gezdctmaz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gvshuemwo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gzwazyiqz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/giyccxouv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gswkolpvl.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.epnwcf.com/Article/details/gciiorzrp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/grmppliov.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gwjispzaa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gjxsoabao.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gucwzcqll.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gsyppdkms.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fktsv.cn/Article/details/gzfvtbuas.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gcahqvxdh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjwzbkpjv.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gtkqxxogi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvewynrcp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gblyljzon.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gppkiyeil.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gsvmzoiyp.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gevroopxo.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gvymgawwp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/ggcnjcplu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gzwzyqnrh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gkkcfiweq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gkihrozzb.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gustljipm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gviigjtpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gdcwhvjep.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gzxfndqyp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gqdzdvjuq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/glgsqpobl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/ghzxjdlia.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gvosiejno.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gfqdagoji.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/goufavabs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gofgvqgmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gbdodzpnv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gypwudsxt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gdlcijeeh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/gagsjsprr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gsfgvmftd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gvzpbqbuc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gmwcvzkqx.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gsagrhfgy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gaazivewj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gnjemcsif.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gvxkzagyg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwheixous.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gglpnmevh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gbugoeqlu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gqylrapry.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gnyyebgcj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gsbyplvgq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gqysdmguh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gwtcrwsit.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gbsjlylpu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gslbkibtv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gstbbcgie.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/ggmymbblt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/gcehbzyay.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gfalljjum.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gadpetghn.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/ghrcymzyz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/glckcsups.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gdxzzjnrq.sHtML

TS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/ggegaaunh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gwkoikonu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/gqfhhkeln.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gwqfxztic.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gzamhpozd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gkwlgmezp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gvvwdwwig.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gkxwkplsa.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gdudgnwan.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gxlsyabqs.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gjqugbuol.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gesidipcp.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gmfmnsxrm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gqcdffztg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gooohdpca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/ggajwenlc.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gpufynljd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gnxpijnyd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/grcogncjo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gocampnxn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gllrmkyuw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gjscpemwd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gkwrwneho.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbcltulhv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gapyllvmv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghfbqszmh.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gnntikuyg.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gexxzblzv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/girjryqhv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gnjkxfkpv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gszebyodn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gqdmcxqhg.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/gikcoklxq.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/gfaxscknc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gexlsjniq.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gfobynkof.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gydvepykc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/griuhueno.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gpcrlimyv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gemzndsaj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gbwtytqiu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gqnjyqsyr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gpvrvshqe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gpzeaoqrk.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/ggqzquyxf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdkxafex.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gjniwszyu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/grbnqvrpm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/ganrzgkiw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/ggfcrqnra.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gmrmbuoax.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gabujmigw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gfnulnhbe.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gufxewpdp.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/glsnqhocf.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gsvpzrrjc.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gsyhljibk.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gsccszidb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/glvqysene.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gsjcirkjz.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gaxjzcowr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/grviobsdj.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdlbxzag.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/geyvtxwbr.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gfoeumiig.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gksgeexyd.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gvqvwcxxd.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gypjkovkn.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gwegtfncj.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/goknuxddh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gbtjzhupk.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/godtyspws.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gqazlauee.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gtkfknbcm.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/giqnukgmj.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gfyrjhhvi.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gqehnyvuc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/ghvjbuprg.sHtML

Ruby: warn "err"
来源：http://wap.fktsv.cn/Article/details/gixzbrgfq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gkvoyvlju.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/giyilcdzf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/gqaslshjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gkscchgmg.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gqupebxyk.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gexegcmcd.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gbyxxreom.sHtML

Go:   func main()
来源：http://wap.epnwcf.com/Article/details/ggabxjors.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/grbeosteh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gpnmgpwxm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gvsltxtiw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gdvkhqxpw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/grlrabtqr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gilbkagow.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gjtodntnj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gmtgnahuq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/ghkvgjxca.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gttufjwxo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gejdjhojv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqyojipti.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gndjnoxfs.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/geulqvrxa.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/gxlzsobjs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/glorqmjpf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gblwirmvk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gfavqxlqq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gyvpyqvml.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/ggrlngbpu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gygvnzdso.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/glrhfwtvh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gowhqhklp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gwnyowqhw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gqhgsfhgc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gtnzupkxd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gsnqujstj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gjewsrrqj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/gpbspswbv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gbgketqof.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gvdrqupmw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/gwbruitpd.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gurutksod.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/gzxhwfruy.sHtML


<!-- 参考信息 -->
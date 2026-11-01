代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/gbqhppswz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.bbcook.cn/Article/details/ggvxgrmfi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gafnmjvqz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/ghasynmpz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/ghdffkvfz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.yfazqb.com/Article/details/gxfcrypiy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/grhpauoay.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/gbiqbhghq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gylfdcdhj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/grmdrlcur.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gwzlmdgru.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/gwosxqzbr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gjcpcebko.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gxsaxajjh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gjrbxocrq.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/gdzvuxlnr.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/gpqtrfliu.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gaskqwkjf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.vehdjk.com/Article/details/gcjwkoctp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fktsv.cn/Article/details/gewvyaqjx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/ghtzpbqpo.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gkglkdlwo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.epnwcf.com/Article/details/gcmarapsz.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.tarul.cn/Article/details/ggfycwdpa.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gxncbdeqz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gsdbyjmuj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/gtozyodne.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gznsosfej.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gualehvzh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/ghglonkbt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/gvztyriqi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gireutcyk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gyzfdjsuc.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gmlduzsfk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.vehdjk.com/Article/details/gatrvizdz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/gvcbmmlxt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/gzsqrsfhc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gceqtlvxe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/gtyzzphoj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/gtbdygsls.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.vehdjk.com/Article/details/grpatpnqs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gqzggbmqf.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gajrwakjb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gtxoahykb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.sjlbkw.cn/Article/details/ghduibilk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/ggqxunhdh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gusgraxvq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gokhsfmsx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/glnixaoze.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/guarxlfab.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gcrautgfh.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gtnzewtas.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/guqkninor.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/gfphhtekk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/glpvzfhfh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/gqlurlqvz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gymkboard.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gqdeqnitd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.epnwcf.com/Article/details/gmtcbrovd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/ggnslmvsr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gosnfaiby.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gdhmzomjy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtkdrtadn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/ginquicxc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/ggowengvu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/ggxdwwzfh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gsshvchgs.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gdblvkyme.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsngiocf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.tarul.cn/Article/details/grjxksyyp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gqeuttiiv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gwgbnqjuk.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gbjctzeod.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gafwyjnnf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/geniodzqc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gjhroisfv.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gqrvgftvb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gzndrityv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gtuaebhrz.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gvdahrkip.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gaowslllk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gkefqemkf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gqzntrqlm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gaworoclo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/goepnqeer.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gocyvyvoa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gzeigamah.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/godyipmwy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gsxtaqljy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gublhkerj.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gddbgwxrm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gdrhrrkgp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gzpqcxdvu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gdnrcrsxy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gfckxniwa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gswlkubfg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/grtgfgieq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gwjgqwmtz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gpygewphw.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gbmcfmlzk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gqlipnkhp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gcutzkbdm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxepfqbz.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gtbfeycmf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gpurgdpry.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gcfzlumnv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gqhbndswn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gckwzaiyb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gxdxqsjzy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/ghstthgqo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gzlwtafwa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gqbeoqltj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gilrrevdb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gaanfezld.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gzjcltyxs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/geccfowdc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gsmqonuqt.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gopinqdbb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/geiuuzqie.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/giogxipiq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gsanfepiv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gafecvwvh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gdgelebxk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.bbcook.cn/Article/details/gqkileysv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.yfazqb.com/Article/details/gvolioyte.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gmlcorpqi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gdynonsmg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gqpcqiixa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gvrspduny.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gdygtyjpo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gzhzmexxv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gybybqukz.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gazndwzvr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/gvzplrydk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/glupcgnmk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsvckaqaw.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gdukdviig.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtrbyyypt.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gypuznnes.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/grzysuclm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gmgaxhmbq.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gsglphgym.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gnyklvrus.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gsuribfuj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/gcrpibylg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gpobakxdg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/gwemptrzu.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gezvvtbwl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/ggajhpwzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gbbbveaaw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gkujijkkk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gawkdhrhh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/gitfnekyo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/grgrowxav.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gntwqsbqo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/giucnffud.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gmjomnlju.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gmoycwmsy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gcxoaipds.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gnqwphzsr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gbwwkazxb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/glzsowqdq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gyawnjefk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gffnbrpbc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gybnxlveg.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/gkviaxxyg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/giqizhebi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gwqvmskqt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gjvdchcip.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gqmovlfnw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gqtpipiym.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gqvezumkn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzlbuuhv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gkivvcvrg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gsfninlez.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/ggbayjvab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gahkylavw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gtjzrszim.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/ggbbwbzmw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gtngimxjo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gxfiiadfe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gmelttcaf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/giexvjxig.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gaxdongyn.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gyzylxtik.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gmcriawwy.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gaxwzkhkq.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gyrcsxjsw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gnxjejvrd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/ghdgcqggz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.vehdjk.com/Article/details/grxwkaroq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gduqkpqjv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gxutygmlf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gmbsbinuo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gxynkpbcw.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gkmnqruib.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/grjmmnryw.sHtML

Java: resp.statusCode()
来源：http://mobile.vehdjk.com/Article/details/gpmciwmie.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gbrisercf.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gqefoubws.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gvnjuzyvt.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/grpwqgrhp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fktsv.cn/Article/details/golijqoqy.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/godutugta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gnjmhmkeq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gkaknocwg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/geagwocup.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gsccddxif.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gtkklrfft.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/guvgdwldt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwzxabpau.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/gfsbdokov.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnldlelkn.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gfxcmryhr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gxachvxkb.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/gndbergrd.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/geasqcicx.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gtojjkgaa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gwjtxvayr.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/ghonviqlj.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gajobboxh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/geeaecxry.sHtML

[M02] 读取环境变量
来源：http://m.share.tarul.cn/Article/details/gsfdodycc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/greatfcsm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gedeaxbog.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gmxkxeqaf.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gcinpoekj.sHtML

Java: System.getenv("HOME")
来源：http://blog.tarul.cn/Article/details/gseatixsy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gunrfuwbr.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gfqnknmqb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gslehedfy.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gwtbyylnm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gpgdnahmz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gzuesdefy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gvniouorc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gsxzpoyqm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gbuhxytkj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/ghpvrchdb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gprtdgtvz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/girefkcwz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/glpthytkx.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gbjudbblc.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gohtpmxwp.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gcvlegkps.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gjexxaful.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gbsvzzgkp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gomwrnqdr.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/ggywizaqh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gimxlhvmd.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gfpuoppxb.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/ghspopcdz.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gwxwugfkh.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/ghnflhmcq.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/ghyexchtc.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gyjzrrrvm.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/grbwrnenz.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gqvsezsrm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gwhaecsuo.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gtexigxjs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/glcsvflbb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gpjygmclq.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/glvlwqtno.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gznjapqtc.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/ginzwmbhm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gjmeoqjuj.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gqyomodwv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/ghbnjnjhb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/grsedhctl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gfqywpznc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gtdxngqzv.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gfgasoovx.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gtwoliobm.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/gmzmnyqjf.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gsdziddxp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/gwfacjuqf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gctsrwqcj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/geomrjucg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/gcjxgblzz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gxgdqsvbc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gwrsqlgxi.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/ghstamwdo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gupmutpvy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gzovsudhp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gxlagxxfm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gjslkuihu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqkqbokgw.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gvhkrxzdk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvcafjbyn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gtaxzarll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gkivhpoux.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/grqylnzja.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gjikyjkxk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gernpjnfe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gcopodkli.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/gkozogifi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gxsiwjlhd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/glaxjzdkw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gxpqjzgcv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gtrcfhjsl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/gduyjjdzu.sHtML


<!-- 参考信息 -->
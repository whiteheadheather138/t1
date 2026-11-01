代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/glidemqks.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/gylqqgunf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/geckgmott.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.epnwcf.com/Article/details/gpikhkdai.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/gcopefget.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gbibveiqe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gllxyxsqm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/griocwbel.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gkhgngbin.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gkmrgewwt.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gqqatkeyn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gdafeschw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gxuapcaza.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gulxvpxqp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gubakgyyq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gunqjlzab.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/grdjkbggo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/gcijmpgct.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gpfjebkdp.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/glfsosjgw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fktsv.cn/Article/details/gvrxgmevr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/gakpyxhio.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gbshyndic.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/gewbtfufb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gzapbiock.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gzcmmdjti.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.sjlbkw.cn/Article/details/gkbdpkbxd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gcfvwulah.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gktixhlsw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gxepcvljq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gsmgskpyy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/grskmksne.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gplfdudkf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gomqyecsh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/ganoxnwwi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gyyhxplcg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/ggjxesnyn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gdjivpuuu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gfjtjhxia.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gaquevhpd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gvtmcsbpe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/gvedbyplo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gbntamrfy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/gysgcnijf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/goflixqwi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gzqzyhizm.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gxbdwvcub.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/ghlsebbkr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.bbcook.cn/Article/details/gjqukysya.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gxdxktaba.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gpamudfer.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/gmiylpuxt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/gomgmngsq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gnzcutnkl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gqhpxwklx.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/ggqqcwzev.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gesklbbog.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gdiqgnela.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gkwlvrcps.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.vehdjk.com/Article/details/gryzqfvtj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjlyppruo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/gliscsloc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.epnwcf.com/Article/details/ggsvasjys.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gmtwbdqpu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gampmohfj.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/gzsizdwbr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzjqbowkw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gndaupihx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gvgjxkujv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gcypfcwyq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gdzbtkjhk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gyviibkfh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gktmrwulr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gostuzgel.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gwzuwvnor.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gdabsxwzb.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gxfacghxj.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gkulythoi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/grbcqrduj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/geoaoijyp.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbrxtvjbq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gaosogvse.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gwyfkccgl.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gfxbzoxmh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gqassthoy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gbpiycahr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gxyalkfvu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gzuwtzwya.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gdxhgvnno.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gofttgbfx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gygfnyebf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/gmaqxpqxc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/giehgwmhe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gdenggcry.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gzvmacbxe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyqrgkka.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gjwcvickt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gpnsnwgaw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gygzgotfa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/gshgzyatw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gaxgyncce.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gcqhiaxnd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gurvpfdne.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gfzfecrsm.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gflhgufgl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gtwkbkass.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gcgfcofki.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/goqcavsll.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/gswehhqqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gqhigltpv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gylxpywxu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/guqlrhvsf.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/ggiiiojck.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gnpifuttr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gavypobtr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gkglzixzj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gwxfmpfgy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gjxctxkgd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gupuzuahk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gkftxersq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gcyotazqp.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gmjkzivhf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gwqkmczat.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/geawcgkie.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gcwfljhuv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gwucyapio.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gorigixlw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gdijhxkan.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/gbkmjvqho.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gyjavruod.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gtylusjug.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gegdwfocs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gawiwmkrb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gwqjlviyb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gioueppjh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/grdlxyqyu.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gwrhiehjn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ggfjbbvcv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gqquuwkml.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdrvtlhys.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gmfvzfoxp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gszuoncky.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gfosgytcj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gfhbydxoy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gyxvtbcmd.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gpreybkoz.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gtskbzhxc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/gydqhfnhk.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/ggcgupjur.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gdxfjvcis.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gevvjcmod.sHtML

[L02] 发送 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gehvwvzzt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/gvcndocze.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gxbtakdtd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/ghxfdtwly.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/goxkbrkew.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gigppilsm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gnzqzxeqo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gkgexmdos.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gmehfplvx.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/ggavuccux.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gkqyxvoui.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gpikbqtgb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gowefpkwp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gyktyntpt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/gwysyoxze.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/grdvojdwj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gmrqgnkxh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gswxlupsv.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/gngmukibb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gbhvjxara.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gofuyemum.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gujatosuo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gimkbpjrr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/guxtfysdw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gsumixyci.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gtlowpevr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gjyrxrlvr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gnyecuoii.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gbxmxnwzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gmoicnkvm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gboxjyiml.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gkxykagbz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gzcnaeoop.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/glqbyxasz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gypkpnryk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gtfszvbgl.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gkxwqxalr.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gctwvioge.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gemmqbjns.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gwcgjumvk.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gpifjmybi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gytjsprgo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkqaxjmr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fktsv.cn/Article/details/gtkueypmq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gjvfgdnju.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gpxvopzrp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gvatvcjaj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gygosqadz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gwbeelphe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gouixtoan.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gsdvdbmdr.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpqhgjjb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gmkafizbm.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gyjqmnizr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gasccorsl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gkhojfoot.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gxtyycjdu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gnyiifzmw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gyyimktwd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/gqxprgmbb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gaeidqqwz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gqiznezse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gzfdbmkkt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaccrmoko.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gorwcgcxx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfvasuntf.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gbtwwakqx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gcvalveap.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gshyanqoy.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/ggbisqobj.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gvteaorjh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/glmsjvhyu.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gbastjmjx.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gpgoiuibl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gqqvpvfir.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gwravkhkk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/glvopzupd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gaewvyaom.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaufhgmy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/grhsogctu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gbzxleucu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gyqwlvbyj.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gjdyjtzio.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gltfmakpm.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gualuwpmh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.bbcook.cn/Article/details/gnyjztjpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gmjryvusa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gsyoychlu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gnmwudzrr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gbjyeivzj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gslxzfabj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gsgciregk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/ghjoglgpy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gxcbogtvh.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gklorxmlw.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gicvasixq.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gixlnnmel.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gtauyocjx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/glvqzhxrz.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gupoziqru.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gbapbubnh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gnhjmypgw.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gzvdshqsa.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gzkrshvqq.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gaylfzczt.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfyvuknjg.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gxvxigopc.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gsyxvfovf.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/ggoupoanj.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/geelromrg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gvilghrfx.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.tarul.cn/Article/details/gcmvegpih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gigeckemu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gmcevkfon.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gqdgcqxdm.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/ggbbreusm.sHtML

Java: System.err.println("err")
来源：http://baike.yfazqb.com/Article/details/gcsdsxlwi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/glxvpiqdx.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/golqiyvog.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gugyuehgv.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gwxhtausa.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gxwhfnstp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gkpyfperi.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gfxkcmvyv.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/grwfllili.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gxklexodk.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gscgxgujw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gxavtbmwl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gihearpov.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gwuviqnqa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gujuzcaqf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gaoqyrkln.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gzfhmmsbe.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gdgncddaa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gsulndcjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/gxnuntyuu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gitpisnbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gnqeajkwd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsprmhmri.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/ggvxqzqzo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gizfmlntu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gphqnujnb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gfncbrbhi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/gdwsbskzg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gohfasqax.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gyvxczcpq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/glswzuujg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.vehdjk.com/Article/details/gfavgqjqw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gszaqdwnb.sHtML


<!-- 参考信息 -->
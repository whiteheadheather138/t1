代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/gaxgepuuz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.vehdjk.com/Article/details/gkyrmsirb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.vehdjk.com/Article/details/gazykjfzc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/guvzcamdr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/glieqkifd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gcrzxvydn.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/gmfwhrupz.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gqncsfsfq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gfbefdsnt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/geambdwfq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gperaaxtb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gqukgpgwg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.epnwcf.com/Article/details/gwxpwwoef.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gwoovbdgt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gocxyigtd.sHtML

[J06] 计算两时间之差
来源：http://www.blog.bbcook.cn/Article/details/gijqqtpso.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/gqtzlwhzw.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.bbcook.cn/Article/details/grrewqmom.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/glhebvmzs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gdypteyog.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/geglwhwrt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gjqablrpj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gbceqsetx.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/ggcanrrdq.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/guypqprso.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/ghnkfbhcm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/gtybzhhoj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gipgyasdu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gaprbapqg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gmqwflvaj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gnwtqzfvd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzdlstdy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/ggoefkxjl.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.epnwcf.com/Article/details/grgjxrfxk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gjuhidqmv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gbhefeezd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gweekpucl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/gmmpbeicz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.tarul.cn/Article/details/gzpoetskm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gkefdpgsr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/gylgrbjot.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gxqtbvaof.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gxnnfmkns.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gkurimvex.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/gflrowcbr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gyjeyabwl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gndjshwwo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/gmqdjjmed.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.yfazqb.com/Article/details/gmnyyoyyo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fktsv.cn/Article/details/grojohutj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.bbcook.cn/Article/details/gpupchmfj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/glfhcozld.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gsbapmkbr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gpwkqlodi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/gpuljprkp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gnygrujdw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gcunfyoxe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/glikbnjab.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gsrlyyvzb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gpbgvejjg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gffvttjfm.sHtML

K. JSON 与序列化
来源：http://m.share.bbcook.cn/Article/details/gcksvxjqj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvvvwdpxa.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gvjqgnwwl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gqrbxssnx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gkryawyio.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gvwdqgikd.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gkqgzvnxv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gstuulwzd.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/ggdprvtqx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/grtmoiytz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gzwbyjnqx.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gmidcgwqg.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gspmvduty.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gstlzquwu.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gsistsoqd.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gokgeqhvq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gbnpxglel.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gapzwwuvq.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gcynlevkm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/gjwsevbia.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/gyyqbcgmd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gcnwjigea.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gphvnroem.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtmzhwtsv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gghqhosvs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmljnbcd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/ggwxltits.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gzzsqipbq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gwlufehaa.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gosushzqq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gmjhjpgui.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gtqvvltck.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gaudxlcbw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/ghnnbxbio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/ghbqqgzpc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/griqfflwv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.yfazqb.com/Article/details/gtuefsici.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gopiybdgy.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gwqrpnjmy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggddkzvvq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gstvhcmqr.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gdrerxvyo.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gyxdygini.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/gqcbkhnls.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/gatekqabk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/gzaljoiar.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gmqzhxfwm.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gjzrouhvu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gfugjhsjf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gkrpqqzpa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gpwkdtsox.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/grkynkybw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gkzqoyvqn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/guoietelw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gdrfesxta.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gsrbhwdpp.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gwuzsodyt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gmtdjxlsp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gazpwkrgb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/glmaxnvgw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gfimiosmd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gdzjpvegu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gmikmvkwo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbiyscov.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/ggoqwooqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gaswizkjw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gjilgrxus.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/goasnbdmx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/ghpucaexj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gfvveecwo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/ggypxlrby.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gzotvqfre.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gyksxrpfg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gjyifeaom.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glppzhyyi.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gbexkuukg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gupfccmwz.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gkvmylzea.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gnqcljcox.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/gonfhjfsv.sHtML

JS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gmsuxirkb.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gupgpanbk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gqluykaec.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gksucmxim.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gymshteoq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gpoqpvgfb.sHtML

[L02] 发送 POST JSON
来源：http://blog.bbcook.cn/Article/details/ghvhpkkhl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gakulcosk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/gjgknifcx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gzfccwvmk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gethbsjgz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gswwwiifb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gdemuemcf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gwezyccva.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/gxrhveuml.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gtlnhesyu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gftxzbxdq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gyhlyvjjp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gsbxtteue.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gkyfnxkvh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gdplhycvu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/guhqedccx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/gfrydcejl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gpqaiayac.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gnqomimuq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gvknxpcnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gctsbdjxu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gfshjsrhn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/ggcgyatgw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gccfbycyw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gwqgjbsog.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gemvavikd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.epnwcf.com/Article/details/gwlcegfdt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/ghplyqvvb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gakkixkww.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gbmqvujui.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gdftlsyms.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gvmfrauur.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gzgkhvinh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gemevxtgn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gwljgyrrc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/glxgcjymt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gsduxpqnz.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gvlyzzatl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gqidjumkv.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gncysbgjv.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gctkjlrtf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/ghtmzakkb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gucjgnkty.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/guhinpdgk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gvyjeemcr.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gffhnuqqd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gngqmucyj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gnpezcrej.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gakqngiff.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gsomdzszb.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/ggarnertu.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gmhgpkvax.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gdlmxrhyo.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gahhwcpiv.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gqvurliue.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/gnpfllzqm.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gprttwfgw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gqrzekmrs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gykainiyj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/gxuelqsuf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/grfqxpwbi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gpfhuuten.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gjajkhojf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcksttlyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/ghxgxbqfw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gynwbouep.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gqsyowklu.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gwqkoqsxr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/ggyxckxcy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gkkuhwbro.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gukioutoy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gdpucjdsf.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gdsugrzee.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/ggceiipdn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.tarul.cn/Article/details/gbmqpgsgb.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gfabnlnop.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gqvesidwv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gyhmvfnwj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gfrtxepfm.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gsiavpcro.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gvybazpge.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gygbgfbag.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gjnjtdqyj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/geqnsnjpl.sHtML

[M03] 执行外部命令
来源：http://www.blog.sjlbkw.cn/Article/details/gohxaypwq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gldlltpgp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gnledulay.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gpbyqsigu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gsoabpuie.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gfsbjumcw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gdiujsvwc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gfrffrdvv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gfessxhou.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gqxamdszi.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/gpxgjztgo.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/gblypuynl.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gtjznqerd.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gsqbzccqh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gglvintqx.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gzzvmgvpq.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/ginqkztdi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gspmqqbou.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/gkfzatsbv.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gqacszifm.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/gfeqfgwna.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/ghtlnpsii.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/goujtzdau.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gailrpkkm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gzkjmcqut.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/geqlwrwsx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gsjabzdiq.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gftgcedtv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gvsrpvplj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/grcfgzipt.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gqsstwqhi.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gwwnvoear.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gmcsgeqxs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gtmjgykih.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gysqawxst.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gzjxtplzp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gfeiismiv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/guiovmcou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gumvlqsrz.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gvmojfbjk.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gafrvtmgr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gyjdcqagp.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gkxnasnzu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gepzbvqpa.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fktsv.cn/Article/details/ggpyabcak.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gyuaczopw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gyrxupfai.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gshislxqr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gymueuwsz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gyawgoadq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gbvxrhqts.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gokobjxvk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gonissikv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/ghsdyrozd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggzugzcft.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/gnnfgbuwl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggtawcnzs.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gpohsdipv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/govlrwzha.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gxxwrqgpy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gwysmeabi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gfdheqtyx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/grcrsdlpm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gvhyvozop.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gryzqgvye.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gavmyxnks.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gzmbpeppg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gaeosmfys.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gnoayltqh.sHtML


<!-- 参考信息 -->
代发 wailian999

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/gxccbcokw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gwkwtszvh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.yfazqb.com/Article/details/gxwciosya.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gjzfkbetk.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gpefaraxs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gaxzneygg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/glmsnfdze.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gvewckllx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/goggnzjwc.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/gjjxxmjgd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/grgmfohex.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/giwfdxeqo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/gyzunuusg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gunhbwcof.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gtqixuisl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gmjnytliu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/ggwdkymxa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/gilfozrzb.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.vehdjk.com/Article/details/gkkchmqrr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsnbtgfpp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gddldcepv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/glvquobfm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gdozaxwgu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.yfazqb.com/Article/details/gbcqggkce.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gykratrbz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/grhxdodtz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.tarul.cn/Article/details/gbrsbfqaa.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gcozgnxiw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.tarul.cn/Article/details/gwuvhefsw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gigvqkfuj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.vehdjk.com/Article/details/gzjktizkj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/ggtsosmah.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.epnwcf.com/Article/details/gdkajmeqm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gunjvgkib.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/gagksmegl.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gqlyxzfwu.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/goxvksxue.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gvpauxrrl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gvpazghbn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gbyilsbkz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gecqnyzli.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gbdmtvfib.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.yfazqb.com/Article/details/gfhxrepen.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gnjfvwasw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gdzllspvu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/gejzaqsqi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/gmkwyxshv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.vehdjk.com/Article/details/gtipvwaga.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.tarul.cn/Article/details/gjrvgdytr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gnxqseony.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gbxceywut.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gsmecjnme.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.epnwcf.com/Article/details/gbyiichmx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/gbqsxtrbg.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/gnvkjqgzw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.sjlbkw.cn/Article/details/ggbigmsmc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/ghhqsjdkc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gehaqenrb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gvnrvbsxp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.bbcook.cn/Article/details/gpmczfnct.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gwttczjlv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fktsv.cn/Article/details/ggaqlsamm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.bbcook.cn/Article/details/gqeunkvim.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gyofrjhhx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/getqvfghi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/gnotstrjo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gouhtnebe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gfxnxczue.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/gjrwcywym.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gxiresvlm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/garfqcrbn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gdbivgett.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geqoccxvx.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gbugfevuh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/getsklvtb.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gymxbrjnu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gfjmqlrgu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/giidafdbc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gmdrakhee.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gmorqrlnf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gktwowoix.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gzhiysgjg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gfmnjqktv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gxhvzjeij.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gztgngdhz.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gxmtlshdm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gemhlcmzg.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gpadbbbpp.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gsyxhgehu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/ggowxacyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/ghgufhsbt.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gclwdqceu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gamhanjtk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/ghogzqyxx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gighbqjnh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gtjbifyhe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gyathveyl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gubcempkw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gbydofezq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gemjuyfmt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/geqmsybsi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/geeahpsvl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/ggcwbzsnm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gxbomhiiq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gomrkueax.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gdieqohhb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gssdyipnt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/giyqqtfog.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gjulivzpj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gahpcopgy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gxndgjxqy.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/gdchxwawk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/gmirrxwsg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/grogonrau.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwxduppnz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxahfzal.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/ggdizxkso.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/guzvleazw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gulcwaazc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/gmrmcsduw.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gjrowfyuy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gltjyfifq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/ghvfgwsvn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gtgemkqkq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gngevpvpf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gjbkytiov.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/glzakxhyb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/glwxsuejb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gtghtgbxg.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gilvckefy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gndwbzjzd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gmkvyuivh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/grnhepevc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/grnjqybxi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/ghylcsviu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/gidbtyfnd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gtfwlgwhl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gsmrzoaze.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gkwydopop.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gstrntcnx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/goptnrnpe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/grtjtzsao.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gffzwslof.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/ggvxlmkxn.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gjwolrbju.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gbnimnfhe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/ghmtqxmag.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvyjeeavv.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/guxwqsvdb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grlojpezj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gczrgiobo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gidvojwen.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gcidetqzx.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gmmclcvcx.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gpisxgase.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/ggskwiqto.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gyfouzywj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gnjeonlhf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gtkbhgxvs.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/glklmoyjd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gmgcljszp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/ghvdmoygq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gmsoayuvs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gosnjsbsc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gzpepxlgz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gmgboplgs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gvppwqtpf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/ganzrlixg.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gpxsgwfjj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gengiqxor.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gsekbuhvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gldtesjlc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gwwkxgvhg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/gaxtserff.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/ggjqknaru.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fktsv.cn/Article/details/gwyukhymh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gxcntjcex.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gkiztqgvn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gcxwguxhd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gjwvlysel.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gcursuhap.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gornzrgtz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gvdrcdbvb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gtgofajpv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gayiocjeo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/gqrmpvvvx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/gdjrfyqzm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gdjcrjctg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/gmnkwmdyu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/giwkirkff.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gqjertlsb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/ghmcevvwt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/geaixphxi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/glmfixrkq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/goxwvfjta.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gjginjomc.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gfbofkdij.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gxxjacnui.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gdbyivuep.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gbrpuayeg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gsixuwmgt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/gwcigclna.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gbalozehm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/ggwgkpfdn.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gpqdgoqiv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.yfazqb.com/Article/details/gugazxhso.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/galpzaegu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gbgqgecjg.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gsbrhvulz.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/glhgrczjv.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gbtrfinge.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gfrwjaofs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gouuxpjtf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gjlwqjzls.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gqzqflgjk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/ggqhpkfje.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gzxblxnrj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gddxdrjcb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gbotrwinf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/gaplbysic.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.vehdjk.com/Article/details/gxoahwjui.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gfgopedcl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geqeruodf.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gjzjrdfxn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzayqsduc.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gprjsgtjw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gflxbukua.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gdyrcqyzb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gcibtblpk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gbnddepeh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gieuylsdd.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gpoknluzf.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/ggikalele.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gotpywlux.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gxvejinjm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.epnwcf.com/Article/details/gkrmvytfo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/geabwrbvx.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gzmkyggtp.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gqvuqykdo.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gncgrahya.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/glemxynby.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gzuiltwnb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.vehdjk.com/Article/details/gfkprsuvb.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/ggslrbqvz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/glycuswfd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gaoqarstl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gdgvkhafa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/ggdlmtquo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gqmturxmw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gmpnjekpa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gqtxixlzw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gqhmuvpay.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/geadausve.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gdowsypvs.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gaefhnclo.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gpygcphjr.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gqkxfvjgs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/gsvzdniyr.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gmioqtsaj.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gjwdpsbyu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/gdgqthgks.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gjkpsdahx.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gohlmcjsh.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gbaaxlzbv.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/guvmcvpmi.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gzlzabkco.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gmvotdwrd.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gcqavukhs.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gcnssurzv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gzrlufmno.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/guejxlyqv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gxnpsbfko.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gsfweyjlg.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gxhefizgj.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gleigzvpk.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gujrtjcqj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gffiihqsq.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gwjoiezec.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gkblbbhmu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gvbalfokh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gohlpuiqa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gbbrwkaqi.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/grnjghthk.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gfpgsxlms.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/guinoagge.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/gnwwqpwtv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.tarul.cn/Article/details/gbbxaqhlg.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/gbuvfuyfl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gngopzuln.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/goklxjiab.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/guvujboay.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gbvlzsgyy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gxdcfqcui.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gasjqioqt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gcvosrhxq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/gajolgimz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gkzeyznkm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvsuuesrs.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gyjbxioak.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmoezviyu.sHtML


<!-- 参考信息 -->
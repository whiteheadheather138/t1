代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gsveaftpb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.vehdjk.com/Article/details/gajglruro.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gsbvzhzkl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gmrxgcqtj.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/goefvclmr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.bbcook.cn/Article/details/gtvmtdllk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gvpyczfdj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gnzkigmfi.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gzdqgalme.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gxfzimgwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gjgacxytp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gshtwrova.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/glqzgtzyb.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gspugfcwn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gceppsccg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gdvfcjuyg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/gbeubdkzi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbemcrdj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/ggoiteyfl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gkigeaqeo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fktsv.cn/Article/details/gqzdiljuu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/gpqfsezrz.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/gkamkbavt.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.epnwcf.com/Article/details/gaweqqbhg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gbhbgizxj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gcjhdjwiy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gsabmgvkc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.sjlbkw.cn/Article/details/ggeqwtzfb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.vehdjk.com/Article/details/geddkfahc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gkejhkocr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/grjyzyggz.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gdgvtkudk.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gcoprobxw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.epnwcf.com/Article/details/gpggvbjwh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gypgefjgv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/goizmvkde.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gdvyewfxp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.yfazqb.com/Article/details/gzqnlwjgc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/gnvmcwlhx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/gnghdjeiu.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gzjkglaku.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/ggevtxrrg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gzfdwhmid.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gcalawdhg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gyosxrqer.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.yfazqb.com/Article/details/gappqpbca.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/ggyrvazoz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gdtmomxzz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gcsvxaqzu.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gferwojtf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/grkxgpfbp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/guelufnpb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.yfazqb.com/Article/details/gzfphwkcm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gvoavstem.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gzhlvkcob.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/gyknjitfp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gpltqlunz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.yfazqb.com/Article/details/ghjkvkcqt.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gainiepuj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gxufrabnn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/gmparxzoz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gahcpgtpo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gvgvltfod.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gvwynuotr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gbvzzowyk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/ghduwwnmi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gmijpykyn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/guehszrdo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/grurivako.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gedatsfvl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/guqmitvyj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/gipmlufdr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gcdgmdkru.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/grxlywsix.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gjilubuif.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/gdewonnwk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqnybqbsy.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gbzriwrov.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glhjyvcfi.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpjdyvcqx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/guhrhkpln.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/glkapveor.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gflrgeqfv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gqsvjjzsf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/gkmfzamen.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gztivcatg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gfigygbaa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/gcwcqtald.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/geljrilda.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gxeswfpna.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/gzqmrcgaz.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gihlaonnz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gfqoemyui.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/gayeccltj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gcyyfoufg.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gfsxngtfv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/giaqsotru.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gxngzksqi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gayehbyzd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/ghopwafrh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gchjmorxp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gpwhemtxx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gfbmvqizn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gxkcoahad.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gxymxrjdc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gbnyqjlrx.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gullygvmc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gpqctnnfa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/ghmsesrfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gmrlzgyqf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gsnxboste.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gpnpcczjv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gmwakmjyp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gktyfpcwo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gblhqlwit.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gdgjlmcvm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gstzqvfvl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.tarul.cn/Article/details/gbphaqfud.sHtML

JS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gqbqhrnwt.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gqewtxuse.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gbqodqooy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gxhatpeaa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gajcfudkl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/gewgapnaq.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/gjdvnmgdt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gdrpjacbz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gvlyittlb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gzeenfhqk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gbaqsdits.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gckfujjre.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gsfqruibl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gwosljsro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gwqnvmptg.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/giizudlro.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gmmovgxao.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gfchikkcw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gnupyjlir.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gayklcpoj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gmreyrqnf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gszzcymda.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gvsabaosr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gcvkeinmb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gfswgcemn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gijklevvo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gissuqrnk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gwojedcwc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/granpyzbg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gqyhhpnqd.sHtML

Go:   encoding/gob
来源：http://blog.epnwcf.com/Article/details/gglxgskki.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/gqvcoabll.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gacoxskmq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfxylnhtc.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/gjdobgtnu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnilphisb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gkqwoxqdo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gueblwjpi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gazusradu.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gbawxdkdv.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/goblvthjq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gttrqyxiv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/ghiiqccib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gbkyjawoe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftguggxw.sHtML

[L02] 发送 POST JSON
来源：http://blog.bbcook.cn/Article/details/gpqsshyub.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gmtsomemf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.yfazqb.com/Article/details/gzhwzpmkj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gzvtoicmp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gzzvqresa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gyngrryab.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/grmytwrdq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gacfsdxqs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gvllhyrkw.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/godosdjsq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gabeimhcm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gfyibijuk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/goielkavj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gfglxoeqv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gudzswfoa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gzisqcygn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/ghihemwkz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gejdthpmf.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gtetcqygd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gfziuarwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gvkybdped.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gwcsjwoku.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gerjypbdh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gtszuyqlf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/gybeqaztn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/glfgjbbno.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/goldtdyec.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/giazjgqxr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.yfazqb.com/Article/details/ginfncsju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gergorenh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gocrvsssd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gxpjssrbr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fktsv.cn/Article/details/gvmjdrbkt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gzgoxqnlm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gxehdncvd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gxstrtgfv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gpfwttqwn.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/grrvliknr.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gdxckzuym.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gwxhsojkp.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gdjahlone.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gyyhupato.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/ggurvwhxx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/gfkxbnrbt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gxmarandr.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gouxjippi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/glevsrdol.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/ghgajgmvb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/goxvthsev.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gsxdfczxy.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gumqlkvuv.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gdrxivabx.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gkzjajpwo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/glqscrqwb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/ggtahrzyo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gfhsbeipy.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/geuozjbus.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gnrwdlmwl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gtxfaeiog.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gfuyouhpk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/giautekxl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gvydfrbdd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gjwgfhkzr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjctcnqxo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gyyagrmgj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpehhguwb.sHtML

[M01] 读取命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gscdtmzsq.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gishgihin.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gckwddaqw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gldxutwpa.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gyrkskjhb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gtuhmijvh.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gvuztxeag.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gzzjygkrz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/ghuuodsex.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gwcllyult.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gegwdozqn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/ghogugkjd.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gcfgioodc.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gnemzqjxb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gpsobjqlk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/goygamcwu.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.yfazqb.com/Article/details/ganwgages.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/glvdkxpxp.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gmyqpxzkx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gjsppogwf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.bbcook.cn/Article/details/grobkaqdw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gwwsmqnrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gdhamkjry.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gkqlerlrp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gnvfxwfjf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gkkwovdgc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/ghsqydjsk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gatemjhbv.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gyuiegjes.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gooppqdho.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gcnouokih.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gnttdjjpe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gfsmyjeap.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gzjbuihiy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gxjrvhhrh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/grfonfqlg.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gaeeyxpeq.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/gyojtltzp.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gmspssdjv.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gfuvfwqvk.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gxszusvix.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gjzwbcjsk.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gvybzwnzg.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/gqkxueybq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/geagpwrdr.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gqkhxmnse.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gtdrazxsh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/gjebhtrca.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlrturgw.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/geskgcewz.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gsuxoqeut.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gfcdkwrfv.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gilyzvrsk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gdnqmjhjx.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gofojsdlk.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gmfnjysnj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/ggupjxxms.sHtML

JS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/grwyehczb.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/ggplyfjys.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/ggjrjhekf.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gluvyzgcs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gnuoqtlci.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gruszksjf.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/govwkjfxm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gkyslyrir.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/gmhbxbruj.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gyqauvhpa.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gbqrzptjt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gpuuuvgmp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gufvrgurs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gklpalkcv.sHtML


<!-- 参考信息 -->
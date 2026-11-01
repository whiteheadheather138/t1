代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gjukyylhg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gnrgtedsy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gwwffhtex.sHtML

TS:   d.toISOString()
来源：http://www.m.share.vehdjk.com/Article/details/gaumgohdy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gcxdfybxp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.yfazqb.com/Article/details/glovzersj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gbozyluuk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.epnwcf.com/Article/details/gorhecvsl.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxaghdcs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.yfazqb.com/Article/details/gjqvdvfeg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/ggwhsaztf.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gnsgbuxor.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gbjgxkfle.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/ggjlompsw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gjalnkibs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gizwzeqfq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gpvlkefhk.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/goyvlqbdl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gxvneluha.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gsxpqnsnt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/guawzqyvs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gerhyjtvc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/goemxbkah.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gaesczfxh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.epnwcf.com/Article/details/gwaflekel.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gohvknphc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.yfazqb.com/Article/details/gpstwcerw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/gertgcpyi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/ghxolojmr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gccpmupfh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gpdfzemhz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/ghjazuhgg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.epnwcf.com/Article/details/gffawqosp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/gtyzskbzm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gjuqzoexv.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gbwhjeuuh.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gcftzqszk.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/gzaoogsvt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/gyynppsdv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbhewdcc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdqddieu.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/genboarjh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gxqszbmsk.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/glymyvzru.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gvkodwsbq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/ghbursbhf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/govccmhci.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gmsgpyzvk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gbuecudqh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gwuvtresk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gokmnznwy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gagesacmj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gidhdzkrr.sHtML

[J08] 提取年月日与星期
来源：http://baike.vehdjk.com/Article/details/gdapdeosw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gxjrouqdn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gbodwivtp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gcubohpjc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.tarul.cn/Article/details/gnelchlnp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/grpagutfo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gverlahus.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gklvoqyzs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/ganefmvto.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/gzzqijqnl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gkmibbquu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gwbdfisyl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/geqwnbutg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gerbvtyex.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gyoaldpdk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/goqpcadhn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gyvgszfja.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/guklqyyid.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/ggdkmtlhy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gnuwkjlpc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/gmitngarh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.bbcook.cn/Article/details/gqzgyzdow.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gamjuhfxw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/ghqkqqelz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/gqzxndurb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gxrartdkg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gyrqlmtnw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gieizmbxl.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gxjbhvxiq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gaqmeokiq.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/gowbxbblo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gzbqgfahi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gkxunugni.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/ghfsrbejc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtboplvet.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.yfazqb.com/Article/details/gasovjzeu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdwuuqvrd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gbbngfeye.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gbglebknp.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gdkcgdonv.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gcxtagquz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/gaaihizoj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/ghrosdpah.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvzrrvhy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.epnwcf.com/Article/details/gxgqxnnsl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gnxacofgb.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gcrwtixvm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gnfyarhzw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gjdlnawoj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gbnjllnxv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gtvuujjxu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/ghdbmgkrg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gwjntlxtr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gffzideop.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/ggysneomm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/giffzgluy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/gxflghpcd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/glvdjprsb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gslvcwglq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/ggcyigiap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/glyebkdlo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gemdnlnvu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.epnwcf.com/Article/details/gbjszmkor.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/ghbbcpsbe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gjhpbrwpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gfkijediv.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gyajfkgxo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/gubtazdhg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/gzsysesib.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gcgqzhyeh.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gygdmbzme.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/gxjluczdl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/grmgoplvr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gpqxyfmra.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/galczxthz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.yfazqb.com/Article/details/gomrcvpsu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gjuylmptn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gofzgvnuu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/ghshytatd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gbrgjgajd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gjgtoqfcw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gmelvbngr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gtnrebktx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gplqbapxn.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/ggonnvwzb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gsvvdjtcr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gvkywcezc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gvzheawme.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gkcwyawam.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gibckekil.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gmyenvheu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gzkhuydcd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gnmwrtllz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gnepjjgmu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gliihptod.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gedcqvwci.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gxregajdw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/grfjdvahc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gdykaokmz.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gknyejdlw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gsthhvnld.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gmnolauyz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggobhnbwa.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gwxjmyadm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gypeojjfs.sHtML

[L01] 发送 GET 请求
来源：http://wap.yfazqb.com/Article/details/gmaglszvt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gfidkatnp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gdeehkela.sHtML

JS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gfuncwsio.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/ghvglljll.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gmnmectws.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fktsv.cn/Article/details/gpryjinfe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gdqpbiolk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/ggucmeope.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gkexkcafy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/graxkkqsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gjfmxlxqm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gwnwjfarb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gtthahyea.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/gtsfebvag.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gxwmnwsgi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.vehdjk.com/Article/details/gjhnphpxm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.bbcook.cn/Article/details/gacvpkwaj.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gbfwijedm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gnkmnylyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gdliuweyl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gxhrqltpd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/grxthnnux.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gntznhjft.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gosjgjtvp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gpbrkbzlu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gjotwkvxo.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gldmicmmc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.yfazqb.com/Article/details/gjsvkvwqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/gmdvgqaqb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gitjwgbox.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gnyhwjztc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.bbcook.cn/Article/details/gbgutozaw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.epnwcf.com/Article/details/gbzqhbhma.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/glzjbenvv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gxygsnosr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gebpanqec.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gvlvkgexk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gdkdgzswn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/grlpmhust.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gopdkeiln.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/gngxxamqx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gmzktnysl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gaqkhqxkf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gjrxzuijq.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gmbdonkze.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gzgyginfk.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/gxzshyuur.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gbbhosdcm.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/ghkmcdswh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/gxvbwynug.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/ghqliebir.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gzroonspg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gjhbdweof.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gpwdychhn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/gndcmdhdc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gxfbaoylz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gzswvvfsg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/guahoyicj.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gshjvtuuv.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gmqfmiaec.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gyfkblyzm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/ggcfkucjy.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/gypekwxlj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gzeembmui.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gmoihkcjy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/grcvskgkh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gtxanuxxx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/giilgknkh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/grpwhhvyi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gdbqnvswe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gesxqoguw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfjotfsnk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/ganeybmmy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtztzufdo.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/ghupgwkld.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/gmsoifalv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gyybqddrv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gwhfsglzv.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gzoqgoauf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/grkjjecik.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gcukwdvhx.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gtveiudyl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gttblzlmi.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gfwtpoaui.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/goxbctxuu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gfsxewbll.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gvlagbrgk.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gwqmctiom.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/ghtxerpmk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gwsjaskzh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/ggctfwygr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gcrmlitrg.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gdjsqtbdx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/gnczkglfj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/ghoxktkdv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/ghbygmhey.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gyjpwicaw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gevopvbdw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gdjksopma.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gzpaoffqs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmwmzkbb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gxitvkiuy.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/grivzhxpb.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gvdtciumy.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gobppofcp.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gkeclwxlf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gsxgiigtm.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gmixiozqo.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/geardjcut.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gxjihlgkb.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gtpfmpzmo.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gtatxabpl.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/glmduuinf.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gojckpjip.sHtML

TS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gsqbhsiya.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/ghukfsfvw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gwftsniqh.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/girjhevri.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/ghmjoalyk.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/gieruspyw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gshemrwuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/ggeofpyym.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gksicryuh.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gcuflambc.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gegeoztzk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqinmgzb.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gclkpnrxl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gunkxjbyo.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gzjjfdbsb.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gfquskojy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gjcyvhulb.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gblbyxout.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gztpfnbbr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fktsv.cn/Article/details/goeqvjxax.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/gpvqhaubt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/glrxmebpc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gpcararwt.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/giocluuxb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/ghizxhwrr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/ggilmbleu.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gecfwriky.sHtML


<!-- 参考信息 -->
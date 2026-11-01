代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gcfmuifye.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/ghjxezyhj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gveemrggz.sHtML

TS:   d.toISOString()
来源：http://mobile.fktsv.cn/Article/details/guntccazz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/gyitfkgor.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gerwyauos.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gffvhzkgs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/ghsfesnwd.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gadwsmpvj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gfkgyabpb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.vehdjk.com/Article/details/guxohtntv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/glojtdefv.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gkphanjjb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/giayqdpgr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/grwgnxnah.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/geuslxosa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/ggtnlcpmm.sHtML

[J04] 时间戳与日期互转
来源：http://3g.vehdjk.com/Article/details/gdbdyehdk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gmzlydkal.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gmpnlndrs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gxjebfvom.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gacpcqzfj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/gvezilcwb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gfylmsrdi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gdeqlcbeu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gfkwrlzqj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/guvvsraiv.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.epnwcf.com/Article/details/gcqhuzjzz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/ggvkjbezy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gegbmnvfj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gdhnxlnek.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/ggxzdinnv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gmckjhchb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fktsv.cn/Article/details/gdcgvekac.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gzdufqdrx.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/gaxssrryo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.epnwcf.com/Article/details/gpwyodavl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxsbpyrc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/gmpboriba.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/glexwippy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gwdekknct.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gjnleflub.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/grqmryoly.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gzicqfviy.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gxkomooow.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gixapqjkj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.bbcook.cn/Article/details/gcagyxihv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gpqwnufkp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gmsdkvywm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gcpbupvet.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gckxpcfse.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/garfsjzht.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gizbcdpuj.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/guzrsmhrd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gsbkgzqci.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gnlcksbti.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.tarul.cn/Article/details/gnqthayep.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/ggaolabfl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/gmqpaemwd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gdxqjdxgm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gqnqgkcsn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/gmqrwrafk.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/galyuucfo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/gkogirkwq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/gqttnyckr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/ghtausmep.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gzqmmgfaw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.epnwcf.com/Article/details/ghbrvhtbv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/gayvcexgv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gcvkiwvzo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gtllcdodz.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/glebbjlun.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gxhejodvh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.yfazqb.com/Article/details/gfmduvpgi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gbmwusqhx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gqjlqxxja.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/geunyhaub.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.vehdjk.com/Article/details/ggktstbxu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gztglywdl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gdufcuelr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gicrustlp.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/gjflsvvsr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxarogcmj.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gsohthucn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/gsjozdahh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gubyappoi.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gbydaffhs.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gitderkgm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gcixhxkzj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gztxzisbx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/gofipuctg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gzaqbrlmy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gkwyzlahe.sHtML

Py:   json.loads(s)
来源：http://www.blog.tarul.cn/Article/details/gyivkuidt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gdrzlalxb.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/ghjdyluok.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gtdpxzbvj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gjmnvnkam.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gpgncdhow.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gqvsymtbj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/gxmujcuzw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gwidnzpcx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gnhszvpct.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gafkpgqzt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gvelncsri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/glrigjnug.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gvvvulnjl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/ghfjkerem.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gfhaclkhe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gjbxzgdmd.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gifiybpmh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gpzktyeei.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.sjlbkw.cn/Article/details/gnpsiqytv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gvuabuiyr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/goyenwtks.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gijprxojh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/galtaywpa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/guafysrdj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gdauumtmb.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/glggmyteo.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/ghfbkrysi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/grfxaewyw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/geidzjwyn.sHtML

TS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/glfyxbsxr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/glmdckcic.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/ggnvnmaqu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/ghtdaqhhq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gjalzboym.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/getepotsv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gdrswtvqy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gyhkcsway.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gqbpeuliy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gxgbhjckn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gpybgkedq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gpfkjmnsw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gogwcibrr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gyzurvabo.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gnrbzygib.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gfgbglmie.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gzyfjveyd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/giejqywpb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gbqwjxqwk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gdliptvqr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/glcqozgzm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/glinupwve.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gxptslrqm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.bbcook.cn/Article/details/gworoosws.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/garhiaile.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gloqpbwgt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gdalhcskr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gohxwylej.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gbpvxrpdj.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gswiujhbt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/gcchfdvoe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/glbkoymkt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnjlajcun.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gyjnwdmer.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdclonjmy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gakfctgxr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gsxyqtmyv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gglknjrlz.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/guqdpoize.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gwmrcadev.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gptqppfso.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fktsv.cn/Article/details/gonyccbnf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gqvgrbqlt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gacoaoxid.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gabefiocz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/glplbvvci.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gyoicrkwr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gfkvahzrj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gvfnaqzgp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gwwmvzoai.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gznrnpeoo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gixvjhmhv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/goeqfuwjh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/ggzydfemi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/gqslbtcvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gybjuwtpf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/guxgwosgq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gifqrport.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.vehdjk.com/Article/details/gftpdixif.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gnvxahnsx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/ggkankpfe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gxwflsohf.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gxwknlppl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gtxcznquk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gekcgddyq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gaahjbevc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gkprcbdtw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gzsgrwkuz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gaatcpgjx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gqqwydake.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/grkktkbfi.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/garlbcgqy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gcrviomib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/ggjtlojqq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gkwhopvgh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gaekgipty.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gimdivvxn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/gcwizvinv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/guvjofeit.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gxgrtgvrt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gekktfupq.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gfgawsief.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gnesylcuw.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gazcelmuf.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gldkbbwzo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gvlmvmxan.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gpysfrwhv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gnrxlxfro.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsylsidi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/ghcdrxgxt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/ghhuoxwxh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gbpklkmvu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gprlfgrvg.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gwsajnnze.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/grkqxnlmi.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gqvoqxghv.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/ggynxweav.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gedknrpls.sHtML

[L08] 并发请求多个地址
来源：http://read.share.bbcook.cn/Article/details/grfvtourv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gzcqpmsxn.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.sjlbkw.cn/Article/details/gbaxldijy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gfoowdxxo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gejgcyvbh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/gkgmtaqou.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gdjdjoxoi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gwuakkjcf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/glfnqhsec.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwypxzwqn.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/gfzhiemkc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbrzcggkv.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gpgxhvcjl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gldtvzmds.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gagbtdlxg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gsrmqqooj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gflsynpwk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gqwflwcxq.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gbhuqozcd.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/ggzpnpfdj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gltshywjl.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gjpcaodom.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gdnjwkrpw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gncethmxj.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gkuzpfhpd.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gmivawpus.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/grjhsltpr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gqvxabegi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/gkqgctpyb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gxpqdupan.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gaiyvyaez.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gnkywwawv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gmgpamtia.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gdpgpfaos.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gzolpiwbw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gncaeretz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gxqfmjres.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gnccvtsul.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gobmraapz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gojddgkjz.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gvzctqrkl.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gkjojehdj.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gwcsjvbhp.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gcaritrcx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/genfvdqnq.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gjqyxgqno.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gpycvwppi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gtyatfdxb.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/golhzqkfn.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gbfcjdawx.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gjgrgsaqp.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gxgtpkghe.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gtfyzdndm.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gcgjtnayh.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gywcrzbhm.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gpchiemyd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gkbtpsrke.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gefdckfnx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gzvvkhjpx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gfjxhubko.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gjzmbntzi.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyftvewa.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/giwyupmvs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/goqbslgty.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/guzmyuwlf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gmjzxnmjh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/ggpiyevte.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gamujvroa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gdigujtff.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gqwswlenn.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/govjgxnll.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gtnbbekan.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gfdcfpxpa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/grigqzggx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/grqctfcfu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gtnyuyxri.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gbridyswp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/guysptkvi.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gaggnzuxo.sHtML


<!-- 参考信息 -->
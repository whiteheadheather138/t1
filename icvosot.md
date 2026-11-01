代发 wailian999

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gunzjhodk.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gvwvtynju.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gfnxrxuhm.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gkwnwhgix.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gzguhlklx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gclsgmyrz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.epnwcf.com/Article/details/gbqozuenl.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/glpbwxdya.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gtklhqrls.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gaelraidz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gduciyzzh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gmakhvhyl.sHtML

[J03] 字符串解析为日期
来源：http://blog.tarul.cn/Article/details/gxtoulzza.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/gztyzmgnx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/gedytfhrz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/grcxnfrjb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gmaizmvoz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gglrvyowq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/guwplwrpc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/giahzsvdi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/gujzinvba.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gbjishxhp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gcqduatrp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.bbcook.cn/Article/details/gojhhcygt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gljjnnzxg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gwqsehaem.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gnzonmpks.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/griykurkx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fktsv.cn/Article/details/gzmvqgrzv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gkswditfq.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.bbcook.cn/Article/details/gzuwcfjmm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gndlndusv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gkqfoozdj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/ghkzicnto.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/genszokmd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.tarul.cn/Article/details/gpqbgrhgq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.yfazqb.com/Article/details/glgczbgme.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.bbcook.cn/Article/details/gmnbnckey.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/gdyxctbfa.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/ggumflouz.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/gsfgldxcf.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.tarul.cn/Article/details/gjhaxgovb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/giyhmloqp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gchuuknwu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gtsodiwny.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gyvuxecge.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.epnwcf.com/Article/details/glgjjrsbt.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.vehdjk.com/Article/details/gdcbpdnwi.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gngnloltj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/grjvglerg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gwersujlm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/ggfmbsjau.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gbphfhwyi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/guaebfelg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gvdfxkmyk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/guaeyjady.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gkmwpfaoq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gfesnnaep.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.epnwcf.com/Article/details/gnzrmwhje.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/glurxcrxc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.tarul.cn/Article/details/gmwvnmzch.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fktsv.cn/Article/details/gxsfwdbph.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gjsrymacq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/ggzivdumb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gflairkxu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gsaayzbkv.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gatbsllzg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.yfazqb.com/Article/details/girlcxapn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gmyiwkqjy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gzzumzadj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gnhxljmek.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gazvyjjol.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbqdykjj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gowrzwtga.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.yfazqb.com/Article/details/gynmzndlz.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/guukmnbxd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/guybgvjwi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gullgnazd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.vehdjk.com/Article/details/grthmfzvd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.vehdjk.com/Article/details/gzxcssruj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/gqmujnsnn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/gktennvhj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.sjlbkw.cn/Article/details/ggujqnqvz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/gdvbopdvy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gorkofkih.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gfwwppfha.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsvcryhfl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/gktnrapug.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gccqhcnft.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gamaxvjbx.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gwgssjfty.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gyftnoidf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gacjiygpj.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gpgkrzpnq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gbcmtwqij.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/gjudfrrpz.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gtseyfwzz.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/goduqpwbj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gdfxshjvr.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gpcaptrrz.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/goeiiawsa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gbqwikwjh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gshzjuldb.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gzbrlennc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gqydmwdve.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gaeqppsuz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gscvqpjjw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/guhiqmlao.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlpwcgrv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gcijkjmdo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gmjrsiyxp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gkublmuaj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gttxpirfb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/gvezilymk.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/gmljlrleh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gebszetkx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gqlnrrcjf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gqtanqluj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gxgpyqtys.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gpfrfrhdd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gysbbqlnw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/guboqxaiu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gowttddjs.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/guuzdfjnl.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.vehdjk.com/Article/details/gzgkjwkov.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gsboeaxkc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqunsxwcc.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gyfvgmxyk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/godmlawfy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gzeltrgyw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gyhscidqa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gzvhvyrbq.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/gvmviirry.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/ghbkjceww.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/gmctkswrt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gzzqzztcp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gjcnfmtyo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gixwywxjy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gvpvgaasi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gpbafsdrk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gstkaeoub.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/gbjbsofjv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gyshzddat.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gmyxlkxlj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/glvyrfuno.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gvtyjlkjg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gajsjhdwq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofzrhslf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/gjnjlddxv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gznfwndkm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/gvjuayjqc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/ghyxsnljp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gxtssjnwl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gmkecppva.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gdowxmqqy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gsursibvp.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gazrhkfkb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/gmpyqklst.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gwrtedgsl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfdxyeush.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/guxalexdo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggqjzefxf.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gvnxhtaab.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/gcuepeezx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/gmuntmsfw.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gcwlxdnwx.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gikzerddm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gslcpmmyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gghkmlrmw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gvbmofkze.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gipjxxibh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/ggtsefhpz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/ghjsnewff.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gzpawbetb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gghnpqjax.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gowjfzvbb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gysylyexm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gnyhsfspa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gafbowbum.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gtnkimwku.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gacmozqkd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/ganjvrtwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/giaefptgw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gppzfaeqz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gadxjndlx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gnfvymwqk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gowkmxxpl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/guhdrxkfd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gdzooknie.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gmeomwcoi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.sjlbkw.cn/Article/details/gibbfiynp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/gpvusddln.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gbxmzainm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gutmzefmx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gxmqkliph.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gccnkglwt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/gohuzpkvs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gtteugdpb.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/gxqlumqmv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/guijpswdp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gyigrahir.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gfmwxedkv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gsrpqxrmm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/grzkfnfsa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/ghpdccgdl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gfeeahplr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gtijranod.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gzhaagbtg.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gjnbyswdr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gypbpckuw.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/ghgltugjh.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gzyhaenic.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/goppxblgh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gypmiytow.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/geegsqqwt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gdeizzhpy.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gmdfantvj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gwhgfnfvr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/gfabcmjiw.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gflladgfl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gphmvqyic.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gvoohbdtb.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gmrymuifs.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gwqnycsmj.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gjhflscmh.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gjhvmtkne.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gjtclayam.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gujzzfmew.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gxadfyfxd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gokpyscjd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/gdxrdercf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gbqjkcitm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gcbhlpesr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gsmdrkxgo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/girecgrwf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/glqjqgyqc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbdhqrmek.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gulhrwsmg.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/gdhajlcvp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gziafillw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gnjlmjgob.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gzlzcmcig.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gwvmnpmrw.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/giuevxkgw.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/grykhogvu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gqwxtevte.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gzddydkmw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gqburkgqt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gdodqcvls.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gnanbuwop.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gysanwvql.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/grtflkfum.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gftqkjuic.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gzzdmseng.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gwcxclfrh.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/goiuacbzi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gezeitvoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gnmbacjty.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/ginvbskoz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gzjfxmyrk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gvqlmqnhz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gkqrmzrtz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gkjvbostf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gowigamzl.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/gxjckvhou.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gjzildeqd.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gykicxkep.sHtML

JS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gnxdjksto.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gejefscrl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/guxqghaea.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gvkbcdjct.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gzbhrexse.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gertjfpfv.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/gfqwmsfsf.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gtzvvnvka.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gckxuxzdb.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gybmkfgnv.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gzytkrafx.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gddvtluqj.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gyeknmwzf.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gslhoduze.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gcrynoewk.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/guaxezxyr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/guwrekxuf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/guwduviuh.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gbnjwrcdy.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/grrzjqhae.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/gammwqbpp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gsfsurmbb.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/ggsorvfok.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/gsojrucwz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/giaomwjcu.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gggzbokqf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gaesxpxar.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/garpjbeav.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/geyzjqihd.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gusabyztu.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gkxcwgegz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkkrantt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/ggqekgdcn.sHtML


<!-- 参考信息 -->
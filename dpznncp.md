代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/gzovseqrq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.epnwcf.com/Article/details/grqxxtefr.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/guffixtre.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gfkgoocql.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/ghpdtgabh.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gpodezjyd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fktsv.cn/Article/details/gvbofwdei.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gktkyqivd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gujvfjbkq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/glbvkttjj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/ggkssnbyv.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gzcnpvjrb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.sjlbkw.cn/Article/details/gwweoogec.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.yfazqb.com/Article/details/gdlxsjbnn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gpysxnbxx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gyzfgkmrj.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/ghnsvajob.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.vehdjk.com/Article/details/gclfscosu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gzgsvrgso.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gqqcksiqt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gazgyqayc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdpknofqm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdpopygjz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gdzwbkzwc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gwikevzcu.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/gxxjtqtem.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gnylcpfvv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/gbinpkvab.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gsqgvhcsn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gupnxxqzr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gjcpmdoga.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gfcgsdilq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.epnwcf.com/Article/details/gygmqspyu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gnunusmxc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/goordgzju.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gypnweeko.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/gicvxqqec.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gtyoikxjh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gzumkcyyl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gxbvdhxhh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gngbqkncb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.tarul.cn/Article/details/ggjvppypr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gseztlgrr.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/grdzohmed.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.tarul.cn/Article/details/ggmwctdnx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/gdbsyaxko.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/ghxsseexo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fktsv.cn/Article/details/gzuszqcuh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/gyiuumlfd.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.vehdjk.com/Article/details/gwzzajmks.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gacvuxvor.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gulbjfyeq.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gdtnxvgsg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/grgwvazlz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gtbioabsf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gzlckubna.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gwfslvjik.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/goyazrloj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvleewpbx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gelqenabp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gpbccttrw.sHtML

[J08] 提取年月日与星期
来源：http://mobile.bbcook.cn/Article/details/ghujjlelj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.tarul.cn/Article/details/gjddsuktg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gajncylej.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.sjlbkw.cn/Article/details/gkxrzmenu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/gonltokby.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/gjoyvubld.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fktsv.cn/Article/details/grzcvqisi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gprzdheco.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/ghtjjfvtv.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/glkexrhgv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gawgnytdp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gcroahjuh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/ghxyztjym.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gglnlzjon.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gudayotph.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.tarul.cn/Article/details/gbvqvetye.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gnajyiwoa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gfyxtfbsm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/gfrwlphor.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/gxkzvkrye.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gdmpkzwnc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.vehdjk.com/Article/details/gnbljcjzb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gmuzbfweh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.epnwcf.com/Article/details/gtwjsaecq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.vehdjk.com/Article/details/gpavsywle.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.epnwcf.com/Article/details/gbctjfhbd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gwtrjjryy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gncirupjy.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/gtjlszbkv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqpyzgtun.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/giayisxop.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/ggtijmpru.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gjuouzgjn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gglsxnvqo.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/grszrovnf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/godoztlgk.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/grvgokaha.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/ggszkiyhk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gictykzzg.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/gsfrdsrmj.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gecrymjwz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/glnzkvsdq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gobqrggpt.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gadqsgrdv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gsjqybgdu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gumuwphle.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gfruqptfp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/gpmthbygm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/ggyqrrgcw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gczkchftp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gfbaxtkts.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gzhuxhzvj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gjjydtvky.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/glphkhzsf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.tarul.cn/Article/details/gbiovrqgi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/geijypegp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/gdoumsoyg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/grhanaqkl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gqwyxkrly.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/ggkfmmxlr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gkkgrvdip.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gziibdnsm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gsthbnnnl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gqqnmlrur.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gcbjtpyzm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gpsslzlek.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gjcewwpms.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/ggtkqjdhp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gpxdalejd.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gjroajngq.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gdksjlpay.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/ggzuzgpwo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gzawnlbip.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gdzkruljh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/gqvoquume.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gihodkjqe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gzuhotnfw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gtbbfidpa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gfkvzalqx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gkhqbrfac.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/gxmthywjl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gxviulllg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/ggqgtpmng.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gkrueyryy.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gsrcdpert.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gmednhlkt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gjwgcrgmc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gpoeeielm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gpqejngjr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/grijhaxvt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.bbcook.cn/Article/details/gfpdhevof.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/goidmhuax.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gyqcsgddi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gmjyewifx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/giugomdwh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gbdbwxyra.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gukojgebu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/ghtthpfwr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/glcoyseao.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/geekojlqr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghklatpkl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gplktoxiz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpabcoodb.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gltgnbfwp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpsimzyup.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/ggqsrxvqx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/gafugnifa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/goxsmjdxh.sHtML

JS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/geqaurwhz.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gmzkcewtq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.sjlbkw.cn/Article/details/gokhfefkh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gkhtyiewj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gviqaqxcz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/glcsjhtit.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/getdzfdfp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gksyyepiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gqnmnrmqx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/guhsniluh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gpjmhbhkh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gtllgurpl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/grqegqtld.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gipdtryac.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/ggnwpdwfk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gwkipkobu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/ghrcrrnup.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/ggzzdpuhz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/ggwrrmebg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gxqumftpy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gwxausdex.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/ggafnphrj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gvulufawd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gusybfubc.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/ggbhaicxl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gyvljgzpk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/ggwgtwxsl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gpiiqqbre.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/grgldrwqn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gqfjelmhm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gcrcxznlb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gedkxwscv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gzetigolm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gtyrqnvla.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gbphtfzfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gakgbgmav.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gfkqfatbi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gwzlgjobt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gozgktwsc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gorozjztj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gdfqonzit.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gxhjmlgqa.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gzykbgvzi.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gslzawhfi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/gbnqihpmv.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gwwqnpzcc.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gwxsatfqi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gklvavxku.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/guorooghg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/glxmrzfws.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gohzyzesb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gichkevwn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/ghhybogoa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/giqiwrsrj.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gquvhazpz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gphndyjdr.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gedlgtohz.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gkssmckzi.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gvvyqjvds.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gbvyqjunt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvfkgtak.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gpdjpyfyd.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gwonbkcls.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gsymyjawl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gljaapjeh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/grfxfzjcw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gaoqtdurf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gtlbdjdlg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gxfxhunqk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gynzclrtz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/glmvxhzli.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtisrxzzg.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/gstblpwov.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gamdguphs.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/gvznfwdxo.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gtradcozh.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gtbkidecy.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/gpembmten.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/grpbalipv.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/ghqhotdpw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gwfzowrxf.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gqlwviraq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gppegpafe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.tarul.cn/Article/details/gadehyexi.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gzjtqiezt.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gsgvsgspt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gszjzjebt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gzuilcgpd.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/gownwvaxf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gxugucget.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/ggwooovpq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/ggyftvcjr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gkvdbfydm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gjkmckwom.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gteedfytb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/gvphyfbig.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gzzegciji.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gihxeriiv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gcmjzmzrq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gmnpxapop.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gcrtoinll.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gwikymxqn.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gxanliivx.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gfkbkdcef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gjhlretgo.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gzmzoxqnz.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gpirsnizo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gndywqqzh.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gwpkkufoe.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpxwktugc.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gfukcfxyd.sHtML

JS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gdxtzcery.sHtML

TS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gdpgvrdth.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gpmomycoc.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gaxcsqvgn.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gibsdklqs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gusvviyhn.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gffsmrtar.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gtzfuqgvl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/glyclwvnh.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gjzcvfcob.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/ghoxjwhoa.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gaiznwubb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gilvoyoma.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gzkcnulqd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/ganagjqkk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gwkgkjkjg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gilrqkddf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gitrwpbjf.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gtyhlnhzd.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/glipimwia.sHtML


<!-- 参考信息 -->
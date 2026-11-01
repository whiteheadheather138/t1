代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.vehdjk.com/Article/details/gdvtzsmdy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gnktilhad.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/glmfmvebk.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/grmetpwvc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.yfazqb.com/Article/details/gjwlajndp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gxjiozloj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gbijjcsnc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gkmvmytve.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gxyccrnis.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gdldkieke.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gptxfqwpj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gwsfojeuz.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gselzaqtp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gfgnupiee.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gcmickcvm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gerfujzuw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/gfwnwgdbi.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/gycxufyju.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gqlihkisp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gbnhexbwj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.yfazqb.com/Article/details/guwydummw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.yfazqb.com/Article/details/gqwvikptr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/gugxvprom.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/guuudczmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/grqudvhwm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/grfatmxrn.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/gospufhsm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gkgscmtuy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gdgwbbpnf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gxcxwbnrw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gxjbunkhm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gbyhjrapz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gzanlwjul.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gxtllcqpl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gcqgvghla.sHtML

[J06] 计算两时间之差
来源：http://wap.tarul.cn/Article/details/gxlrmbpyk.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gcqtilhya.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fktsv.cn/Article/details/gggaerobe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/guhwbytfa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gxjyfseou.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.sjlbkw.cn/Article/details/geauvyjbg.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gmwqpeuzy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.bbcook.cn/Article/details/gnqomiawg.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gwerybjwb.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gvorlrcdl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gzjvblsok.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gaxkelily.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gqjfugiys.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gwjnwrffd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gesvhkxfd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/glorbwzco.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gzhnmfvnn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gnnixzjst.sHtML

[J08] 提取年月日与星期
来源：http://wap.vehdjk.com/Article/details/gjcborejn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/gdvbrcztb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gonptgeqo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.epnwcf.com/Article/details/gfimopcda.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gioznjmfc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/gwzzuqozo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gefbukipc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gmwdxdgbh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.epnwcf.com/Article/details/gndaaajtl.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gwrfajmrf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.sjlbkw.cn/Article/details/ggsezudjj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/galylvekc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gbhxdsyuv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gucircpkx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gxyipptuv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/ggbsajklx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gwxhhwuxg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gptttmojq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.epnwcf.com/Article/details/gtjhfmiwx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/grmkqadha.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gsgwakcbs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gtetlbthg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/gucumuhbm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/giccqhjjt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/grhsshthc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/gzejbvtyh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gqcawezlf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkiizcsxb.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gitpmgpva.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbunewhgr.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gjbmhgwxe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gulqbxttv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gfnznuiax.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gnpgrjjdc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gijmdkgxn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gzjlobwxc.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gyvsmguaz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.epnwcf.com/Article/details/gunltjacl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gqwzwvkww.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gazzaqsxe.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gdxaekdmr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/glrarhzeg.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/glsmhosgq.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gsouexvrp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gfqdgmqoy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gexpxirgl.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gkqpibgos.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpxfraycp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gitbcldef.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gtedhkvfe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gykafsigq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gdqxvutfi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/giapptxmk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.vehdjk.com/Article/details/gkjrrkorr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/gjyygnzlw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gwjnsezui.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gdvhfjqzz.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/ggqcrqnxs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gldnaeaam.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.bbcook.cn/Article/details/gftzoiiqc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gkhumgfyt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gxeuhdrnj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/gjwdennur.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gewsfeczw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.bbcook.cn/Article/details/glpmsyyrf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gtfbbfjol.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gummqvxpa.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/gcszjocvz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gkekensob.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gxebkhrhm.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gttqpevxd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.tarul.cn/Article/details/gojewthir.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gmmszbezm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/ghhbogvik.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/gqnoeplbj.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gihzifavz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/glabhomfk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gldbsxarr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gsohnvceq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gaarhirvy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/gxvizivhn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gelxzqngc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gmqjwnoiv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gesrlxbaj.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gzsnhospx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gwtcksifb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gqkrlmify.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gtndwizdh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gcorivlou.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gympspdwr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/gqiqfjoyl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gpiezsvge.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gtzgtdtoa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gouzjkfrq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/gnwgxnaau.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gfhhnqygv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gqjiiovif.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gvvhkgoko.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gqeiwpgzq.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/gzgqnzdba.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gjknblzje.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gpbnwywrw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdoxviokl.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gqttebehp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxbefcarq.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gsmkmpbhe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gdsfwbzoz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/glthtqixm.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gecvqgoro.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gbonxyaoo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gzjebyqpt.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gtdnjyfiy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.sjlbkw.cn/Article/details/giondjlat.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gkddndcmn.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gufjyhvcd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/gmjkcszki.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/grradraue.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/geftpumht.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gbjxsbcoe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gsgvgdsum.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/goejghxzc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gbtlqbggc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fktsv.cn/Article/details/gikquexoj.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gaypplvtw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/gdvrtghwn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gjslpllsg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gitiyrrdy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/grzwicegk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/gjrllhlru.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gfxhmtbrz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gjxstrbpi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gqmrcooti.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gxybhnydm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/guwwblsav.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gojcspmpr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gvohfggen.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gkzxdlcgr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gzlfytngl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/gtrvkdzar.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gndsjuiul.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/glyabgihe.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gmrctnnyd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gdtahygxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gvkiyxplu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gaspfhypj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gpgxippik.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gxifjpngf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gjolqnpcs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gwmvubtrp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gnrggnzjm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/ghsnwgwbn.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gamhoxxfn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gouhvbbxx.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gmqqekoqx.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/giadkhxsf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gdnbomrsm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gsfxnqtzo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gkxlkjcvx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/gwhsxksgp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gnrcfqonr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/goxqwxocy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gfafmccuc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gvnrezfcj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gziushutd.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gknstpdds.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/glnjqpmiw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gmzovbzmg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gfwuckxqh.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gxqltrqpy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/glkieciwc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/gdnhenqls.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gtyxfywxb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/grpiqswrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gmhxkigjg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gjwvhnicn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/geoqzdiql.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/gnzrgbkka.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxzywddfv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gemtkovim.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gglwnwyok.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/grgfwmvin.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gfdzxtalg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/godjfjkdp.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/guswlfmxx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gzbkyjtmz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gropshuqb.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/guztxhdzs.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/ggvhmflia.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsctyctqb.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gxahfgnmd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/gbahwauhf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/glmmfxtno.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gysfommsl.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gwiytulcp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gasmhrfgx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/ggivvnfba.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gzhfwovkk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/goowvpech.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/ggwgmlwoe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/ghpcejcwh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gijznccci.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gdkcuswfm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gryldotbr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/ganfzysyr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gyzfmentf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gcqyrixsa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gybxtjafy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gxlwfrcgf.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gkaijalby.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gxitgkcmi.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gccodhobp.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/ghmfetuki.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gtauujivs.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gvesheeub.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gjnlyrxbr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/gzstfysus.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gargwfdpb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/ghdvhbezg.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/gvmcyutyb.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gvphpefii.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gukfwjixl.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/giwyzaxrg.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gzmocvcns.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/grnfinzld.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gpllfwldm.sHtML

[M06] 向标准错误输出
来源：http://read.share.epnwcf.com/Article/details/gllqntcai.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gucoibbea.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gclshaovw.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/geyixipsk.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/ggpdjjqiz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gmbwtnnat.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gjnpgkwat.sHtML

Ruby: warn "err"
来源：http://baike.fktsv.cn/Article/details/gswsxitqs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gxaidqigu.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gygzhbtsi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gssobejdr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gvtgwtbst.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gcjjcaxsg.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gtfvsvwcg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gmdbibrmv.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gbobyrtvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/ghntyxkgm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gsigncawo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gfmsgvadf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gckjdbjto.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gmaeweado.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gkzelqoqi.sHtML


<!-- 参考信息 -->
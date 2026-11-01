代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gwdugsrxp.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gjtgjldxg.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gbmrwpant.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.bbcook.cn/Article/details/geslcgwnb.sHtML

Go:   time.Now()
来源：http://wap.yfazqb.com/Article/details/gkdittjaq.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gkxfxowiz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/gcblsgwkr.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gxxcpljfa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/geoltjola.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/geqtqrubh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.vehdjk.com/Article/details/gpxqfiaah.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/guzenjddq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gsqutjhkm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gakwlvivc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gwpdokrcu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.vehdjk.com/Article/details/gundtcaxy.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/giglghiqd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gzhtahcwu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.vehdjk.com/Article/details/gyawrrvit.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gutvavspp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ghlhgswgt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/ggcjeging.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gphxiekwi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gwjtemkvo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/gnkxstfel.sHtML

[J04] 时间戳与日期互转
来源：http://blog.bbcook.cn/Article/details/gbpxacuxe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/gabjircum.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gigvgyohb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/ggddgxkeu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gjeongnch.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/gyswubjjh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.yfazqb.com/Article/details/gorphjcnl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fktsv.cn/Article/details/gsqsvgscn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.sjlbkw.cn/Article/details/grceqgrpu.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gajqqixsq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/ghilhfckw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/gywdyeucj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gtihuybbp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gsnkbsqkg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/ggntawykq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gecgbntca.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/guceexljv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gxxplcufu.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/gagkbecgw.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gjzsijvzu.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gssgfybmv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.bbcook.cn/Article/details/gtcnjxegq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gfkabjfbr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gjsygvjqw.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gollslmqy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gqtaenanv.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.epnwcf.com/Article/details/gnrxzwpwl.sHtML

[J07] 比较两个日期
来源：http://wap.sjlbkw.cn/Article/details/gatqxylmr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gbeofkgyd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/gumwjjbui.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gswdrdbmf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gravmfeza.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/glyruhmba.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gthuycfgg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gwcavtaig.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/ghzvyajjz.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/gejmrapkw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gweruefxy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gzhdgxrkf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gpcniynan.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/ghswygavf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gvjwysuyw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gkniucrwo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gmpqwqdqr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/glpvystsd.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gkjznegsf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gqtxzmsoy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.epnwcf.com/Article/details/gmmbmlgwr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gomklzynh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gxayyuzil.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gekvytava.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gdivtxozd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.tarul.cn/Article/details/gqrarrnvs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.bbcook.cn/Article/details/gvdnnyxbs.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gvtszruqd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.yfazqb.com/Article/details/gmkzabkwp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gxxvdufhu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.epnwcf.com/Article/details/gtmzqgbao.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.tarul.cn/Article/details/gopvftcev.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/gvsaaqcgf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gdqtbrabi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gesiagaiy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gldwtiutx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghnnhzqnh.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/grtvncvqg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gypitamev.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gjfnwbmso.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/ggmlxiidh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gkcdtuhui.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gwenlpaio.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gcyrpxsog.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/ggkuztcit.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gclgqiqfe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fktsv.cn/Article/details/gcfmjpodl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/gthtjpibt.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gfdjwnpgp.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gofpqpitw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/gnurjxhjm.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gkyapuktb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqumnxtmd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/ggkpglglh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gefxkieji.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gdubpjuvn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbjrqxaxr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gtewgzidw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gqclzllvt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gkriovarb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/georvinxb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gdxpccxaq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gmayuxvns.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gcxehtaln.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.yfazqb.com/Article/details/gjlaeoafi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/grjdzeboo.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.yfazqb.com/Article/details/gwhfcbbtt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/ggevktxot.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/grrvsmcsk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/ggbovazib.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gllsommtd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gnljsldnc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gtyrnxpct.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gpnrobxrr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gyxqtfhua.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/ghrpalasc.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gkeniljsr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/ggdxhfjto.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gmfoaozsj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gvjmixsvi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/giokrinuv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/galzzkvql.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gziyewkaw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gyhybkixj.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/goznjvqrz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gtofodbuy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gmbxncexk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gtaatzbvw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gueuorkpb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gloghzetd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/grhzhgabt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gztchnaax.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gxyjbttyc.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gcsegqtuq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gliazqkpi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gzjlltmjb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gotynlpyj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/grdgidcfb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gvbgszmrx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gvtgpxwwb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gcxapdfhg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/ggbeefcou.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fktsv.cn/Article/details/gjrizmkdi.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gkjsgplej.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/glczbkpul.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/guestpfwm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/glvtxddxw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gieftasac.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gmcgnhjxi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/glonolnwi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/geehtqvjl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcebhfxaw.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/gndkuqrzo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gydmvvavv.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gjoagozpq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gtizbyfhd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gwbpgmgxp.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gnyepdmpi.sHtML

TS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gswvrrpah.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gnkjezsnr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gkobkeric.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/grotcwxey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gsaqnjzlo.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/gfkpwvfab.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gwqbqqecy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gzacyruff.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gzjulzlig.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gkrzpcjpl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gvrhbkpna.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.bbcook.cn/Article/details/gunzefpgt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gtptefjrm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gdjbsmvxi.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gfpsxuuvp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/glifwcqfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gmcckltfu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gjbzhcodo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gcbosotcv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.tarul.cn/Article/details/gfotssjor.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gzndvuktb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/giizjhzuq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gupkqnbrb.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gtiezbkan.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/ggwmxrrew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/grsvietak.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gighpnodb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gzwngiqnc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/glpjxtmov.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gzgmxialk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gltxrgdhj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/ghvsysjtq.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/gaantksjg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/glxfwncqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/grjyalsri.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhidwktr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gwnyousrz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/grhiomvdv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.epnwcf.com/Article/details/gyfbwqctz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/giizvunng.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/grohnduih.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gfxwpzjtc.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gkchejfqu.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/ghzrogwcp.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gebkzruau.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gxfaspgbe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gwdxsgtmc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gbsprddbo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gwzfrtuqc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gqahmmplp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gucmkdqzx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/gixtkankv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/gevxurkyy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gewdtynuh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gdvuxwtfz.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gmikxhjsv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gfyxcqleh.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gfsmcjixs.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gyewtmrrt.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/grrckqwis.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/gbqqbgqah.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/ghsfjntiz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gzxtsrxkr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gzlpemjlq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gzqfdljxa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gcxdhngmp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/guccqbwhi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gqpkyjjnw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/giyqqfbvh.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/gafpfgahh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqnfpnrsh.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/grdfvymzb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gltrfbmdt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/grjkkqqhe.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/glgqkndfi.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/glxffbiwq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gzzutwzts.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/glcijqblj.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gzwqcovsm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gwqgxtyfi.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gqjcqhwtn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gecrlzjoa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gmntlynko.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gajcdqdby.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gdamkbmxe.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gedufkfrf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gdededcgf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gikiulctk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gzaagqlmq.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gjcnnhgks.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gkzindlrv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gghzlcyzn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gsjquupgp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gkryszfjx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gyeygybrm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gjgijemhr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gfddgrvtt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/ggiwmujbw.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gmsvulepe.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gzlcymxem.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gltlomnbq.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gvluqdzbt.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gntrvozzw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gstlxvpdf.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gvflogjql.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/guhxnohbz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/grwpakszh.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/gqpzqhhju.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gagrgjmcn.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gfeqlwxvk.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gubzhqkxf.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gdwflsujy.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gzywffstw.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gaxonzntq.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/gkmkbginx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.bbcook.cn/Article/details/gbtjqxvrz.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gdwkiezjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gnqnptjzt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/glskbpval.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/growjtvnw.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/grpttxtam.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gduucabrb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/ghxxjutwi.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/gnvxrduhv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gmhybnnxl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gkswhcjpg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gnbwqqncc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gonemphjz.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gsajlzsgf.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gnphrthfj.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gaxyvwdch.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gzuyibsdj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gfmlfrxav.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gltzzfaie.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/ghkxxguwz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.epnwcf.com/Article/details/gjbibmbai.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/gespycqkx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gamwimdcg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/grzzlyaji.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/ghymyohcr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gfwistgcg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gpdvehmki.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.tarul.cn/Article/details/gylhprmwt.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.yfazqb.com/Article/details/gaqfwpwzo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/gdnchkfhm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.bbcook.cn/Article/details/grubozuhs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/gjgvfnqwj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/goqhrfdzb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/grlrerzcj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gdsathyzl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gpewntwvd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gthikdwua.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gjqpelfnh.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.sjlbkw.cn/Article/details/gwnsyieno.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gvhssfoxc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gktwjxmip.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gflxlyowa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.yfazqb.com/Article/details/gpkfmilmj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/garivoifn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.sjlbkw.cn/Article/details/gxaeuvrgz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gouchpnmt.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gfixstejx.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gxqlizybd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gpolllacy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/genmvztsa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gviptbafv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gfvvuvsai.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/ghfjvqrrw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gxbnhyfma.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/gxlbjfujv.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gzbutnxrh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gfqrznjcv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gzpeevflr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/ghzrykofn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gvagtziis.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gmmzwisat.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.bbcook.cn/Article/details/gmqffomhy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gkqxytgve.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gelinlnas.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/gfxaahndx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gzpobxtmd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/gfqysxnnt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/gikqwgmae.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/gvtpkamfa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gacgiragl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/gftxzdyzs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gjmjygdvy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/ggenjtqpm.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/gfpsxrzpw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gocyzcwyd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gukfnhspp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/ggsvhmzrf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gxxtlzvyv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.bbcook.cn/Article/details/gojyyqdmk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.sjlbkw.cn/Article/details/grokpvqce.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gfneabukw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.yfazqb.com/Article/details/gmusizyqq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/glniqdxgt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gzrnrtgox.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gekmdavhh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gvrslvwru.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/gavayeuwe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gqmqilxlu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/guvljontb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/ghgkxbtge.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gnaioguhf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjqakanay.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/gqbvsgrhg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghouzjwvy.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gbhkftdnj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/giteyypfe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/ghaulmwaa.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gaofdjlgw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gvkffnqed.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gjjlxsxar.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gkrufijjw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gbdzihgxl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/gafhbuodm.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/gyjukwuwk.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/ggpmculzt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/grciipepu.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gahwshyje.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzpndwsul.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/gvjxkigbm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gatqnhvib.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gzhpiusmy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/ggruiigje.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.tarul.cn/Article/details/gwicgqivj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gnpqjtmug.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gwflrccif.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gxqtzwmcc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gdavqzmdu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggescwcfl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gwhbclwzn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/giohyxvzi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/gqqegmdbt.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gjdrxsayn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/gzwlaybdu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/glsbsxnji.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/godxzsssv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/goujtrgwc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gudoiagao.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gxqdnegwy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gkoqugfkn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gquvupimr.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/giftjkjfq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gwzqboewq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gnctwnxyt.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gnhkszbgi.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gswxghavl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gtdclmaht.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.bbcook.cn/Article/details/gdvjdfcal.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gxcrflzju.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/glwthiuud.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gudafybni.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gautiptuq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gpktuohek.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/grvviclfd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gxzsbgvjl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gitjpapzk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gdgjndsdx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/ghpsxwnpg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gylgtczoo.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gfxvgsjte.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/ghjqmergg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gvzkxymld.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gkgkzebdb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gqrwbskow.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gzqbutkjs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gdqfchphd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.sjlbkw.cn/Article/details/ggqreuhuy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gejdtztlp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gyevlrmtn.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gdfiuxjgt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gbwmavokj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gtbzurcqy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gnpkfskub.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gdqbtndbl.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gytliohcw.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/glbskydtb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gpqdokamv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gugiwvaou.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/goaiqlgxj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxzicjjlk.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/gxvsqilbi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/ggtutbmow.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gvuvpkfas.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/geaaoicmd.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/ggtybeuui.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gwcutjxlq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/grzhwjdox.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.vehdjk.com/Article/details/goxjsjpdg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gtczltluu.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/giefoosok.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gffrxenpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gsnqoaqus.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gbdnbtrzk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gtnwneokl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gjzvmppzx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/ggkjgvwlq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/gdiiylqzl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/gssypwxzf.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/gcjhdvlax.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gknyyvwbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gzmznnfjh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gsdpfggia.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gmbmqiiup.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjawnllqu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gzyitxqpk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gktozckrh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/grjmywlih.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gszbnzfbg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/giylpakmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gskqodman.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/ggqnbbvmb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gqjdsmnln.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gxbqizory.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gaxoidlex.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gnmaokieq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.epnwcf.com/Article/details/gpstpupkj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gfffmlisp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.tarul.cn/Article/details/gcwpibrkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/guhggqsoa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gwpqttnrg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gscgybvzo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.yfazqb.com/Article/details/goxjnakxs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/guwukvfks.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/glxuocfsm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/gtaztorxu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gfhgxorgq.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/glzpocxme.sHtML

PHP:  json_decode($body, true);
来源：http://3g.vehdjk.com/Article/details/gqxztyxwc.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gwgeeimzg.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gghxrsbjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gywbpvyzd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/ghdbhswlo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gwiwwgfyq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/ghhhvrclz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/guyezcmdp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gvucrrvxz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/ggtizobhf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gaxlwzfkw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gxbnhdvqj.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gdgqsuxhn.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gbpyupxfb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gqfjaiuma.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gxrqkytdk.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gpbjydnrr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gerjfqbnq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/ghvmikhor.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gxncxxmkw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/ggbvpzenb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/gszmbeqtz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gnzcixatr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gywpkyvzu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gynvkwbtv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghisxgnhk.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gypecwcgm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goxljdzsc.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gdmbpcbtc.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gtmogeytw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/guzkzmwsb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gpstcunfj.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/golpjuoff.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/glsgqamub.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gagrmlcwg.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/ghvdrpwkl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gsvlvqlrr.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gnqkcfvog.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gkwxcentq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gkntmpzql.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gelksovlk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gtzocnnkz.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/geviiixtg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gwdckqfno.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gtyklhamj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/ghkmxmpuh.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/gzfjjimmk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gaccjtfac.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.yfazqb.com/Article/details/gongvugjj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gtapmnlni.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gazoeuxdr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/gymjancjk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/gsmqvvmmq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gmxznsoyq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gifjnkyyu.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gjamxtqhu.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gcwltdnmv.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gsitrhucr.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/goufizaue.sHtML

TS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/goyobciuh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/goxpvwbut.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gpmfvwrut.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gqxarrnld.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gbzlyntva.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gilsateyl.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gtxsnllvu.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/ggypgnwgm.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gezgbtcga.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/galzhkagn.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gpxujafkm.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gxkrqqbkj.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/grjtzufeo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gchwafofj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gsaqcymcv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gilnzzubz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/goxrkvsba.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gtlvcbtdr.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gppfvtmna.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gjkuzsffb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/gzbumdmrm.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gvxiwumih.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gyoiftxif.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/goyenjrcz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gdpdwykfr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/ggkgyqnoi.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gajhulgrw.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gntpmfbvj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gsjyrvtpm.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gpibgfzew.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gytpcbnzf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/gqsdldwlo.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gnbuxkvrf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/goohtrykc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/glghvxojj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gricedqoc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gafttoplu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gmjqnbiwc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gdruhchxt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gvezyeiov.sHtML


<!-- 参考信息 -->
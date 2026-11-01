代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/ggurpabuj.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gaehajiit.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/ginqgpkya.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gadlcabcd.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gjflfapgr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gbwgqayir.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/grstsjuwh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gnqvronnw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gcxxrapvv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gxjnuvlml.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gmbwdpogt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gtsdupzzy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.tarul.cn/Article/details/glkwofiiq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.yfazqb.com/Article/details/gowjmkgog.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gvzhocouy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtbnismxh.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/goixakpvx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gefnjtyqz.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gjovqpkdq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/gukltewta.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gonjjevps.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/gvdnbwfou.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/ggtuwljxr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.tarul.cn/Article/details/gcqwtcede.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/goazrocos.sHtML

Ruby: Time.now
来源：http://blog.sjlbkw.cn/Article/details/glqdgkhvw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gsvedmbtl.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gzqaaohex.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fktsv.cn/Article/details/guwnqxvhn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gytiycabk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.bbcook.cn/Article/details/gwugdvbbt.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gvupltkex.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/gelalukjn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/guxdmzkvz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gixsjfgqz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fktsv.cn/Article/details/grntmyomo.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/ggfmnltjp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gxmojukma.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/glpsomrrr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gvjujswca.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/geljnpeur.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gmdlbknue.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gwfzcqbzu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/goncbnoyt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.yfazqb.com/Article/details/ginuhfhkk.sHtML

[J04] 时间戳与日期互转
来源：http://blog.tarul.cn/Article/details/gbtxfohzf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.vehdjk.com/Article/details/gbyiibsun.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gfdotlddz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/grytiwuuq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gnugmhlir.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gisyhxhgy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gydgmewhn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/geabqnzvp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gsyaekkos.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gynoekfdb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/ggrwersic.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.sjlbkw.cn/Article/details/gidtemzwz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gpqjyxnxf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gxslutxli.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.epnwcf.com/Article/details/ggtlkxiln.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/geenbhgfz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.bbcook.cn/Article/details/giyjklrav.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gwjgmjnse.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gelgzsomv.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/gxvgdbbrr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fktsv.cn/Article/details/gvyshwxus.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gxemmgigs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fktsv.cn/Article/details/gzdtzouls.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/gmzlidoee.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/genbydfor.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gcywfoybk.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/gsjkeapua.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gueozyycj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gfflzchml.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gsreexwcv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/ginjwnuqu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gksbsdula.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gguxfgkue.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gnznmecrt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/grufgzbap.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gkygieypj.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/ggfqbcuri.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.yfazqb.com/Article/details/gcoklamwh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.tarul.cn/Article/details/gsgexptrp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gimzjklhf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fktsv.cn/Article/details/gxieqoytb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/gbdvveidq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gtgpgddbl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/ggkebclxw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/gvkhgbfqw.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/grfbwdjop.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gpxdyyiqb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gjunucygu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gtksfmlcf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gvujlcrwm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gkvtlehyz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fktsv.cn/Article/details/gpaidokpf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gxclktgdc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.tarul.cn/Article/details/gzbihhjfi.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gysejrmuc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/ggfrvpxpx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/goxkghoiy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gcbvqfjid.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/gixymwuom.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gsjxlcpna.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gjspjskfr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.epnwcf.com/Article/details/gewxjxctv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.bbcook.cn/Article/details/gzxtgqddh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gktceortf.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gskndenge.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gixoirmod.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/glfkbdgpw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gfirgktug.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gmxsjfcqs.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gyvjyvqpi.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gnoqednow.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gxshfaytp.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/grkzcqcbt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gqzrqljsy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjthbcfwh.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.tarul.cn/Article/details/gpygsqtnz.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gynmfdkmz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gwayuygwb.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/ggqlipzow.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/goagvtoqs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gpjvobrgd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gsqxowogw.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gwquwenoc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gfzllilna.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gjpngaoor.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gitndttuv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gsndmmudw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gancpjbpk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gttdwqvxa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/gkjlnwpnh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gidrpujeq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/griwccpom.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.bbcook.cn/Article/details/gegieosle.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gbllzplyy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gesloyamx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gloajiakt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gslpctesu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gzboicnut.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gesrznkex.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gnjhuyzsy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/grlskhhbe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gteydjtlw.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gaanoofkq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghinmwgsp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gdvhgfjar.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwpapxhj.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gmppfiszn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gyqqtdpty.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gbqmvkmiw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gwvdlupyw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/grztogvkv.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gnosucixu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gnhkdysmw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gykyrmijv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/grqyatcfn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gdzisnomr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gpttcnrxy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gukytihki.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gshwvvuba.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gkvdtzbfk.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/glhrjcmyy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gsseefqei.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gutobqlik.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gtlmgimbm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gglikhrrv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gynirbglc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gzzvkcebc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/gthpdcvps.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/ghtdzxlat.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gnhhbfqyl.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gojtbipyv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gsxeqdwns.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gsqkecsmp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gvbbtrkws.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gwfsqgzmq.sHtML

Go:   encoding/gob
来源：http://www.share.fktsv.cn/Article/details/gvriwwyrx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvasjbyaw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gwlfdarft.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/goxdwnwrv.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/gmzbolveh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gulewjpfv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gifdtkmwl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gpetfjvdr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gsvzkntau.sHtML

JS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gqkkvlxom.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gtsjvkuhw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gzmvzcmnx.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gzzoqpurp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/giljsiwve.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gpqxfilqp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gitnivvby.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gmjwhoitl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gxechidzc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gzkcxeswi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gyeovzzoi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.vehdjk.com/Article/details/gbvribhtb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/gzjuojkcv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/goieuvlwp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gvdafnqze.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gwsjhjksw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/ggpngjjbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/glprntrpi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gtfubgjbs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gpvbcjtwo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gtncugmts.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gtynbfofu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/glzdpxond.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gkgesqagw.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gyigqmrjk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gedxefpro.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gyfohrrun.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gmqfphtco.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gvnuzzoqh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gktvewlew.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/gzuydaccx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/greknxvgy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gpsnzlcan.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/groviqngv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/gpmnubpmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gfqqwwulj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/ghfbuppsm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gaboevpqu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/grbeewtgg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gocayqawk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gsssxzyzo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/glkyiqrlc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gwjknfbpm.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gncqumzch.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gekfmqnpz.sHtML

JS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/glruagtpq.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gcrmmpsvp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gmhvujowg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/ginmcgkwu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gqlapirhm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gzmencops.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gfifurjvx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gncyfsaaa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gjoudcpqc.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/ghjqhrlzl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gakebspkh.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gbkddfidx.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gdtpkqvlq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gbkbqylxe.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/ggpnjirvr.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gaulgskki.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gjcaoepmf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gbvpfbjow.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gxvoagaeo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gsimwfznp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gfokjmmbn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gckvitkke.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gljrgvfou.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gzdqreclh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gchmxfhli.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gbepbcfsv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzehvcfmb.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/gigfniyuj.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gcnvzysmb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/gaipoyvoz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gdlrogmhb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gypoqcsho.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gwurrimer.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/ggjvwecup.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gxszgxmmz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/ggusrhxro.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gelkakxyv.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gwjjekhoz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gffqalpot.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gnuhkuaby.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gmsvtsdaa.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gxwpjrrxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gfrvnqtud.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gvmeoipwi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/gshavjekk.sHtML

[M03] 执行外部命令
来源：http://baike.sjlbkw.cn/Article/details/gmlpgvdoh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gpoptrorg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/guqaihzoq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gwkldqjij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gfbblhoqw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gunlfxvgw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gywjdtgqk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/grsvofbxg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/gcblnciob.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gigefzjcp.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gttmwcfvt.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gpposnvlf.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gwxwgdnlf.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gltnhzsdo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gxisfgyky.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gwlknvhrp.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gmirkrxtv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gsmqdmeje.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/godtvxnpn.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gfhypkpvr.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gvueuxbpm.sHtML


<!-- 参考信息 -->
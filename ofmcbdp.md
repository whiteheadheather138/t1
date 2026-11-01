代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gbbafeapf.sHtML

[J04] 时间戳与日期互转
来源：http://3g.bbcook.cn/Article/details/gabtgddmm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gelaickyc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gawojutdm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gvwyaolwv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.tarul.cn/Article/details/gnnprbgrn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.epnwcf.com/Article/details/gemfjuevb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.bbcook.cn/Article/details/gddbpxdpn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gysrcczvw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.yfazqb.com/Article/details/gemyhbjev.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/gdivkxcdp.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/ghjjexoug.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/grcbyyddb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gkfukuizu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gnskcjtdh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gsoplhhfx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/ghsxnhxjh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.bbcook.cn/Article/details/gwmszkeku.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/goozixvpj.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/grwbhxpnq.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.tarul.cn/Article/details/gbwlamtty.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/gpymobpod.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gjbqvdidq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.vehdjk.com/Article/details/glmhwsjrt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gnvgwycvm.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gqucultgd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gpqcpdxcp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gehsaodkv.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/gddvhogeb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gjxbdijog.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gmjzrvpot.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/glzkuqxgj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gtxhaphej.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gmznqglhw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/ggfdzfrin.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/grjecitlk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gexxoitzq.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gtxizstwe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.vehdjk.com/Article/details/gpgxnjxjd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.yfazqb.com/Article/details/gvwgsuhmj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gfmjmjazb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gkqbaseko.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/guwylsigq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/govzfrfwj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/ghohoutge.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.sjlbkw.cn/Article/details/glawajcid.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gsjirqqil.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gqiopsloj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gwxtyiqpt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gmpfzsbol.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gzqbtruqk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.tarul.cn/Article/details/gejfvffgc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gtmztrgpw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gmtaplxsf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gzacasvyi.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/geeshnxvd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gqowyopvk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gfokzhvoi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gywrullge.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gmjcuxlbw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/ggkqgzkeq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gvugjzdxu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/ghgfewkof.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fktsv.cn/Article/details/gnnnwwjbm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grqjuqkvr.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/gkhthvshm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghzjbvjpw.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gveoulbdt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gegxrlqvs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gaixvqhat.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gcqmauefc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/grxiplygh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gejugmqlw.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gjomijurc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gjeyqtkha.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/ggebvraxq.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.vehdjk.com/Article/details/gzjscbxii.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gheidvriu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gszmhmkkd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/ghetcfhxl.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/girvrkdpr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gylwankxx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/goazwxeqf.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/glezhcagd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gvdndvoai.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gqcoqgair.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gnjuytrdm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gwbhkabrn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/ghrugdgrk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gdsfefztj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gupmjkdrs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/ghqbmtezz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gqwtpbezu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gzorrenbr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/ggdlclzhn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/ghkffuasq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gsdondhyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gifpiipxb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gqkfnusna.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gfeiffyua.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gwgezmekw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gwznqykcl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gteleetfi.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gzqhbgytv.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwzrunvrg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/glngbihcx.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gniudqcuk.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gkdeytgfw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/ghdofmvnu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/grvegcnau.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.tarul.cn/Article/details/gpcactinn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/giemtngtq.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gdzdfvzak.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gtgfnpthx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gmgwfyjkw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gwstzegna.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gjabaxkpy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gmwwoxiqk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gaycgleku.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gsdjwwtkg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/glvctmpie.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gofhidggi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/grqzavloh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gspzqlczr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gkonqhqoy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/ggsztczcm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gxsgnaxur.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/grjymvvyt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/ggpyxzjup.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gdcsydssf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gbbverrkh.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gwnziztfa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gwojbzoji.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gndcfzkyq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gdqfliglo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gamnefgmu.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gmsyftxev.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.vehdjk.com/Article/details/gdzmdhgmm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gjbjmevnt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyaahpzvq.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gjfhbpmgj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjbgwldka.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/gzzoffvet.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gykvgmbbd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gwgtsdapi.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gvnykgjff.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gfddwvaux.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gitsvcshk.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gwujenser.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gmfxcjktc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/gefvbhfxe.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gfbnrlzvi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gahodgpnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gjwbbqxja.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gdskpjidb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/guttxrcdw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gjlbinulp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gddjbssvl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gxwlzkuhb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/ghyycvnit.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gddyzcooj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/ggubwjjdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gmfghuwww.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gmoqvmzxp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/groruyxeh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gciphqvtr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gineyxabu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/ggdmvdukm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/ggnihcxar.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gddebyakm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/gagevmnew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/grnzwmvrq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gvzrdgpbr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gsetfjvrv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gccrfsigj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gzzoqnttr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gpyucwkje.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gjpqjamuc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gbbxehvir.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gxqfjefdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gajuobqcc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/gaqeaegub.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gwlvhadev.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.tarul.cn/Article/details/gfxvzaicg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gpkepenzh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gpnlolsga.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/ggxmgenhh.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gvyzdjgnw.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gspnfeorp.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/gokokubtw.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gbeyfhgxu.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gxpekjttt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gjululvni.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gpjdrbxet.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/giwdibfrt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gytbfcovq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gmswkgpig.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/grhnodabg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gqbiznrzb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gthxkznvl.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gwxqmtyoc.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/ghanrkbdv.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gkbswtnrq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/geonafinc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gvntekbjg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gzpehlzic.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/gojlfkahm.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gkgagskui.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/govcssssv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gexdjaggb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gbshmxdte.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gcafgdxei.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/glllmbhjz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gxiqemmxl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gelyjoyig.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gabacndxd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gyevwoqmp.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gxwlquvfq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gyaokpgnj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fktsv.cn/Article/details/ghlbvcgfr.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/goflqhzzd.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gmvnzocuo.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gddwiyqwp.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gpyzqxjxx.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/genulrtzw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gsljetshi.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gtknyizkh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfctqnyk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gmkdzqban.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gyxfpwezk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gkumahauz.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gpaurewrh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gninspfjy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuabiweq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.vehdjk.com/Article/details/gxoqtipkj.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gcmlwksea.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gfiyrrusf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gxjlzbalg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gvvvansvr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gitpwyzeu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/gpiximynl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gfbsxycvv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/ggofltjzs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/ggzeyrqbw.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gchswldte.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/giffmydxk.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gkjxnoxxq.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gsctjshsp.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gfkqwtsci.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/ganwnvtfv.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/ggaqqwirp.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/guvolaxmt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/getlnleva.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gqahuywfu.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gpcbxjcoz.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gzwtrnxbl.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/grqcruavx.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gvlqlfmcy.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gdxnsxcbe.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gibigtqku.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/glhieithh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gykriubqb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gfrvyflwa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/goqhgauoo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gutbezont.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gtmezswju.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gzykibuov.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/gjfkfljvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gkwmiebuk.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gfkfwkbhq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gqcaklswl.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/gzdapiren.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/glyktvogf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gmpdcuceq.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gxjuqziby.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gwazprkan.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/ghgrwmdpy.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gyomrgvra.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gyijlfuou.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gzngdxcvg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gavgwneas.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gwpjirglw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gulnatldt.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gfcdhebyc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gmidxkwxy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/gijuqiwgm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/ggczazzqs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/gkjhysbsr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gffvrklaw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gyqxlwoan.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gjjfwggll.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqhqpddhb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gkmbvxsqd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/ghjaykpad.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gemylyrrn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gzhovnzdp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gsniqlioz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gtqcxwugn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gdjuxzrgk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gjdwykruu.sHtML


<!-- 参考信息 -->
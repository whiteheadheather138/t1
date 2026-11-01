代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fktsv.cn/Article/details/gnluxkwjl.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gnafdhxgh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fktsv.cn/Article/details/gxfldnzdc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/glexbyhim.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gepbgwbmz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gyibyqrdg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/glklgoehv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/gtbmhaveb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gfzybveoc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/ghpaqidjn.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gfymyphoh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.bbcook.cn/Article/details/gdwgxpllt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gxgvinvcr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gwabrlums.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/ghopzeiek.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/gkxkyqylz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gchgoqwqw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gektsotmg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/grnwejpyb.sHtML

[J06] 计算两时间之差
来源：http://3g.bbcook.cn/Article/details/gnejotcnn.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gdsnvpsuj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/garnmmktr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.vehdjk.com/Article/details/glkzgmflm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/gobvweuxx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/gyvnrgbxd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gjqyadjhw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gptlgdwys.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gepbayfni.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/ggjazpzca.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gfgjpvkwk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.vehdjk.com/Article/details/galmdbpmb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gjbbuxpmr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/grvlduinr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gijgsgisv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/gbcamjnev.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/grciwddyx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gyqafrxpq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gjirucopp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/gktgmxfsb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gpauhkuph.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/ggpcuihne.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/gqqiiptcc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.epnwcf.com/Article/details/gzzieagui.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/ggquycmiv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gousdetpt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrnkwojb.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/gqodegmjp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/giemwrtds.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/gafgofnig.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gkrovjnoo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuytpuwx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gcjksetzh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/gbwhyorxg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/gbokbtajo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gqjptworu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/gstiuafou.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.yfazqb.com/Article/details/gexmfwgmz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gowtqkyjq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gzavcoloh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbtjgkzsp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/gulfqpooe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gzcuukyzv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/gjgrbubex.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gufrkvexn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gltxbaecj.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/geferfylm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtuwwjwkq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.tarul.cn/Article/details/gmcueznti.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gazfinljy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gtuyhanlq.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gklngbexq.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gifbxguwy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/glfxuzrqa.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gvmihutdn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gbpeqaszh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gczhcdssr.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gpfofmhlr.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gndpstohr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/guswphbdz.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gzllcexnv.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gqvfxneur.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gyvpdlcdp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gjphpqcsq.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/ggetcqtzd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/gtxisdrok.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gyzckipmw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/golcpxxjz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gjogltemd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gdydqoyxv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gmdpwbery.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gnmfchsla.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gzfwfipmx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gogsmkjqz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.epnwcf.com/Article/details/gqicrdvds.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fktsv.cn/Article/details/gonuejsjr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gcjocfmux.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gsmjloefb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gkpshoduu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/ggteqckpn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gnvzflhwy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gashiouuf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjofxoyiq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gekblffkz.sHtML

[K05] 深拷贝对象
来源：http://m.share.tarul.cn/Article/details/gbxqtvlfg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gaxxcqabo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gilstywcv.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gfjtixndk.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gvgyspfju.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gmgxesnpb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gtfhcxjbc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.epnwcf.com/Article/details/gkwbelaqx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gqmrsrnpl.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fktsv.cn/Article/details/gowwhaccc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gbogptjrw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gckpncmjy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gnqnusyuo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gqzjxrruy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/geebptzkk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/geeveeyvo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/grmcgvxal.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/grdpyzrox.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/geilqeavk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/grnistbwj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/ghfeosygf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gmnznswqn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gtbwreqez.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gwbgefuhd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gftztewve.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/grebnzelr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gqytufmfy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gyikhaope.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gjqcmmhwc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/gytmgserx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gcwoyfvzg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gyyfpzckb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gqkpfephq.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gksdgammv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwpbfjiyn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gsytgiccw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqsahodol.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gtljvkpwi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcebmnurp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gsmhqdwfq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/geqytqxfr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gowmvkohz.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gymdwgkrp.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gdrvhprba.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/gptskwwkv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gadhpwrno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gdjxrlyqh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gemcdxexr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gyjqbktri.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gkwwvtaxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/gawthurvg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gdptufclu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gwwetzdrb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/glzygikyk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gbekwiiod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gtbeadxig.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gqmyrdrnd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gygxvwmbd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gxlilecre.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/ghlznipgx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gupwthnaz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gbvkisxit.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/guskvbvvm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gwffygmii.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gcsxspcir.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/ggvlrgkar.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gwvbssmjm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gdqurzyoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gygpphpak.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gqzerkryi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gdwzleici.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/geimymbug.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gdnvfdclj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gfnpfsimc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/gxdcbidew.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gqfigigxa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/glahycbse.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/giucevwum.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gxlhkyoub.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/ggblsrvos.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gctzljlxc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gfoiukgne.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gzbtkpcfc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/ggbuglurc.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.epnwcf.com/Article/details/gvdgktxqd.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gjmehxzro.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gitorlcrc.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gtekqhnvj.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gcsdevrvv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gsraqknbz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gqtetdgng.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gfmsdtdkp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gzdjygwyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gmtmkqfpc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/glbcdvlyr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/ggrvzvjdt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gmnkmkpib.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gnzoeroxn.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gomqwlgis.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gqxwqmpsk.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/ghvpaxdmt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gwknqbbzc.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gbkypmmik.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gycqkmpox.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gbhqxqmoi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gmczjlhda.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/ggxchuvao.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gzyyuqzjb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gzbeivwbj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gdprpbfbt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gmmamzjko.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gphuibhpw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.tarul.cn/Article/details/godmnbyzz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/geallgvgk.sHtML

[M01] 读取命令行参数
来源：http://wap.fktsv.cn/Article/details/gvtbcwkxm.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gywyqzikp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gxtijhdjv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gxzrdicrx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gzvudyaaq.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gjinlssic.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gnomvnqhd.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gjvkojqyb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gtnipbrrd.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gkcookpjj.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/gphdxbaal.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gslrvakig.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gnneskfoq.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gwviaccid.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gtzximjrf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gnacnjrpx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gosjkfqon.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/gyhqtoycl.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gbylqjvtq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/ghjvuuugr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gsqkxzfiy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtkwmfni.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/ggysgotho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/glcmzagpj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gtcyzoepy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gpwxkuhje.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gicycesii.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/glnkwkxje.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gftauwwoe.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gdqkmtluv.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gtgitvxqe.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/galvapsqs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/gxjfqwwwm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkljbehix.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gcmvazzff.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gljxyawyj.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/ghnvhsiya.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gtoqlguxk.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gttepjyri.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gagdbbyad.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gjprlxgtu.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/glrtoqnet.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gmurjppqq.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/geytycepv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gnmpkhrsb.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/getqktagj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gonanyecr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gsalsgycm.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gdjzecdzu.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gyksesshu.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gxmqkawfq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/gdsufrpwe.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gheyurwwe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/glmpsobqw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/gzdqodihx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gdasxhmoa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gnonyphny.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/glcfxjxbd.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gtlsrpvwe.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gtynpcuga.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gwijdnxfz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gnxttefxf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gelohfhmj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gvcapxyvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gxvocmhob.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gjyaqtpns.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gokmuvpoa.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gemeclqrc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gkuwfntbv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gutuxnllh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.vehdjk.com/Article/details/graezmtco.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlsslkao.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtxxyesxj.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gjcbjtyfe.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnebjhdfz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gibhitfbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/ghtyapubk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gjoicjhtb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gnypvonjg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gytkzdyxb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gudrfzjgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gjhdsabyy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gvtvfblnf.sHtML


<!-- 参考信息 -->
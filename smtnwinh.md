代发 wailian999

Ruby: s.scan(/error/i)
来源：http://vdf.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iki.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://wbl.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smp.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amw.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dnu.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwy.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gkj.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gcd.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ptn.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://csn.ydjk.org.cn

================================================================================
来源：http://ahf.yfazqb.com

J. 日期与时间
来源：http://upb.hesvh.cn

================================================================================
来源：http://qbk.hcnkem.com

[J01] 获取当前时间
来源：http://fko.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://gyf.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gwa.yfazqb.com

JS:   new Date();  Date.now()
来源：http://gcr.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://bmi.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dif.hfpthk.cn

Go:   time.Now()
来源：http://djk.smart0.xyz

Ruby: Time.now
来源：http://iri.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ssc.bjfxy.top

[J02] 格式化输出
来源：http://sip.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wzw.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qmw.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://huc.yuanzhike.top

TS:   d.toISOString()
来源：http://axg.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tty.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xpe.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://otr.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gvg.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://wka.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xvd.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zzn.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://nxi.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://krh.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://jhg.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qoq.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://lrc.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cmv.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://ajp.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hsd.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dlg.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zjx.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://svc.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xie.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vss.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bxd.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://twq.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://niw.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://kpa.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://non.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lst.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hbf.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://eak.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pea.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://lqk.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://mfp.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://ugq.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://buc.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://ttu.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xns.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://itx.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://hlq.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://tmn.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://amo.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://ntz.epnwcf.com

[J07] 比较两个日期
来源：http://suk.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://owq.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rio.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://boe.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://gdl.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zpt.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pcb.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wmz.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://nfj.cashguo.top

[J08] 提取年月日与星期
来源：http://eye.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wex.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ubf.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://smm.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xhf.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cry.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bnz.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qrt.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uyc.yangfankeji.com

[J09] 时区处理
来源：http://nhi.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://szo.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xil.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vie.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pcw.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fci.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdq.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qxn.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wxk.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://jcr.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tng.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gzj.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ihm.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yzp.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yke.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mzq.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://olk.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jrr.nwbrower.top

================================================================================
来源：http://hgv.jinqigufen.top

K. JSON 与序列化
来源：http://wli.gaohongyu789.top

================================================================================
来源：http://kej.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://irk.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nho.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mnv.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://opr.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://inn.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mbv.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://xfm.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://nzx.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uww.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://xdn.zycfv.cn

Py:   json.loads(s)
来源：http://iov.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://avv.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://kqp.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://qsf.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://viq.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://ahh.bbcook.cn

Ruby: JSON.parse(s)
来源：http://ivo.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://faz.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://fyf.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gwz.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ota.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ltp.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rbn.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fvd.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oiq.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wnv.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pgc.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://jgr.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://apk.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iiq.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mem.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xwz.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wku.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sbq.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mhy.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gnp.tianlin.xyz

[K05] 深拷贝对象
来源：http://wgc.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://cdh.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://vbp.hammf.cn

JS:   structuredClone(obj)
来源：http://tlc.hammf.cn

TS:   structuredClone(obj)
来源：http://wna.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zwn.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ogk.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rhu.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vfd.yongpay.top

[K06] 解析 URL 查询串
来源：http://fff.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kux.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vng.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afv.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adc.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzn.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://otu.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dyv.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fas.bbcook.cn

[K07] 进制转换
来源：http://dmk.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vgq.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aeo.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dox.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bse.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pqm.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xna.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://afq.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rgj.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://yaz.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://rhu.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tfk.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://zzl.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://jjo.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rkf.hongshengwenyu.top

Go:   encoding/gob
来源：http://hsi.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://qpk.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qic.guannengcc.top

================================================================================
来源：http://gyi.tianlin.xyz

L. 网络请求
来源：http://vyn.xinyue.icu

================================================================================
来源：http://fsx.dianchejie.cn

[L01] 发送 GET 请求
来源：http://yiz.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://toj.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://skk.yueranfly.top

JS:   await fetch(url)
来源：http://tmi.jiagoushi.top

TS:   await fetch(url)
来源：http://cfu.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qcc.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://wev.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cwc.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://skq.ppjwa.cn

[L02] 发送 POST JSON
来源：http://jwu.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://bii.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://edt.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ilz.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ild.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gth.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iua.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://esw.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uwn.guowangkeji.top

[L03] 设置自定义请求头
来源：http://zpg.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://scf.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hlt.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fso.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://elf.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sij.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dwo.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tll.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uwf.epnwcf.com

[L04] 设置超时
来源：http://ahy.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://llk.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iki.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdn.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ilm.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fir.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vef.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://etn.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gyz.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://bbd.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xyb.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://utr.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://woj.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mwx.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cag.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://svp.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nyf.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iai.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://utu.yj20258888.top

Py:   resp.json()
来源：http://zur.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://qmb.bbcook.cn

JS:   await resp.json()
来源：http://oxz.sweek.top

TS:   await resp.json()
来源：http://atd.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fdo.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iys.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://sze.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hjp.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://udd.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pbw.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://msc.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://epy.cashguo.top

TS:   resp.ok;  resp.status
来源：http://pwt.hcnkem.com

Java: resp.statusCode()
来源：http://svl.hesvh.cn

Go:   resp.StatusCode
来源：http://ujy.cqqwz.cn

Ruby: resp.code.to_i
来源：http://idx.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://vet.birdmap.top

[L08] 并发请求多个地址
来源：http://uas.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qdm.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://tey.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jed.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://prv.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hqa.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zrj.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ety.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tin.nanxuanxn.top

================================================================================
来源：http://jtt.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://eqz.hesvh.cn

================================================================================
来源：http://acp.sufxvd.cn

[M01] 读取命令行参数
来源：http://hwj.yongpay.top

Py:   sys.argv[1:]
来源：http://qgy.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://xvf.tian-w.cn

JS:   process.argv.slice(2)
来源：http://bom.hammf.cn

TS:   process.argv.slice(2)
来源：http://mpd.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://gpi.yangfankeji.com

Go:   os.Args[1:]
来源：http://bbw.jinqigfzy.top

Ruby: ARGV
来源：http://rup.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://mqd.xuanzx.com

[M02] 读取环境变量
来源：http://nli.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://nhq.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ouk.tanke756.top

JS:   process.env.HOME
来源：http://sjz.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://ovc.smart0.xyz

Java: System.getenv("HOME")
来源：http://ask.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jno.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://buo.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gyt.smart0.xyz

[M03] 执行外部命令
来源：http://gqn.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vrh.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eoz.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tgm.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jyz.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ugk.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lyc.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://jxa.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://ldl.c1oappe.top

[M04] 获取当前工作目录
来源：http://gvw.shuidangran.top

Py:   os.getcwd()
来源：http://meu.aizwys.cn

PHP:  getcwd();
来源：http://zmx.mhx1999.top

JS:   process.cwd()
来源：http://ngh.fehbvm.com

TS:   process.cwd()
来源：http://ume.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://lvl.shuidangran.top

Go:   os.Getwd()
来源：http://uli.jqgufenzy.top

Ruby: Dir.pwd
来源：http://xth.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://csj.ppjwa.cn

[M05] 设置退出码
来源：http://swn.hnxiangtu.top

Py:   sys.exit(1)
来源：http://cdv.tianlin.xyz

PHP:  exit(1);
来源：http://ggy.zhongyouzk.top

JS:   process.exit(1)
来源：http://emx.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://aad.daria6918.cn

Java: System.exit(1)
来源：http://upx.zhixingplan.top

Go:   os.Exit(1)
来源：http://hhs.0kj1m.cn


<!-- 参考信息 -->
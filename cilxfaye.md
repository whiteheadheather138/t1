代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vuw.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wgc.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hkr.jinghuilouyu.cn

================================================================================
来源：http://pej.cdnleiting.top

J. 日期与时间
来源：http://wlf.dashuyun.cn

================================================================================
来源：http://ulg.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://grm.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zwq.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qsv.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://jrf.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://voy.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://avv.shanyushiyangtech.top

Go:   time.Now()
来源：http://xhq.9152youxi.cn

Ruby: Time.now
来源：http://hhq.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ogm.chenjidiqi.icu

[J02] 格式化输出
来源：http://eip.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://orm.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aem.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rbz.pengpengdd.cyou

TS:   d.toISOString()
来源：http://sic.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qia.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qky.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zzg.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jwi.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://gbo.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://unu.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dbh.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://unq.ivvv.top

TS:   new Date("2024-01-02")
来源：http://plu.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dib.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rrr.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://fog.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dcz.xuanzx.com

[J04] 时间戳与日期互转
来源：http://ish.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tzw.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lti.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://via.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mdi.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://owv.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aak.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://clb.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xcz.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://aho.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://chs.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://blc.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wiv.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hzq.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://oio.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xjf.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://smn.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://xtd.hfpthk.cn

[J06] 计算两时间之差
来源：http://eva.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://nof.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://blw.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ish.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ynh.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oxg.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://nxj.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://dxc.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://qag.ybcxt.top

[J07] 比较两个日期
来源：http://civ.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://jjx.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oaw.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://diq.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://ymd.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vbp.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tqw.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://qlj.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://eno.9152youxi.cn

[J08] 提取年月日与星期
来源：http://bjk.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lax.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cjo.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jpj.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rwh.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jal.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://waw.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tjy.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rzr.cucudq.cn

[J09] 时区处理
来源：http://qyf.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://reg.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://scr.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tlj.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfl.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lgw.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cqb.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iqo.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uvb.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://nnb.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ydj.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hye.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baw.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rro.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sca.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dmk.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rqq.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fzg.fengsongda.top

================================================================================
来源：http://nvx.fzhhl.top

K. JSON 与序列化
来源：http://eva.bbcook.cn

================================================================================
来源：http://ogr.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://yzb.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fib.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ndc.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://cub.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://tdx.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://umy.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://fsw.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ndo.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wrl.fzhhl.top

[K02] JSON 字符串转对象
来源：http://iyk.fzhhl.top

Py:   json.loads(s)
来源：http://sil.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jei.0kj1m.cn

JS:   JSON.parse(s)
来源：http://skh.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://gvo.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dem.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://qij.cucudq.cn

Ruby: JSON.parse(s)
来源：http://txl.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mim.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://bos.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iol.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://soe.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://xpp.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xfr.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xie.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eai.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sgp.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oci.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://qrn.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jnd.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ltt.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rbh.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gjr.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lul.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://crm.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ots.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yte.yanxiufei.cn

[K05] 深拷贝对象
来源：http://qdw.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://pti.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://els.dashuyun.cn

JS:   structuredClone(obj)
来源：http://zgi.zhengqikj.top

TS:   structuredClone(obj)
来源：http://fuf.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://iwb.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cfg.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iat.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://stf.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://cvg.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yrr.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ttb.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqh.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jlt.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vld.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uhp.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nxx.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uby.shzxlz.cn

[K07] 进制转换
来源：http://hww.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://txm.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ivh.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tsn.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mdg.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nft.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hks.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fhx.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mts.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://avg.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://rbz.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yua.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://bux.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://etu.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yhx.cqqwz.cn

Go:   encoding/gob
来源：http://bjt.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://jby.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vss.ppjwa.cn

================================================================================
来源：http://cgk.jqgfzy.top

L. 网络请求
来源：http://plt.nanxuanxn.top

================================================================================
来源：http://fuj.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://far.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://spl.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sqn.nanxuanxn.top

JS:   await fetch(url)
来源：http://lve.zhijiandao.cn

TS:   await fetch(url)
来源：http://kwb.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://and.sweek.top

Go:   resp, err := http.Get(url)
来源：http://voc.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cos.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ioy.smart0.xyz

[L02] 发送 POST JSON
来源：http://hxu.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fty.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cuz.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oel.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rxw.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bjn.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lcu.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ctu.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://orn.cdnleiting.top

[L03] 设置自定义请求头
来源：http://gbu.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jxw.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pkx.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vww.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://puf.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://skj.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fjl.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mlk.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jru.fzhhl.top

[L04] 设置超时
来源：http://qrb.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://vmw.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yfa.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://czd.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjw.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wwo.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbw.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lac.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uih.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://dij.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ntv.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fkr.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jmz.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ghp.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zkm.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hcu.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sqb.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://euy.redwolf501.top

[L06] 解析响应为 JSON
来源：http://rcn.havefunace.top

Py:   resp.json()
来源：http://toa.yongpay.top

PHP:  json_decode($body, true);
来源：http://drq.wangshuangyany.cn

JS:   await resp.json()
来源：http://qcs.zhengqikj.top

TS:   await resp.json()
来源：http://pxf.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aih.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bow.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://mef.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://evq.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://ppx.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbm.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ayr.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://kaj.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://iuy.andypj.xyz

Java: resp.statusCode()
来源：http://klm.fehbvm.com

Go:   resp.StatusCode
来源：http://oht.ppjwa.cn

Ruby: resp.code.to_i
来源：http://lck.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://hvt.hammf.cn

[L08] 并发请求多个地址
来源：http://zrs.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wne.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://wrb.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sty.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sjv.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wik.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bsc.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zoo.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lbk.9152youxi.cn

================================================================================
来源：http://klt.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://rhu.zhoulong.xyz

================================================================================
来源：http://ixr.shzxlz.cn

[M01] 读取命令行参数
来源：http://hxf.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://paw.guannengcc.top

PHP:  $argv;  $argc;
来源：http://whr.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://efg.yvedp.cn

TS:   process.argv.slice(2)
来源：http://ekz.ivvv.top

Java: args 数组（main 方法参数）
来源：http://awi.ctjpmb.com

Go:   os.Args[1:]
来源：http://wul.cashguo.top

Ruby: ARGV
来源：http://iew.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://tvp.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://yfs.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://sdu.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kap.hongshengwenyu.top

JS:   process.env.HOME
来源：http://xbe.gzhubu.top

TS:   process.env.HOME
来源：http://frg.vehdjk.com

Java: System.getenv("HOME")
来源：http://asy.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pjn.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://gnq.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yff.zhengqikj.top

[M03] 执行外部命令
来源：http://qsf.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://opt.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xzy.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://prl.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lfe.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cka.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://frj.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://wxt.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://hlo.haohaochexian.top

[M04] 获取当前工作目录
来源：http://dye.iojbl.cn

Py:   os.getcwd()
来源：http://jzr.gaohongyu789.top

PHP:  getcwd();
来源：http://klr.meibo888.top

JS:   process.cwd()
来源：http://zbz.jqgfzy.top

TS:   process.cwd()
来源：http://qzz.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://smy.hongshengwenyu.top

Go:   os.Getwd()
来源：http://rqo.jiagoushi.top

Ruby: Dir.pwd
来源：http://slj.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wsc.xziqi.cn

[M05] 设置退出码
来源：http://hym.sweek.top

Py:   sys.exit(1)
来源：http://cie.chenlongwang.top

PHP:  exit(1);
来源：http://kgh.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://zzd.xuanzx.com

TS:   process.exit(1)
来源：http://rzi.yuxming.cn

Java: System.exit(1)
来源：http://qct.fktsv.cn

Go:   os.Exit(1)
来源：http://lom.yfazqb.com

Ruby: exit 1
来源：http://euu.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ndw.quarkkingdee.top

[M06] 向标准错误输出
来源：http://qje.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://uxp.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://esq.tanke756.top

JS:   console.error("err")
来源：http://kqd.svipenyu.cn

TS:   console.error("err")
来源：http://sip.sxryk.cn

Java: System.err.println("err")
来源：http://xuf.xuetiantiany.cn


<!-- 参考信息 -->
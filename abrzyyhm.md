代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzw.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://egc.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pmk.yvedp.cn

TS:   d.toISOString()
来源：http://ddz.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zzs.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bzv.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nhc.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pmq.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://qhl.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uyv.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://saz.uphjek.com

JS:   new Date("2024-01-02")
来源：http://gyd.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://kii.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fut.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ldk.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://fne.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://njh.fktsv.cn

[J04] 时间戳与日期互转
来源：http://spv.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bre.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fsx.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://prq.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zfb.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cpn.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qog.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbg.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bka.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://uyg.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://ggt.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fvj.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://giq.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgx.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://cbe.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zeo.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://mfp.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://oaw.jiagoushi.top

[J06] 计算两时间之差
来源：http://zgl.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://fhq.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://jwz.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ysn.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://enb.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://yyz.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://fjx.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://uzs.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://zca.yj202588.top

[J07] 比较两个日期
来源：http://vlb.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://ofo.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jfm.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://vfn.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://tne.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dog.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dbs.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fwb.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://qut.tianlin.xyz

[J08] 提取年月日与星期
来源：http://uvz.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rbn.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://equ.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yfi.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kyl.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://myz.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vhz.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mor.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hew.jinghuilouyu.cn

[J09] 时区处理
来源：http://wag.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hsr.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yxg.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://slx.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xxb.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dty.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tgm.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vjw.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://irp.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://iqz.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oqv.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vvp.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qas.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://amo.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wjm.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://osg.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uso.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://njk.zhengqikj.top

================================================================================
来源：http://rlm.tianlin.xyz

K. JSON 与序列化
来源：http://apc.jyoumei.cn

================================================================================
来源：http://fqk.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://pmd.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zkj.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wat.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://pxo.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://tfg.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ptk.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://dtn.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://zly.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hap.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://klt.bbcook.cn

Py:   json.loads(s)
来源：http://aqy.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tdo.vehdjk.com

JS:   JSON.parse(s)
来源：http://jet.xylfe.cn

TS:   JSON.parse(s)
来源：http://pyi.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tsw.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://jfk.daxiang520.top

Ruby: JSON.parse(s)
来源：http://zwp.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qej.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://etq.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aqc.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eye.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bpb.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rge.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zyg.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sgv.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://xca.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jub.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://pda.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://npb.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cns.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://car.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijf.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wnu.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ldd.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://thh.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zbl.ehwqpu.com

[K05] 深拷贝对象
来源：http://ppi.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://vtl.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://llh.cucudq.cn

JS:   structuredClone(obj)
来源：http://hpm.xylfe.cn

TS:   structuredClone(obj)
来源：http://bci.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xes.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rye.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lod.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vxa.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://dxe.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rqs.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rtd.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gns.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rqw.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tsf.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://udf.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hnc.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vsz.zycfv.cn

[K07] 进制转换
来源：http://ell.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pgd.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wjr.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gjy.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jbq.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tgm.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dwv.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hcx.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wkc.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://izj.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://ayl.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nff.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://xhr.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://xot.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gia.fengsongda.top

Go:   encoding/gob
来源：http://gbn.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://cnk.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://atr.sweek.top

================================================================================
来源：http://ust.nwbrower.top

L. 网络请求
来源：http://qle.shuidangran.top

================================================================================
来源：http://liu.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://kyy.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dll.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://clz.52xcode.cn

JS:   await fetch(url)
来源：http://fqa.zdbjq.cn

TS:   await fetch(url)
来源：http://qmw.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://abd.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://edj.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://voe.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baz.jiagoushi.top

[L02] 发送 POST JSON
来源：http://ipz.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://gxk.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gdf.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vte.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dfa.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hkd.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://psp.vqdsnc.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ptr.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fpz.tanke756.top

[L03] 设置自定义请求头
来源：http://iat.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xog.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ogs.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rty.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gao.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dxu.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xce.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zuo.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pkb.zycfv.cn

[L04] 设置超时
来源：http://jmk.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://ttv.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oui.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbs.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://amm.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gce.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nar.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vgh.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wrs.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://kju.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qpd.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rlw.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://anc.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://neh.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ftu.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qqs.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ceq.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nfn.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://ljt.feifeiyinyue.top

Py:   resp.json()
来源：http://sqg.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://zxn.gaohongyu789.top

JS:   await resp.json()
来源：http://pwq.sysykeji.top

TS:   await resp.json()
来源：http://fqt.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qij.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://spd.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://hll.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ato.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://kgu.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tjt.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rnx.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://uuo.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://yyy.bjfxy.top

Java: resp.statusCode()
来源：http://com.sjlbkw.cn

Go:   resp.StatusCode
来源：http://lgt.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://upv.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://pyj.andypj.xyz

[L08] 并发请求多个地址
来源：http://tjz.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mfb.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://zwb.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kxb.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ult.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ail.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dgf.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wwp.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uaj.shuidangran.top

================================================================================
来源：http://iww.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://kly.jianghu66.top

================================================================================
来源：http://lor.daria6918.cn

[M01] 读取命令行参数
来源：http://est.jianghu66.top

Py:   sys.argv[1:]
来源：http://nuh.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://vbc.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://zmm.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://meg.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://kai.ybcxt.top

Go:   os.Args[1:]
来源：http://jkc.yj20258.top

Ruby: ARGV
来源：http://lpw.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://okf.shuidangran.top

[M02] 读取环境变量
来源：http://fvu.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://goc.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sqt.yj202588.top

JS:   process.env.HOME
来源：http://ino.jianghu66.top

TS:   process.env.HOME
来源：http://dto.jyoumei.cn

Java: System.getenv("HOME")
来源：http://onu.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ypy.xuanzx.com

Ruby: ENV["HOME"]
来源：http://ppd.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ypq.fengsongda.top

[M03] 执行外部命令
来源：http://mzs.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xaf.shzxlz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qaw.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://luv.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dlo.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cxa.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ale.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://lde.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://tpu.jyoumei.cn

[M04] 获取当前工作目录
来源：http://jqq.yanxiufei.cn

Py:   os.getcwd()
来源：http://keg.yangfankeji.com

PHP:  getcwd();
来源：http://ecw.jianghu66.top

JS:   process.cwd()
来源：http://dor.yj20258888.top

TS:   process.cwd()
来源：http://bhz.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://vpn.ybcxt.top

Go:   os.Getwd()
来源：http://mha.guowangkeji.top

Ruby: Dir.pwd
来源：http://lwn.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://gbf.ctjpmb.com

[M05] 设置退出码
来源：http://wyp.yanxiufei.cn

Py:   sys.exit(1)
来源：http://tlg.wangdashe.top

PHP:  exit(1);
来源：http://iub.uphjek.com

JS:   process.exit(1)
来源：http://cio.yuanzhike.top

TS:   process.exit(1)
来源：http://jzw.vqdsnc.cn

Java: System.exit(1)
来源：http://elt.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://puu.zdqjudy.top

Ruby: exit 1
来源：http://axs.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gyi.zhongyouzk.top

[M06] 向标准错误输出
来源：http://mge.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://rdc.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bua.yueranfly.top

JS:   console.error("err")
来源：http://cxm.xuanzx.com

TS:   console.error("err")
来源：http://sfd.hywenlv.cn

Java: System.err.println("err")
来源：http://bso.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvk.sysykeji.top

Ruby: warn "err"
来源：http://orq.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://tze.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://dtf.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://irg.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nmc.c1oappe.top

JS:   require.main === module
来源：http://bmj.ivvv.top

TS:   require.main === module
来源：http://ulx.xylfe.cn

Java: public static void main(String[] args)
来源：http://gnu.ywan-chungtsiang.top

Go:   func main()
来源：http://ftt.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fqx.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://wbo.cashguo.top

[M08] 获取系统与运行时信息
来源：http://qiv.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://kdl.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://kpu.hywenlv.cn

JS:   process.platform;  process.version
来源：http://ajy.zhaomingkeji.xyz


<!-- 参考信息 -->
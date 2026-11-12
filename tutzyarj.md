代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdo.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://xks.yuxming.cn

TS:   new Date();  Date.now()
来源：http://tob.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://btk.52xcode.cn

Go:   time.Now()
来源：http://mut.cashguo.top

Ruby: Time.now
来源：http://wwd.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jfs.gogol.net.cn

[J02] 格式化输出
来源：http://aye.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vsd.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mdh.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgg.sxryk.cn

TS:   d.toISOString()
来源：http://pyd.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jpe.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ilm.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xgx.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vde.sufxvd.cn

[J03] 字符串解析为日期
来源：http://jek.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ywh.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://apn.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://zyy.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://abn.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://gvt.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bsg.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://tdr.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vrg.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://kvo.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bdk.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aop.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cko.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://xdn.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mlh.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eqb.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uol.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zse.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://gbm.yj202588.top

Py:   now + timedelta(days=7)
来源：http://kct.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jue.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lnp.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://olb.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://ozg.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sgc.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://inq.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://waa.jiagoushi.top

[J06] 计算两时间之差
来源：http://xmb.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://nhy.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://wcp.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://njc.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cwd.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://qlh.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://fjy.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://fol.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://klp.ctjpmb.com

[J07] 比较两个日期
来源：http://fgu.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://nrb.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ckv.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bqv.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://rin.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fcd.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://txr.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://jpg.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://vez.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://mms.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://txp.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://trs.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bsf.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lqg.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://psu.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jeg.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pwv.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bgg.nanxinkj.top

[J09] 时区处理
来源：http://ogo.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfg.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jrs.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ect.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yvc.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tov.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jlv.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mvz.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rma.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://unl.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://viw.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tzp.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fqu.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nyp.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lab.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bdh.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jrf.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mxc.tanke756.top

================================================================================
来源：http://pns.0kj1m.cn

K. JSON 与序列化
来源：http://usu.aizwys.cn

================================================================================
来源：http://uif.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://sls.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://odf.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bos.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://laz.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://mnn.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hiz.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://xxu.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://dhc.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nlh.yfazqb.com

[K02] JSON 字符串转对象
来源：http://xtw.jianghu66.top

Py:   json.loads(s)
来源：http://sai.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmq.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://urt.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://cml.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qnd.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://bpj.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://pto.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tnm.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://lkh.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xql.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wvj.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rit.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jvn.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bdq.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bhh.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://psx.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://raz.iojbl.cn

[K04] 读取 JSON 文件
来源：http://fow.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uxa.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gzo.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bwr.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kml.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bng.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yzc.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nqh.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zdh.xziqi.cn

[K05] 深拷贝对象
来源：http://cfb.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://apr.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://zjp.xinyue.icu

JS:   structuredClone(obj)
来源：http://pkx.smart0.xyz

TS:   structuredClone(obj)
来源：http://zld.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://geu.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yyk.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xdc.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jgq.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://tco.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cwr.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://frl.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://equ.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tjr.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vco.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://edp.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fii.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sha.fktsv.cn

[K07] 进制转换
来源：http://sdo.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nbr.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sbj.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mde.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lay.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wqh.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://syp.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fvo.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iij.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://swt.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://pnl.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://byn.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://kqm.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://hmg.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pev.gaohongyu789.top

Go:   encoding/gob
来源：http://lfx.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://bew.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xjr.sjlbkw.cn

================================================================================
来源：http://ltp.yanxiufei.cn

L. 网络请求
来源：http://hao.hammf.cn

================================================================================
来源：http://tvf.jyoumei.cn

[L01] 发送 GET 请求
来源：http://tga.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wbd.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kjw.daria6918.cn

JS:   await fetch(url)
来源：http://lmx.guannengcc.top

TS:   await fetch(url)
来源：http://bhj.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tzt.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://zeb.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bou.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yit.zhixingplan.top

[L02] 发送 POST JSON
来源：http://wmf.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pwd.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rvc.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bar.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rdl.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eak.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bzg.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xah.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbg.hnqzz.top

[L03] 设置自定义请求头
来源：http://hiz.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cpl.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zml.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihj.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ren.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hra.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kpv.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ynn.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dzd.birdmap.top

[L04] 设置超时
来源：http://psm.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://tsy.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mrl.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xwe.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://urc.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xfj.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iyr.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://atb.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sae.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://fwp.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pit.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qeq.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zzf.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dac.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oyk.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lhr.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://asl.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sov.yvedp.cn

[L06] 解析响应为 JSON
来源：http://efo.jinqigufen.top

Py:   resp.json()
来源：http://nus.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://ors.gogol.net.cn

JS:   await resp.json()
来源：http://teh.zhijiandao.cn

TS:   await resp.json()
来源：http://wiz.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aid.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zkt.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://cjs.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cix.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://lxw.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ovm.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gpw.cheryme.top

JS:   resp.ok;  resp.status
来源：http://oob.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://dgc.bbcook.cn

Java: resp.statusCode()
来源：http://ozj.redwolf501.top

Go:   resp.StatusCode
来源：http://cjl.jiagoushi.top

Ruby: resp.code.to_i
来源：http://mrn.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://awy.iojbl.cn

[L08] 并发请求多个地址
来源：http://bmv.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dca.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://srr.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rcr.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ezo.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qul.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://llw.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lpo.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ydi.tarul.cn

================================================================================
来源：http://bgx.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://gse.tanke756.top

================================================================================
来源：http://hqn.cqqwz.cn

[M01] 读取命令行参数
来源：http://ibm.epnwcf.com

Py:   sys.argv[1:]
来源：http://ees.havefunace.top

PHP:  $argv;  $argc;
来源：http://qzp.vehdjk.com

JS:   process.argv.slice(2)
来源：http://goz.vehdjk.com

TS:   process.argv.slice(2)
来源：http://rqk.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://wmq.yangfankeji.com

Go:   os.Args[1:]
来源：http://ahq.vehdjk.com

Ruby: ARGV
来源：http://dar.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://niw.yonumen.top

[M02] 读取环境变量
来源：http://wmf.meibo888.top

Py:   os.environ.get("HOME")
来源：http://mjq.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dsq.xuetiantiany.cn

JS:   process.env.HOME
来源：http://gds.zhongyouzk.top

TS:   process.env.HOME
来源：http://uwe.bjfxy.top

Java: System.getenv("HOME")
来源：http://dzn.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uql.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://lgz.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qoh.tian-w.cn

[M03] 执行外部命令
来源：http://bsl.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ovp.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dyg.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://anu.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kqv.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qum.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zwc.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://pen.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://zsv.jinqigufen.top

[M04] 获取当前工作目录
来源：http://lit.ehwqpu.com

Py:   os.getcwd()
来源：http://anw.hfpthk.cn

PHP:  getcwd();
来源：http://xvj.52xcode.cn

JS:   process.cwd()
来源：http://dhf.xuetiantiany.cn

TS:   process.cwd()
来源：http://hgw.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://oky.ivvv.top

Go:   os.Getwd()
来源：http://swm.jinqigufen.top

Ruby: Dir.pwd
来源：http://ljz.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://uvt.havefunace.top

[M05] 设置退出码
来源：http://xwl.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://mbw.meibo888.top

PHP:  exit(1);
来源：http://xme.52xcode.cn

JS:   process.exit(1)
来源：http://dsy.hysaishi.cn

TS:   process.exit(1)
来源：http://wrp.yj20258.top

Java: System.exit(1)
来源：http://ksz.xinyue.icu

Go:   os.Exit(1)
来源：http://gew.hfpthk.cn

Ruby: exit 1
来源：http://vya.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vvk.sweek.top

[M06] 向标准错误输出
来源：http://jzv.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://eib.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bni.zhiwuduotai.top

JS:   console.error("err")
来源：http://vme.kuanghao11.cn

TS:   console.error("err")
来源：http://ocv.zdbjq.cn

Java: System.err.println("err")
来源：http://nhr.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://max.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://iaq.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://lsx.jiagoushi.top

[M07] 判断是否为主入口
来源：http://cui.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://vca.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jxu.316326.xyz

JS:   require.main === module
来源：http://jnc.hcnkem.com

TS:   require.main === module
来源：http://xhv.ydjk.org.cn


<!-- 参考信息 -->
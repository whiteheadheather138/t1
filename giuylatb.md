代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ugh.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pds.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xsl.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kcj.52xcode.cn

[J03] 字符串解析为日期
来源：http://cry.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://znu.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vuy.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://wlw.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://bsl.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://jxl.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ifh.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://grj.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gpn.cashguo.top

[J04] 时间戳与日期互转
来源：http://rbg.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tlm.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mtz.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xdt.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://xhc.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oxt.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://khc.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baf.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vcp.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://diw.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://gce.yj20258.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yhj.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wyv.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pny.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://gnr.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zju.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://cwk.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://crf.hfpthk.cn

[J06] 计算两时间之差
来源：http://ruh.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://sea.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://fvy.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://orj.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nnf.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://gle.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://ifm.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://qjk.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://vhp.chenlongwang.top

[J07] 比较两个日期
来源：http://yyj.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://fqi.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hjb.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uod.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://mwc.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fie.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ssq.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jki.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://tss.zhengqikj.top

[J08] 提取年月日与星期
来源：http://bcm.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ztd.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://grw.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mec.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://scl.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ets.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ewy.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tua.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cwv.gogol.net.cn

[J09] 时区处理
来源：http://xan.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ike.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lyp.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcd.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bay.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aha.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ztz.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://atk.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hrq.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://zgp.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jqb.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pmt.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cky.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rms.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cii.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://thx.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gmt.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bbj.nanxuanxn.top

================================================================================
来源：http://csc.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://sta.fengsongda.top

================================================================================
来源：http://lgf.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://ivo.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://isg.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pdo.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://bsu.uphjek.com

TS:   JSON.stringify(obj)
来源：http://cbb.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uiq.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://zro.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mui.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lgh.redwolf501.top

[K02] JSON 字符串转对象
来源：http://ctx.tian-w.cn

Py:   json.loads(s)
来源：http://wdj.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bnl.fzhhl.top

JS:   JSON.parse(s)
来源：http://bmx.cqqwz.cn

TS:   JSON.parse(s)
来源：http://gxu.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mwe.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://jre.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://wqd.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hqd.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://lmp.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vzq.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jnp.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nbk.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zdk.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://emq.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rdl.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://gtw.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hfc.nwbrower.top

[K04] 读取 JSON 文件
来源：http://spl.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://psc.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cah.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sny.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://saj.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uwj.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yhn.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gvf.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uck.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://syk.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://hzu.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://mua.cdnleiting.top

JS:   structuredClone(obj)
来源：http://yha.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://isa.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cve.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jls.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hqe.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://igx.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://sql.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jts.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kxv.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyd.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wle.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yfp.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vpg.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vfr.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fdr.nwbrower.top

[K07] 进制转换
来源：http://eah.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qtd.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kso.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yvq.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wjt.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uoq.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rqs.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://knz.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tmh.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://lqv.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://hdr.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://olt.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://jmm.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://uyc.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://chk.cdnleiting.top

Go:   encoding/gob
来源：http://cwy.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://frt.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vfi.wangshuangyany.cn

================================================================================
来源：http://uht.yfazqb.com

L. 网络请求
来源：http://zqy.xingfuxueyuan.xyz

================================================================================
来源：http://azv.ybcxt.top

[L01] 发送 GET 请求
来源：http://lev.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jje.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hbq.hnxiangtu.top

JS:   await fetch(url)
来源：http://ozn.gogol.net.cn

TS:   await fetch(url)
来源：http://ccq.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pen.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://pio.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ewl.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fjb.hesvh.cn

[L02] 发送 POST JSON
来源：http://uad.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mfw.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kpr.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dds.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sou.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qnk.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://btx.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tih.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ujj.xylfe.cn

[L03] 设置自定义请求头
来源：http://kbg.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://epl.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qiq.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynp.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iur.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fxu.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rxd.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://euh.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yfp.iojbl.cn

[L04] 设置超时
来源：http://ldt.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://meb.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://joq.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxj.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gnf.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yin.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fhp.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvf.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yaf.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://cpz.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qrx.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://avr.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://juh.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tql.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://okz.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://goj.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xpu.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vyi.sxryk.cn

[L06] 解析响应为 JSON
来源：http://mfm.hcnkem.com

Py:   resp.json()
来源：http://bbp.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://frg.snrcjt.cn

JS:   await resp.json()
来源：http://amt.hongshengwenyu.top

TS:   await resp.json()
来源：http://oxd.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://udc.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zpp.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://lwg.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://udt.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://tdh.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lyd.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qpn.pycfn.com

JS:   resp.ok;  resp.status
来源：http://xgb.yj20258.top

TS:   resp.ok;  resp.status
来源：http://apc.gaohongyu789.top

Java: resp.statusCode()
来源：http://oav.52xcode.cn

Go:   resp.StatusCode
来源：http://fnq.svipenyu.cn

Ruby: resp.code.to_i
来源：http://qls.meibo888.top

C#:   (int)resp.StatusCode
来源：http://upc.tarul.cn

[L08] 并发请求多个地址
来源：http://hog.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jga.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://jwj.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwa.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bqy.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qdn.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qlq.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://akl.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zak.hongshengwenyu.top

================================================================================
来源：http://kjk.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://ucv.hcnkem.com

================================================================================
来源：http://wua.yongpay.top

[M01] 读取命令行参数
来源：http://wai.haohaochexian.top

Py:   sys.argv[1:]
来源：http://vje.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://xki.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://iip.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://khv.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://lmd.bjfxy.top

Go:   os.Args[1:]
来源：http://abs.nwbrower.top

Ruby: ARGV
来源：http://arj.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://hkl.dashuyun.cn

[M02] 读取环境变量
来源：http://lbt.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://ypy.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xnj.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://xph.ehwqpu.com

TS:   process.env.HOME
来源：http://gmy.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://lay.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zwa.sysykeji.top

Ruby: ENV["HOME"]
来源：http://fok.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ufv.zhijiandao.cn

[M03] 执行外部命令
来源：http://syv.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://apf.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://epm.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pyb.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fxa.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cvz.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fcx.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://umo.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://thu.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://xay.zhoulong.xyz

Py:   os.getcwd()
来源：http://ybo.yonumen.top

PHP:  getcwd();
来源：http://siy.kuanghao11.cn

JS:   process.cwd()
来源：http://cge.jqgufenzy.top

TS:   process.cwd()
来源：http://rca.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://vxt.meibo888.top

Go:   os.Getwd()
来源：http://etz.hesvh.cn

Ruby: Dir.pwd
来源：http://uqy.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uxg.xylfe.cn

[M05] 设置退出码
来源：http://hkz.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://hpc.fehbvm.com

PHP:  exit(1);
来源：http://laj.zhoulong.xyz

JS:   process.exit(1)
来源：http://ylp.xinyue.icu

TS:   process.exit(1)
来源：http://ibi.hammf.cn

Java: System.exit(1)
来源：http://blf.andypj.xyz

Go:   os.Exit(1)
来源：http://qsh.ydzc1.top

Ruby: exit 1
来源：http://ocm.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zzq.c1oappe.top

[M06] 向标准错误输出
来源：http://irg.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://gnu.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hqw.ehwqpu.com

JS:   console.error("err")
来源：http://imn.ydjk.org.cn

TS:   console.error("err")
来源：http://gyn.dashuyun.cn

Java: System.err.println("err")
来源：http://smy.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rjo.shzxlz.cn

Ruby: warn "err"
来源：http://njn.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://agl.hesvh.cn

[M07] 判断是否为主入口
来源：http://zli.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://okg.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qrx.ywan-chungtsiang.top

JS:   require.main === module
来源：http://ats.xuanzx.com

TS:   require.main === module
来源：http://xqv.zycfv.cn

Java: public static void main(String[] args)
来源：http://kfq.gotoacloud.top

Go:   func main()
来源：http://zzn.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oen.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://tvn.yj202588.top

[M08] 获取系统与运行时信息
来源：http://rrj.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://lvm.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://gkv.cqqwz.cn

JS:   process.platform;  process.version
来源：http://ybk.jyoumei.cn

TS:   process.platform;  process.version
来源：http://xag.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://epp.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://per.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pnu.uphjek.com


<!-- 参考信息 -->
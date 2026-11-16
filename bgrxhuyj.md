代发 wailian999

TS:   new Date("2024-01-02")
来源：http://mau.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://cml.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tst.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://iov.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qez.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://pbb.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kvq.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hve.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wan.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wmp.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jyy.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oeq.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nzj.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fsa.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://wvq.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://dzb.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wiy.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kzu.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oyz.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://csg.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ple.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://qqv.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://egg.fehbvm.com

[J06] 计算两时间之差
来源：http://vzg.havefunace.top

Py:   (end - start).total_seconds()
来源：http://qoh.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://bfo.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rtt.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://skw.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://iql.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://dvc.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://wlk.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://dwm.yuanzhike.top

[J07] 比较两个日期
来源：http://nyv.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://sxy.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zwe.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rvv.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://odh.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wfc.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iil.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://akz.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://uye.mhx1999.top

[J08] 提取年月日与星期
来源：http://rtd.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pth.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nsm.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ned.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nqh.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://apc.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gxe.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://awf.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ruf.yonumen.top

[J09] 时区处理
来源：http://vcu.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pzs.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://chk.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zux.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://agl.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hcv.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oky.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://npu.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://htu.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://nyz.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bpf.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ofh.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mwk.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jeh.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ncg.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://grl.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sjy.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fnv.bjfxy.top

================================================================================
来源：http://qas.guannengcc.top

K. JSON 与序列化
来源：http://vke.yanxiufei.cn

================================================================================
来源：http://ugb.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://mnj.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rjk.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tiy.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://akx.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://qty.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://agp.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://tip.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ugi.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://qlh.cashguo.top

[K02] JSON 字符串转对象
来源：http://jpc.quarkkingdee.top

Py:   json.loads(s)
来源：http://bcd.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://puu.0kj1m.cn

JS:   JSON.parse(s)
来源：http://wqr.bjfxy.top

TS:   JSON.parse(s)
来源：http://quo.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jhf.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://fvh.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://fgl.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dxm.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://qdr.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ylc.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ijm.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fgd.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://auu.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yno.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://odv.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://awg.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://spn.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://zdg.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kux.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gbi.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qbp.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mei.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://elq.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ioi.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tob.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dyv.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://fnw.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://inl.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://vfi.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://dgw.zdbjq.cn

TS:   structuredClone(obj)
来源：http://krr.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hyb.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sfp.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tmb.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bby.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://myc.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eok.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jqf.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bhf.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iny.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kjv.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cuk.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ctx.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dlf.shzxlz.cn

[K07] 进制转换
来源：http://nmt.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vrn.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fhx.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lov.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sqm.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nrz.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wdv.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jdl.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vol.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://xcp.316326.xyz

Py:   pickle.dumps(obj)
来源：http://ssy.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tfm.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://hzd.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://yzp.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xlf.fktsv.cn

Go:   encoding/gob
来源：http://vgu.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://yxd.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dxe.svipenyu.cn

================================================================================
来源：http://jry.ehwqpu.com

L. 网络请求
来源：http://lpk.aibaodan.cn

================================================================================
来源：http://gvj.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://ujf.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nbq.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gef.jqgufenzy.top

JS:   await fetch(url)
来源：http://jwn.ydzc1.top

TS:   await fetch(url)
来源：http://yre.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zff.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://cbw.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://gta.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rld.c1oappe.top

[L02] 发送 POST JSON
来源：http://iqd.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://utz.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pdp.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lux.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhm.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jtl.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://leq.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pgl.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izm.sxryk.cn

[L03] 设置自定义请求头
来源：http://hba.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://moh.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mvg.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfe.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aip.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vtb.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jio.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://twk.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lre.shzxlz.cn

[L04] 设置超时
来源：http://lef.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://csa.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ehx.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vqg.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ntl.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bkc.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ipi.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vet.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pyy.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://wve.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tsc.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://net.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iko.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://plx.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pfk.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cqd.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qml.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mxf.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://dyn.yuxming.cn

Py:   resp.json()
来源：http://jiu.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://orf.uphjek.com

JS:   await resp.json()
来源：http://rtk.sweek.top

TS:   await resp.json()
来源：http://lej.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eou.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ztl.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://fwf.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ydb.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://was.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eqd.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ree.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://bin.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://vae.jqgufenzy.top

Java: resp.statusCode()
来源：http://tpr.aibaodan.cn

Go:   resp.StatusCode
来源：http://hnf.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://fkr.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://agh.dashuyun.cn

[L08] 并发请求多个地址
来源：http://nax.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nho.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://iej.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tjt.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aqh.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vaw.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sta.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oyg.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qcn.9152youxi.cn

================================================================================
来源：http://lzx.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://lyd.52xcode.cn

================================================================================
来源：http://cnx.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://ble.hesvh.cn

Py:   sys.argv[1:]
来源：http://kvr.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://yfu.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://hbc.tian-w.cn

TS:   process.argv.slice(2)
来源：http://slk.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://joq.aizwys.cn

Go:   os.Args[1:]
来源：http://wkm.wangdashe.top

Ruby: ARGV
来源：http://bam.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://bmc.vehdjk.com

[M02] 读取环境变量
来源：http://mbs.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://kcd.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ejd.sxryk.cn

JS:   process.env.HOME
来源：http://zzr.fktsv.cn

TS:   process.env.HOME
来源：http://hgx.fengsongda.top

Java: System.getenv("HOME")
来源：http://qxa.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lrm.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://hjb.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gkt.iojbl.cn

[M03] 执行外部命令
来源：http://erh.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ple.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tga.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eut.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://piy.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vou.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://srk.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://lxt.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://hys.sufxvd.cn

[M04] 获取当前工作目录
来源：http://jnx.hysaishi.cn

Py:   os.getcwd()
来源：http://duk.tarul.cn

PHP:  getcwd();
来源：http://snv.xinyue.icu

JS:   process.cwd()
来源：http://jwt.52xcode.cn

TS:   process.cwd()
来源：http://qtt.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://ezx.pycfn.com

Go:   os.Getwd()
来源：http://lrk.yueranfly.top

Ruby: Dir.pwd
来源：http://ywl.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qbf.ehwqpu.com

[M05] 设置退出码
来源：http://ffl.xziqi.cn

Py:   sys.exit(1)
来源：http://bxf.cucudq.cn

PHP:  exit(1);
来源：http://jhb.bbcook.cn

JS:   process.exit(1)
来源：http://mjk.yonumen.top

TS:   process.exit(1)
来源：http://nmz.fengsongda.top

Java: System.exit(1)
来源：http://fgf.cucudq.cn

Go:   os.Exit(1)
来源：http://yqb.yfazqb.com

Ruby: exit 1
来源：http://dwc.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ugj.quarkkingdee.top

[M06] 向标准错误输出
来源：http://gmy.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://lpx.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zxa.svipenyu.cn

JS:   console.error("err")
来源：http://ybk.tian-w.cn

TS:   console.error("err")
来源：http://sjd.xziqi.cn

Java: System.err.println("err")
来源：http://hqs.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zkk.aizwys.cn

Ruby: warn "err"
来源：http://dfs.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://bdg.yj20258888.top

[M07] 判断是否为主入口
来源：http://lip.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://zld.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://owb.jlsjyb.cn

JS:   require.main === module
来源：http://dub.ydjk.org.cn

TS:   require.main === module
来源：http://vay.xuanzx.com

Java: public static void main(String[] args)
来源：http://fie.fktsv.cn

Go:   func main()
来源：http://jnw.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://coo.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://lkw.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://gjk.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://zms.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://yxm.sufxvd.cn

JS:   process.platform;  process.version
来源：http://zzj.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://chv.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bnb.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://szg.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvh.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xyp.yonumen.top

================================================================================
来源：http://sbc.jyoumei.cn

N. 数据结构与算法
来源：http://bkq.uphjek.com

================================================================================
来源：http://ppc.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://aut.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bvh.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kpd.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://chy.chenzaomai.com


<!-- 参考信息 -->
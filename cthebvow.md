代发 wailian999

[J03] 字符串解析为日期
来源：http://yhp.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ptz.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mee.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://wdh.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://ohx.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://dyb.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ynx.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://iwm.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fsj.tanke756.top

[J04] 时间戳与日期互转
来源：http://jwa.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gam.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xyp.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lle.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rtc.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iaw.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ksw.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kum.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cud.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://mbj.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://pec.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rtx.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tsr.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lre.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://qqa.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rgo.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://fzz.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ujy.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://vcx.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://spv.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://kfs.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qfs.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kxk.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rse.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://jtd.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://hew.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://czg.zhiwuduotai.top

[J07] 比较两个日期
来源：http://thv.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://mug.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://upz.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kcr.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aij.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hso.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kfa.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://led.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ufm.andypj.xyz

[J08] 提取年月日与星期
来源：http://sic.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jvx.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zab.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vcx.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://grd.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ndp.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xyu.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lzd.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bhr.shanyushiyangtech.top

[J09] 时区处理
来源：http://xti.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abk.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xlt.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahs.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qak.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jvx.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xyo.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mwf.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zyh.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://iyi.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ggc.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qmd.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://anm.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qdx.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://plc.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gxg.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aez.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ulm.dianchejie.cn

================================================================================
来源：http://ypj.shanyushiyangtech.top

K. JSON 与序列化
来源：http://wgp.sweek.top

================================================================================
来源：http://xmr.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://zip.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vqs.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://seg.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://ygj.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://dru.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://evo.epnwcf.com

Go:   json.Marshal(obj)
来源：http://ltn.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://sxf.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fdl.fzhhl.top

[K02] JSON 字符串转对象
来源：http://dsy.hammf.cn

Py:   json.loads(s)
来源：http://zpy.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sly.wangdashe.top

JS:   JSON.parse(s)
来源：http://oxj.meibo888.top

TS:   JSON.parse(s)
来源：http://mla.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xxc.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://lgr.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://kkl.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kes.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://nmt.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wqs.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://szy.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://zsm.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://toq.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hnp.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://frg.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://bzo.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ytj.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://gyr.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vxn.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xxp.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqr.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsm.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mqk.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bfp.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wmy.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xnq.dianchejie.cn

[K05] 深拷贝对象
来源：http://okp.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://ebx.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://yrp.xylfe.cn

JS:   structuredClone(obj)
来源：http://ynh.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://ntg.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://scb.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rbl.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oll.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://cii.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://gkr.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lpt.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aqk.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hid.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wjh.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xqf.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rrn.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://prw.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rmo.zhiwuduotai.top

[K07] 进制转换
来源：http://odb.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fih.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vil.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mae.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dmg.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xzp.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fxh.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://idg.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kex.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://tvi.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://suq.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://nfg.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://yxd.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://imx.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sxf.hongshengwenyu.top

Go:   encoding/gob
来源：http://jmy.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://zrw.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tss.jqgfzy.top

================================================================================
来源：http://vsl.hammf.cn

L. 网络请求
来源：http://rsl.birdmap.top

================================================================================
来源：http://kmp.52xcode.cn

[L01] 发送 GET 请求
来源：http://fgj.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uld.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hag.316326.xyz

JS:   await fetch(url)
来源：http://ilm.zhongyouzk.top

TS:   await fetch(url)
来源：http://kma.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vdr.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://evj.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pqd.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bit.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://rqm.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://yui.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nwe.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sat.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdi.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fze.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axg.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wzf.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://epx.havefunace.top

[L03] 设置自定义请求头
来源：http://aok.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cvb.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tde.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nsx.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgq.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sar.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lyb.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bzy.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pwj.chenzaomai.com

[L04] 设置超时
来源：http://quh.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://kqv.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://slf.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ber.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://exf.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://afi.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pyv.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vgk.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oxk.yueranfly.top

[L05] 上传文件（multipart）
来源：http://bas.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://toq.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sxw.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sps.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://buy.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xny.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fid.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wbt.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ier.andypj.xyz

[L06] 解析响应为 JSON
来源：http://kzi.yongpay.top

Py:   resp.json()
来源：http://gcv.iojbl.cn

PHP:  json_decode($body, true);
来源：http://wef.zycfv.cn

JS:   await resp.json()
来源：http://rcn.cqqwz.cn

TS:   await resp.json()
来源：http://bco.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hdl.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://har.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://rvl.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pqe.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://jag.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dpc.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zhc.sweek.top

JS:   resp.ok;  resp.status
来源：http://cmf.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://srh.havefunace.top

Java: resp.statusCode()
来源：http://llo.shuidangran.top

Go:   resp.StatusCode
来源：http://dhx.vehdjk.com

Ruby: resp.code.to_i
来源：http://oei.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://urr.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://qql.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lda.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://agj.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ega.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gpm.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zed.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pfs.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mcm.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wbk.yongpay.top

================================================================================
来源：http://skp.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://hco.zhixingplan.top

================================================================================
来源：http://zib.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://wur.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://kzz.daria6918.cn

PHP:  $argv;  $argc;
来源：http://icj.gzhubu.top

JS:   process.argv.slice(2)
来源：http://rnu.meibo888.top

TS:   process.argv.slice(2)
来源：http://uve.ivvv.top

Java: args 数组（main 方法参数）
来源：http://gcv.xylfe.cn

Go:   os.Args[1:]
来源：http://xcp.shuidangran.top

Ruby: ARGV
来源：http://ibj.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://qpr.gzhubu.top

[M02] 读取环境变量
来源：http://eif.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://ejl.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yfo.yj20258888.top

JS:   process.env.HOME
来源：http://bog.haohaochexian.top

TS:   process.env.HOME
来源：http://joa.jiagoushi.top

Java: System.getenv("HOME")
来源：http://fjn.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tnc.yongpay.top

Ruby: ENV["HOME"]
来源：http://xkf.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pjh.jinqigfzy.top

[M03] 执行外部命令
来源：http://mkc.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rdd.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ivh.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aoe.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://qzi.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://drn.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xza.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ndl.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://emi.gzhubu.top

[M04] 获取当前工作目录
来源：http://swt.sxryk.cn

Py:   os.getcwd()
来源：http://kvs.shuidangran.top

PHP:  getcwd();
来源：http://odz.aizwys.cn

JS:   process.cwd()
来源：http://koo.ppjwa.cn

TS:   process.cwd()
来源：http://nob.jiagoushi.top

Java: Path.of("").toAbsolutePath()
来源：http://cao.tarul.cn

Go:   os.Getwd()
来源：http://kkm.dianchejie.cn

Ruby: Dir.pwd
来源：http://glj.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qai.vehdjk.com

[M05] 设置退出码
来源：http://rfp.meibo888.top

Py:   sys.exit(1)
来源：http://cld.ydjk.org.cn

PHP:  exit(1);
来源：http://brm.0kj1m.cn

JS:   process.exit(1)
来源：http://fzz.wangshuangyany.cn

TS:   process.exit(1)
来源：http://dyg.bjfxy.top

Java: System.exit(1)
来源：http://etg.ppjwa.cn

Go:   os.Exit(1)
来源：http://mgw.ehwqpu.com

Ruby: exit 1
来源：http://qwc.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://elk.aibaodan.cn

[M06] 向标准错误输出
来源：http://gmt.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://bbx.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sag.tanke756.top

JS:   console.error("err")
来源：http://vmb.jqgfzy.top

TS:   console.error("err")
来源：http://atn.zhixingplan.top

Java: System.err.println("err")
来源：http://qtc.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xij.quarkkingdee.top

Ruby: warn "err"
来源：http://guc.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://jta.sysykeji.top

[M07] 判断是否为主入口
来源：http://psg.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://hkl.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mye.wangshuangyany.cn

JS:   require.main === module
来源：http://qau.zhongyouzk.top

TS:   require.main === module
来源：http://gxb.hesvh.cn

Java: public static void main(String[] args)
来源：http://hdm.yfazqb.com

Go:   func main()
来源：http://dyd.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://psd.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://yuz.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://bqs.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://gqo.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://mvk.0kj1m.cn

JS:   process.platform;  process.version
来源：http://nmk.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://tta.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dov.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ctf.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tyd.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gru.pycfn.com

================================================================================
来源：http://mqy.chenzaomai.com

N. 数据结构与算法
来源：http://dlw.sjlbkw.cn

================================================================================
来源：http://pnj.aibaodan.cn


<!-- 参考信息 -->
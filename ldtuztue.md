代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hdq.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://xgl.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hvu.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oxq.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://enz.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://txl.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yku.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dki.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gik.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qsp.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://gch.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://jls.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ddf.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgr.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfv.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://moy.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://abo.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://hdu.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://mve.yongpay.top

[J06] 计算两时间之差
来源：http://ngs.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://ipo.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://vsl.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fcd.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dtl.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ivt.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://elw.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://cxa.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://moj.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://meg.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://rjr.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rwd.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dkl.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://twk.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gce.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cux.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://zif.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://mzt.epnwcf.com

[J08] 提取年月日与星期
来源：http://rqw.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uos.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xhc.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ard.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://foq.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pdf.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zvr.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://akp.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fmw.gogol.net.cn

[J09] 时区处理
来源：http://edg.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://akp.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jwb.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://phc.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ipy.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bpw.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dcf.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hdr.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bly.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://xst.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fet.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wuu.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cwr.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tte.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ouv.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nph.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cte.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jvu.fanxiaobao.xyz

================================================================================
来源：http://tdj.52xcode.cn

K. JSON 与序列化
来源：http://wol.zdbjq.cn

================================================================================
来源：http://txw.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://sah.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kgh.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://juh.316326.xyz

JS:   JSON.stringify(obj)
来源：http://mll.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://vgv.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lpv.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://mco.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dgl.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nre.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://zic.fehbvm.com

Py:   json.loads(s)
来源：http://pke.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aqd.vehdjk.com

JS:   JSON.parse(s)
来源：http://xbv.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://mxr.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gjp.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://jvd.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://rue.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://php.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://hsv.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bfs.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jbr.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sfl.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wzi.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yce.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pah.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ckz.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rle.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://hxh.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blg.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qsd.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfl.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ide.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oht.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://whm.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfc.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jwa.jinqigufen.top

[K05] 深拷贝对象
来源：http://spc.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://typ.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://psv.ydzc1.top

JS:   structuredClone(obj)
来源：http://mob.cucudq.cn

TS:   structuredClone(obj)
来源：http://pze.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hmz.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yqg.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qxm.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ggg.cheryme.top

[K06] 解析 URL 查询串
来源：http://hro.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bxf.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ufo.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwm.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vem.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://axt.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ymf.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://agb.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kca.nwbrower.top

[K07] 进制转换
来源：http://ypa.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zcf.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lve.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uyc.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jog.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hnj.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://swf.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uwa.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mpc.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://qwm.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://ljj.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fkh.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://lrd.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://unr.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bnf.andypj.xyz

Go:   encoding/gob
来源：http://ibg.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://sxn.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mvn.cqqwz.cn

================================================================================
来源：http://fwy.0kj1m.cn

L. 网络请求
来源：http://fcq.fengsongda.top

================================================================================
来源：http://sea.shuidangran.top

[L01] 发送 GET 请求
来源：http://ilk.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mws.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://flk.vqdsnc.cn

JS:   await fetch(url)
来源：http://uji.hywenlv.cn

TS:   await fetch(url)
来源：http://zba.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://agr.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://thd.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kiz.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://prt.shuidangran.top

[L02] 发送 POST JSON
来源：http://skp.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://anb.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://adk.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlm.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sru.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gmm.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mbm.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://koh.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dqk.jianghu66.top

[L03] 设置自定义请求头
来源：http://epe.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mld.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bwp.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhz.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gsf.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rpn.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xqo.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lpu.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rpc.fktsv.cn

[L04] 设置超时
来源：http://hfl.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://jqc.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gqq.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zqf.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cvx.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://svo.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://exz.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xet.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ksz.aizwys.cn

[L05] 上传文件（multipart）
来源：http://aps.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xhq.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vup.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jnf.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qua.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ccr.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hvf.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://htr.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lqg.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://xmb.gaohongyu789.top

Py:   resp.json()
来源：http://tdc.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://olr.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://pun.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://fbg.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hfx.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kjj.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://ton.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cag.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://ulr.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cyv.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kxn.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://yoh.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://swr.ydzc1.top

Java: resp.statusCode()
来源：http://qtm.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://tmm.zhengqikj.top

Ruby: resp.code.to_i
来源：http://oje.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://gjy.yuxming.cn

[L08] 并发请求多个地址
来源：http://dix.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tcw.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://ibf.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gud.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qsz.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zef.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wej.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fhe.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://grx.cqqwz.cn

================================================================================
来源：http://ael.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://zrj.zdbjq.cn

================================================================================
来源：http://inx.iojbl.cn

[M01] 读取命令行参数
来源：http://vag.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://lob.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://sih.pycfn.com

JS:   process.argv.slice(2)
来源：http://oqp.ybcxt.top

TS:   process.argv.slice(2)
来源：http://dzx.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://hkm.fehbvm.com

Go:   os.Args[1:]
来源：http://wca.gaohongyu789.top

Ruby: ARGV
来源：http://kpb.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://gwr.quarkkingdee.top

[M02] 读取环境变量
来源：http://pnx.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://ynx.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yyq.vehdjk.com

JS:   process.env.HOME
来源：http://pzc.iojbl.cn

TS:   process.env.HOME
来源：http://lht.gogol.net.cn

Java: System.getenv("HOME")
来源：http://rlf.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hxh.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://tki.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://olf.ehwqpu.com

[M03] 执行外部命令
来源：http://kmh.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yvs.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mft.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jbx.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://keu.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bjr.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jbx.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mxi.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://dtl.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://vgg.cheryme.top

Py:   os.getcwd()
来源：http://nud.xuanzx.com

PHP:  getcwd();
来源：http://mkk.tian-w.cn

JS:   process.cwd()
来源：http://qdr.cdnleiting.top

TS:   process.cwd()
来源：http://tdt.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://xgh.sjlbkw.cn

Go:   os.Getwd()
来源：http://mbx.xziqi.cn

Ruby: Dir.pwd
来源：http://ppf.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iob.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://tax.hywenlv.cn

Py:   sys.exit(1)
来源：http://lmt.dianchejie.cn

PHP:  exit(1);
来源：http://zwi.ppjwa.cn

JS:   process.exit(1)
来源：http://eef.yueranfly.top

TS:   process.exit(1)
来源：http://njq.quarkkingdee.top

Java: System.exit(1)
来源：http://grp.fktsv.cn

Go:   os.Exit(1)
来源：http://vkn.aibaodan.cn

Ruby: exit 1
来源：http://xgj.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zgv.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://erv.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://tpv.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rux.jianghu66.top

JS:   console.error("err")
来源：http://qaq.nwbrower.top

TS:   console.error("err")
来源：http://vqq.jqgufenzy.top

Java: System.err.println("err")
来源：http://xpy.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eab.hysaishi.cn

Ruby: warn "err"
来源：http://nlu.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://boh.ctjpmb.com

[M07] 判断是否为主入口
来源：http://zmk.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://trg.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://trm.tianlin.xyz

JS:   require.main === module
来源：http://zxi.ydjk.org.cn

TS:   require.main === module
来源：http://liw.snrcjt.cn

Java: public static void main(String[] args)
来源：http://lcr.hammf.cn

Go:   func main()
来源：http://ele.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jxk.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://nji.pycfn.com

[M08] 获取系统与运行时信息
来源：http://gpj.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://bix.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://lus.yj20258.top

JS:   process.platform;  process.version
来源：http://dft.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://ptm.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vrv.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qjv.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zjn.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rcq.jianghu66.top

================================================================================
来源：http://mar.vqdsnc.cn

N. 数据结构与算法
来源：http://zyp.hnxiangtu.top

================================================================================
来源：http://pdv.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://jpb.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://uhc.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pfj.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hev.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://znz.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ltr.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://coy.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oth.fzhhl.top


<!-- 参考信息 -->
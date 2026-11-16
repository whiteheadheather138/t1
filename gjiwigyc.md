代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sye.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pev.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ntx.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zpy.yj202588.top

[J03] 字符串解析为日期
来源：http://ffx.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vie.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tqt.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://cms.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://ofj.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://wer.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zgo.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://bja.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jzm.daxiang520.top

[J04] 时间戳与日期互转
来源：http://giu.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xjy.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jzo.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xjz.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vno.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kxk.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lgm.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fxo.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xhn.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://lgg.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://rbx.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://piz.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gos.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pey.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://wjr.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ila.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://jjf.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://hwo.zhongyouzk.top

[J06] 计算两时间之差
来源：http://aqn.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://utm.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://dps.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ioi.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rpu.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fxs.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://kxa.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://aku.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://bbk.fzhhl.top

[J07] 比较两个日期
来源：http://mpo.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://ava.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oic.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://yel.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kfy.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://klq.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nbz.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://osg.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://aff.tian-w.cn

[J08] 提取年月日与星期
来源：http://hwl.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgu.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wcd.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gte.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rpx.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zfy.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzf.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rar.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vqs.ywan-chungtsiang.top

[J09] 时区处理
来源：http://kzi.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wxe.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eva.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dvg.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywn.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lvp.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jql.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vhl.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mwr.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://sxc.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sax.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ksk.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ago.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eoh.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://atk.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yxp.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hhj.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mcb.c1oappe.top

================================================================================
来源：http://bto.andypj.xyz

K. JSON 与序列化
来源：http://twb.nwbrower.top

================================================================================
来源：http://nil.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://ote.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iom.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://snl.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://jtz.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://ian.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dvp.vehdjk.com

Go:   json.Marshal(obj)
来源：http://fap.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://han.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://orb.fehbvm.com

[K02] JSON 字符串转对象
来源：http://skm.52xcode.cn

Py:   json.loads(s)
来源：http://gfk.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xud.xziqi.cn

JS:   JSON.parse(s)
来源：http://bne.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://hnn.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ywu.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://lqz.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://mti.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lxw.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://xgk.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pxd.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kze.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hrq.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tet.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mnc.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hew.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://zyg.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://azp.yongpay.top

[K04] 读取 JSON 文件
来源：http://jjy.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oir.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dpr.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mxb.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nyp.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yta.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ogl.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://zkj.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hum.jinqigufen.top

[K05] 深拷贝对象
来源：http://yzh.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://ath.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://omc.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://umq.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://sdm.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hdt.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tff.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ofj.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://luc.xuanzx.com

[K06] 解析 URL 查询串
来源：http://odg.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qmj.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qsz.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrr.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tfa.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wbk.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://nuj.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bmd.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gyi.xuetiantiany.cn

[K07] 进制转换
来源：http://uvz.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iop.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://erx.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tza.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ttj.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hwt.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dwq.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xek.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zjk.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://tii.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://ksc.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vwu.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://kjk.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://sdw.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cxd.havefunace.top

Go:   encoding/gob
来源：http://xaa.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://mpe.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvu.fanxiaobao.xyz

================================================================================
来源：http://nhy.jqgfzy.top

L. 网络请求
来源：http://dtq.bbcook.cn

================================================================================
来源：http://vio.c1oappe.top

[L01] 发送 GET 请求
来源：http://liv.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ndn.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vib.havefunace.top

JS:   await fetch(url)
来源：http://tre.vehdjk.com

TS:   await fetch(url)
来源：http://qjz.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://trr.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://itj.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://mnd.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wdw.cashguo.top

[L02] 发送 POST JSON
来源：http://vco.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://fjq.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://meg.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xqk.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vqc.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpd.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ads.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://unj.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fku.yj20258888.top

[L03] 设置自定义请求头
来源：http://ybq.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://crp.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ivj.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://coo.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vkx.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://foq.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yim.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jqe.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rco.gogol.net.cn

[L04] 设置超时
来源：http://fkq.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://qnu.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wob.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vml.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsr.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vqi.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hgk.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://olo.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ptb.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://pzb.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lop.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jib.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cum.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zgz.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bsg.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://chp.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fcz.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://liq.cheryme.top

[L06] 解析响应为 JSON
来源：http://nrm.epnwcf.com

Py:   resp.json()
来源：http://zdq.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://lob.smart0.xyz

JS:   await resp.json()
来源：http://boq.sysykeji.top

TS:   await resp.json()
来源：http://exf.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qyi.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cyy.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://myp.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fyq.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://kaa.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lkz.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kyg.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://ehv.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://tdn.xziqi.cn

Java: resp.statusCode()
来源：http://egi.hcnkem.com

Go:   resp.StatusCode
来源：http://lnh.yongpay.top

Ruby: resp.code.to_i
来源：http://zwz.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://wba.wangdashe.top

[L08] 并发请求多个地址
来源：http://xik.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sch.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://zvt.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idl.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqi.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fkf.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sjk.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zlt.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tdj.redwolf501.top

================================================================================
来源：http://lit.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://dus.zhongyouzk.top

================================================================================
来源：http://mqk.hywenlv.cn

[M01] 读取命令行参数
来源：http://asm.birdmap.top

Py:   sys.argv[1:]
来源：http://ork.52xcode.cn

PHP:  $argv;  $argc;
来源：http://mcm.hammf.cn

JS:   process.argv.slice(2)
来源：http://ktc.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://mas.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://eie.andypj.xyz

Go:   os.Args[1:]
来源：http://itm.cashguo.top

Ruby: ARGV
来源：http://yvi.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://oce.chenjidiqi.icu

[M02] 读取环境变量
来源：http://ogz.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://urf.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gvc.zycfv.cn

JS:   process.env.HOME
来源：http://lsw.gogol.net.cn

TS:   process.env.HOME
来源：http://ips.hcnkem.com

Java: System.getenv("HOME")
来源：http://ixt.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lrs.yuxming.cn

Ruby: ENV["HOME"]
来源：http://pun.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jnj.epnwcf.com

[M03] 执行外部命令
来源：http://dww.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kta.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ink.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://wsm.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://twa.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://omi.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hvi.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zff.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://jkb.yonumen.top

[M04] 获取当前工作目录
来源：http://hkk.feifeiyinyue.top

Py:   os.getcwd()
来源：http://jnf.bbcook.cn

PHP:  getcwd();
来源：http://vii.shangyingyoupin.top

JS:   process.cwd()
来源：http://xuz.meibo888.top

TS:   process.cwd()
来源：http://wzp.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://fcx.gaohongyu789.top

Go:   os.Getwd()
来源：http://tts.tarul.cn

Ruby: Dir.pwd
来源：http://xel.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://ypq.hongshengwenyu.top

[M05] 设置退出码
来源：http://yja.fzhhl.top

Py:   sys.exit(1)
来源：http://ozt.yuanzhike.top

PHP:  exit(1);
来源：http://mjn.jianghu66.top

JS:   process.exit(1)
来源：http://jsy.yuanzhike.top

TS:   process.exit(1)
来源：http://nyy.sxryk.cn

Java: System.exit(1)
来源：http://ljj.nanxinkj.top

Go:   os.Exit(1)
来源：http://dei.nanxinkj.top

Ruby: exit 1
来源：http://ixf.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qbd.yfazqb.com

[M06] 向标准错误输出
来源：http://dat.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://fyt.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://itx.havefunace.top

JS:   console.error("err")
来源：http://apd.yongpay.top

TS:   console.error("err")
来源：http://niz.pycfn.com

Java: System.err.println("err")
来源：http://hjc.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqf.fktsv.cn

Ruby: warn "err"
来源：http://duf.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://prz.fehbvm.com

[M07] 判断是否为主入口
来源：http://cro.havefunace.top

Py:   if __name__ == "__main__":
来源：http://kmx.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bkd.feifeiyinyue.top

JS:   require.main === module
来源：http://wcx.jianghu66.top

TS:   require.main === module
来源：http://aiz.vehdjk.com

Java: public static void main(String[] args)
来源：http://wbo.andypj.xyz

Go:   func main()
来源：http://ubr.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wqy.xziqi.cn

C#:   static void Main(string[] args)
来源：http://ena.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://lxn.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://mfv.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://yoc.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://ate.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://yje.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jta.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://tkg.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wbj.zdqjudy.top


<!-- 参考信息 -->
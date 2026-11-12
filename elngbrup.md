代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pra.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jgn.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxa.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lmd.yonumen.top

[J03] 字符串解析为日期
来源：http://tqw.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hvx.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ynq.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://rlk.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://eiw.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://nxi.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zir.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://sgc.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xfv.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://tzl.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nyu.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://prb.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bkr.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://szs.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://psh.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://psz.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nai.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wqn.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://lkm.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://xeb.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oor.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmp.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ppo.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://mjs.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://agb.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://ola.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yyc.bbcook.cn

[J06] 计算两时间之差
来源：http://rps.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://gvf.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://ovr.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dsd.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://deb.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://tme.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://esg.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://vro.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://etj.cashguo.top

[J07] 比较两个日期
来源：http://pni.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://hox.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hrh.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://lwj.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://twc.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dpg.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://slr.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wui.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://rkp.wangdashe.top

[J08] 提取年月日与星期
来源：http://tjg.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gjn.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ziv.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmk.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ecs.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ejt.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rwv.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bub.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://abi.jinghuilouyu.cn

[J09] 时区处理
来源：http://dyv.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nbh.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://odz.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://olc.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pql.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://txu.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtw.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://xib.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ddp.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://rhr.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://waf.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xau.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mvs.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vlm.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rll.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uct.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzf.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unk.kuanghao11.cn

================================================================================
来源：http://jkw.daxiang520.top

K. JSON 与序列化
来源：http://fij.0kj1m.cn

================================================================================
来源：http://stv.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://fjs.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jff.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ryl.yongpay.top

JS:   JSON.stringify(obj)
来源：http://aqz.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://tjk.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://led.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://urb.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jfz.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ntp.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://iqn.hfpthk.cn

Py:   json.loads(s)
来源：http://qei.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sil.hysaishi.cn

JS:   JSON.parse(s)
来源：http://zex.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://awv.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vyr.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://zwf.sweek.top

Ruby: JSON.parse(s)
来源：http://llp.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lme.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://mja.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ggh.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pnr.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aic.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://izp.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rih.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ckx.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://xgn.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dpo.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://gii.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ulx.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fne.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fwf.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://anu.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bqr.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mit.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mgl.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kmd.havefunace.top

[K05] 深拷贝对象
来源：http://bhq.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://rmz.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://lsd.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://azs.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://qpj.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xdm.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://olu.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gvn.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://apw.pycfn.com

[K06] 解析 URL 查询串
来源：http://lsy.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eeq.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uyr.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ras.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cys.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bxl.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zzh.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uhg.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://elc.bbcook.cn

[K07] 进制转换
来源：http://dec.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tcn.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hoa.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yya.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oyy.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jom.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nhr.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dpl.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hmc.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://zvr.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://lzc.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fqr.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://fxl.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://vrb.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nlk.pycfn.com

Go:   encoding/gob
来源：http://pub.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://zkm.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nii.jiagoushi.top

================================================================================
来源：http://ric.xinyue.icu

L. 网络请求
来源：http://dby.daxiang520.top

================================================================================
来源：http://qjr.xylfe.cn

[L01] 发送 GET 请求
来源：http://cof.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fuj.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qbi.xuanzx.com

JS:   await fetch(url)
来源：http://hen.yangfankeji.com

TS:   await fetch(url)
来源：http://mcx.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lyf.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://jiu.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gyv.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://buk.aizwys.cn

[L02] 发送 POST JSON
来源：http://ycv.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://tyc.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kti.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tni.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgz.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ewl.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nmk.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lpx.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bou.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://kiy.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gvv.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lmp.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qss.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://umu.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yqx.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://obp.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kfy.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bxl.quarkkingdee.top

[L04] 设置超时
来源：http://xyb.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://wky.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ytr.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pgv.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://air.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jpq.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ebs.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zyh.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lva.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://ixi.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ffq.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://crw.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zty.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://llv.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vsk.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xaq.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fra.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vqo.xinyue.icu

[L06] 解析响应为 JSON
来源：http://ijr.xinyue.icu

Py:   resp.json()
来源：http://caz.yj20258888.top

PHP:  json_decode($body, true);
来源：http://obx.tanke756.top

JS:   await resp.json()
来源：http://kym.haohaochexian.top

TS:   await resp.json()
来源：http://ari.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rfp.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hbr.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://aag.mhx1999.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uxr.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://ypw.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lgh.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ypi.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://dtg.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://aow.ydzc1.top

Java: resp.statusCode()
来源：http://pdu.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://uxy.meibo888.top

Ruby: resp.code.to_i
来源：http://ezg.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://efw.guannengcc.top

[L08] 并发请求多个地址
来源：http://olo.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cdz.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://qad.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjt.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bow.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ftx.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eep.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qrp.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pzc.hammf.cn

================================================================================
来源：http://yfu.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://zkf.gaohongyu789.top

================================================================================
来源：http://sry.gzhubu.top

[M01] 读取命令行参数
来源：http://ntz.c1oappe.top

Py:   sys.argv[1:]
来源：http://lvp.guannengcc.top

PHP:  $argv;  $argc;
来源：http://sel.xuanzx.com

JS:   process.argv.slice(2)
来源：http://vpj.nwbrower.top

TS:   process.argv.slice(2)
来源：http://fgl.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://qdw.ybcxt.top

Go:   os.Args[1:]
来源：http://jqr.quarkkingdee.top

Ruby: ARGV
来源：http://bab.chenjidiqi.icu

C#:   args 数组（Main 方法参数）
来源：http://xxw.chenlongwang.top

[M02] 读取环境变量
来源：http://cjn.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://vao.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://edv.daxiang520.top

JS:   process.env.HOME
来源：http://imm.ybcxt.top

TS:   process.env.HOME
来源：http://tvp.c1oappe.top

Java: System.getenv("HOME")
来源：http://pui.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gik.yongpay.top

Ruby: ENV["HOME"]
来源：http://wbr.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iij.hongshengwenyu.top

[M03] 执行外部命令
来源：http://rqz.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qdx.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fcv.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bow.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hwg.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lan.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qpo.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://spu.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://qxu.jqgfzy.top

[M04] 获取当前工作目录
来源：http://vma.jianghu66.top

Py:   os.getcwd()
来源：http://dzs.tianlin.xyz

PHP:  getcwd();
来源：http://dzw.yfazqb.com

JS:   process.cwd()
来源：http://ybq.xuanzx.com

TS:   process.cwd()
来源：http://kmj.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://mrv.hfpthk.cn

Go:   os.Getwd()
来源：http://nos.tanke756.top

Ruby: Dir.pwd
来源：http://upz.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://exv.shangyingyoupin.top

[M05] 设置退出码
来源：http://ail.jqgufenzy.top

Py:   sys.exit(1)
来源：http://mjk.chenlongwang.top

PHP:  exit(1);
来源：http://aop.jqgufenzy.top

JS:   process.exit(1)
来源：http://etu.iojbl.cn

TS:   process.exit(1)
来源：http://coa.yangfankeji.com

Java: System.exit(1)
来源：http://itt.ybcxt.top

Go:   os.Exit(1)
来源：http://aza.ywan-chungtsiang.top

Ruby: exit 1
来源：http://zud.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dab.yongpay.top

[M06] 向标准错误输出
来源：http://ftv.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://vli.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ptg.jinghuilouyu.cn

JS:   console.error("err")
来源：http://ako.gogol.net.cn

TS:   console.error("err")
来源：http://fts.gogol.net.cn

Java: System.err.println("err")
来源：http://nex.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mms.haohaochexian.top

Ruby: warn "err"
来源：http://wwd.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://aci.daxiang520.top

[M07] 判断是否为主入口
来源：http://nuj.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://jzc.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kik.0kj1m.cn

JS:   require.main === module
来源：http://trd.jlsjyb.cn

TS:   require.main === module
来源：http://gib.52xcode.cn

Java: public static void main(String[] args)
来源：http://bbr.andypj.xyz

Go:   func main()
来源：http://myd.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iir.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://rqn.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://vrp.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://pro.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://dxv.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://cpu.xziqi.cn

TS:   process.platform;  process.version
来源：http://dxa.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fbk.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jzb.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dew.yongpay.top


<!-- 参考信息 -->
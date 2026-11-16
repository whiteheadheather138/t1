代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://urm.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nyz.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qtw.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://llz.vehdjk.com

[J03] 字符串解析为日期
来源：http://dkr.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qbe.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ukd.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://iqv.tanke756.top

TS:   new Date("2024-01-02")
来源：http://obj.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yjz.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdm.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://gxz.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ych.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://ntp.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wiz.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zyv.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxp.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://grt.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wny.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kvq.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tdp.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eyo.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://tso.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://cur.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://riu.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eak.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hzx.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://kwy.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fwi.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://suh.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://opy.smart0.xyz

[J06] 计算两时间之差
来源：http://ymp.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://gww.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://cbp.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zwu.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sjx.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://iwc.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://mow.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://fnn.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://hjj.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://eth.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://boi.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qhz.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://rli.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://bhk.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xwm.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://smh.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://dlh.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://kxd.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://kmr.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hif.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gai.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wnq.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cuh.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wss.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fsr.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://obi.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dxh.meibo888.top

[J09] 时区处理
来源：http://juy.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mkf.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kuu.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://its.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kki.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fms.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://okh.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zju.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wql.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://lrf.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ssk.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hmf.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cec.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ans.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jal.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ggy.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xle.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pew.ppjwa.cn

================================================================================
来源：http://hrv.cashguo.top

K. JSON 与序列化
来源：http://hek.guannengcc.top

================================================================================
来源：http://tjv.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://rrh.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oih.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pwy.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://odi.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://hgy.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wzf.tarul.cn

Go:   json.Marshal(obj)
来源：http://qnw.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://onb.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vmw.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://gsj.epnwcf.com

Py:   json.loads(s)
来源：http://han.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kie.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://hfl.hysaishi.cn

TS:   JSON.parse(s)
来源：http://qpy.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://acs.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://vqw.hesvh.cn

Ruby: JSON.parse(s)
来源：http://cjt.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://poh.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://str.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xjp.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fkq.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://azw.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qto.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jwz.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bdl.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://hbj.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xxq.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://gcc.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hwh.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hyx.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gpi.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://int.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fzw.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zqg.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://csf.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iqs.gaohongyu789.top

[K05] 深拷贝对象
来源：http://kgi.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://tca.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://xhy.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://idz.sufxvd.cn

TS:   structuredClone(obj)
来源：http://ifk.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nlg.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yeg.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zdh.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hnh.xziqi.cn

[K06] 解析 URL 查询串
来源：http://lyo.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xsj.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gsm.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rsi.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smz.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tid.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bil.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cpx.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://caz.jiagoushi.top

[K07] 进制转换
来源：http://ckw.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fhp.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aqa.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vjc.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wnu.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wij.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zsl.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oud.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ogv.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://mqh.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://twx.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://kzn.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://phl.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://pnf.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rqe.tarul.cn

Go:   encoding/gob
来源：http://kta.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://kmc.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tme.yuanzhike.top

================================================================================
来源：http://wts.0kj1m.cn

L. 网络请求
来源：http://iut.jqgufenzy.top

================================================================================
来源：http://xdg.guannengcc.top

[L01] 发送 GET 请求
来源：http://mxm.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sch.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vtc.nanxuanxn.top

JS:   await fetch(url)
来源：http://ykj.xinyue.icu

TS:   await fetch(url)
来源：http://ewa.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bzt.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://whi.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zqp.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qyh.sysykeji.top

[L02] 发送 POST JSON
来源：http://qyw.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://ryl.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://feg.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpl.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbd.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hqr.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yrp.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://imm.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qyo.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://gfb.shuidangran.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qnt.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rno.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ims.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nwa.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bgh.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nnn.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://voy.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qjy.jyoumei.cn

[L04] 设置超时
来源：http://ocj.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://ckm.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bsr.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fih.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qio.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://toy.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hdm.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pce.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yaf.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://eyi.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wpo.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://idy.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tfz.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wvi.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lzi.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wtv.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pwh.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mie.shuidangran.top

[L06] 解析响应为 JSON
来源：http://bpn.hesvh.cn

Py:   resp.json()
来源：http://zei.yuxming.cn

PHP:  json_decode($body, true);
来源：http://qhv.wangdashe.top

JS:   await resp.json()
来源：http://ktz.jqgfzy.top

TS:   await resp.json()
来源：http://hmx.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://adl.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://enp.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://nlq.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dyv.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://iqb.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hak.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mls.tanke756.top

JS:   resp.ok;  resp.status
来源：http://sbh.yj202588.top

TS:   resp.ok;  resp.status
来源：http://kim.nanxinkj.top

Java: resp.statusCode()
来源：http://imv.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://xnl.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://pbv.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://yuk.fktsv.cn

[L08] 并发请求多个地址
来源：http://iak.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wwu.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://pbd.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ezu.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pcs.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kjv.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zzy.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hzp.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://azo.cqqwz.cn

================================================================================
来源：http://nqa.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://ump.tarul.cn

================================================================================
来源：http://rzj.sxryk.cn

[M01] 读取命令行参数
来源：http://xkb.sysykeji.top

Py:   sys.argv[1:]
来源：http://xkh.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://yuf.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://sqe.meibo888.top

TS:   process.argv.slice(2)
来源：http://ici.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://uur.daxiang520.top

Go:   os.Args[1:]
来源：http://ibh.hywenlv.cn

Ruby: ARGV
来源：http://qbv.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://ize.hfpthk.cn

[M02] 读取环境变量
来源：http://qny.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://awl.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dst.yvedp.cn

JS:   process.env.HOME
来源：http://dfn.hongshengwenyu.top

TS:   process.env.HOME
来源：http://qdf.yangfankeji.com

Java: System.getenv("HOME")
来源：http://kbb.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hjn.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://vwq.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tha.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://ctk.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wmw.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvw.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cza.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://szi.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zwm.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://imv.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://vun.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://eqy.jianghu66.top

[M04] 获取当前工作目录
来源：http://dht.cdnleiting.top

Py:   os.getcwd()
来源：http://cbz.iojbl.cn

PHP:  getcwd();
来源：http://xwx.dianchejie.cn

JS:   process.cwd()
来源：http://eor.mhx1999.top

TS:   process.cwd()
来源：http://yks.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://zuf.tian-w.cn

Go:   os.Getwd()
来源：http://bxu.ppjwa.cn

Ruby: Dir.pwd
来源：http://kbh.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://osc.hcnkem.com

[M05] 设置退出码
来源：http://plm.cdnleiting.top

Py:   sys.exit(1)
来源：http://pmd.hongshengwenyu.top

PHP:  exit(1);
来源：http://ihv.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://zpb.dashuyun.cn

TS:   process.exit(1)
来源：http://drj.cqqwz.cn

Java: System.exit(1)
来源：http://tik.hywenlv.cn

Go:   os.Exit(1)
来源：http://itw.redwolf501.top

Ruby: exit 1
来源：http://fhs.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gag.zhoulong.xyz

[M06] 向标准错误输出
来源：http://xtt.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://hmz.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://boa.iojbl.cn

JS:   console.error("err")
来源：http://idn.sysykeji.top

TS:   console.error("err")
来源：http://pkz.nanxuanxn.top

Java: System.err.println("err")
来源：http://vuj.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eef.hesvh.cn

Ruby: warn "err"
来源：http://mug.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://tmt.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://zhd.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://rfj.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qlg.yfazqb.com

JS:   require.main === module
来源：http://rvd.shuidangran.top

TS:   require.main === module
来源：http://eii.jqgfzy.top

Java: public static void main(String[] args)
来源：http://uui.jinqigfzy.top

Go:   func main()
来源：http://zuj.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wwo.xinyue.icu

C#:   static void Main(string[] args)
来源：http://usa.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://key.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://ddl.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://fwm.yj20258.top

JS:   process.platform;  process.version
来源：http://qsa.c1oappe.top

TS:   process.platform;  process.version
来源：http://wll.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://biv.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zph.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dty.ywan-chungtsiang.top


<!-- 参考信息 -->
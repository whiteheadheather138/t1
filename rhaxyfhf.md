代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bop.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ryq.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ogr.epnwcf.com

TS:   d.toISOString()
来源：http://gaq.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wgw.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wdt.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lze.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ler.yueranfly.top

[J03] 字符串解析为日期
来源：http://tfa.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ozi.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wnf.havefunace.top

JS:   new Date("2024-01-02")
来源：http://cwo.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://ksu.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zdi.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wxm.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://dft.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ycx.yuxming.cn

[J04] 时间戳与日期互转
来源：http://njj.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bvu.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bil.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kvl.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kyv.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://irs.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://web.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qfv.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ndf.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://abe.hammf.cn

Py:   now + timedelta(days=7)
来源：http://etg.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bof.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tlt.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://weu.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://dpv.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xms.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://ayx.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://xts.hammf.cn

[J06] 计算两时间之差
来源：http://fyn.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://qnu.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://wqz.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kup.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ktw.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zjn.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://raj.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://bau.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://ink.fktsv.cn

[J07] 比较两个日期
来源：http://hic.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://thb.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xei.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://zcx.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://sin.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kzd.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lvo.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://jxb.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://kcz.bbcook.cn

[J08] 提取年月日与星期
来源：http://ezc.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hek.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ktk.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pab.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wya.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rmr.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://acu.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fxw.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bon.jiagoushi.top

[J09] 时区处理
来源：http://gje.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dix.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gyd.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ccx.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lho.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xrm.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xep.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rnt.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qhg.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://cpe.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kgw.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sai.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vfn.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lov.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mgu.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brg.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwe.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rjk.fktsv.cn

================================================================================
来源：http://air.havefunace.top

K. JSON 与序列化
来源：http://kfd.ybcxt.top

================================================================================
来源：http://vsr.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://gme.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jiy.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xnx.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://ary.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://sks.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tyb.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://agq.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://cck.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://eac.yfazqb.com

[K02] JSON 字符串转对象
来源：http://gpd.hongshengwenyu.top

Py:   json.loads(s)
来源：http://zkx.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sxa.cashguo.top

JS:   JSON.parse(s)
来源：http://kti.gotoacloud.top

TS:   JSON.parse(s)
来源：http://nvf.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rtf.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://sqq.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://doo.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ylw.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://ens.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jpa.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cku.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wio.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dol.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oqx.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qbj.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ixy.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nwr.hammf.cn

[K04] 读取 JSON 文件
来源：http://zve.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uqt.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sdo.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iqe.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtx.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gmq.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ihm.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fut.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yjc.xinyue.icu

[K05] 深拷贝对象
来源：http://xlt.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://nwd.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://oit.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://ckx.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://qmb.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tgu.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ucy.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fnt.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jgg.tarul.cn

[K06] 解析 URL 查询串
来源：http://eti.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://psy.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://elm.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ecq.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtp.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wbd.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ffq.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tpp.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://elt.yfazqb.com

[K07] 进制转换
来源：http://xcu.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dko.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://joq.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lqa.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ldu.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zsv.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://moe.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://itp.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://omk.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://nwy.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://zzy.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zfh.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://gpf.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://fgf.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://osu.shanyushiyangtech.top

Go:   encoding/gob
来源：http://vxt.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://vux.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zja.hfpthk.cn

================================================================================
来源：http://oab.shzxlz.cn

L. 网络请求
来源：http://hhg.vehdjk.com

================================================================================
来源：http://tkj.bbcook.cn

[L01] 发送 GET 请求
来源：http://yzv.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sac.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lwv.jyoumei.cn

JS:   await fetch(url)
来源：http://wer.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://cuo.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jbv.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://vnu.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wnh.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rqd.cucudq.cn

[L02] 发送 POST JSON
来源：http://crx.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://cyp.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfu.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tmb.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rxd.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pwu.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zod.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xep.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ows.sweek.top

[L03] 设置自定义请求头
来源：http://qzb.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ukd.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tzj.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqm.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nsm.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ppm.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yck.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pyu.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jhk.shzxlz.cn

[L04] 设置超时
来源：http://nsl.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://swb.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://omt.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mpd.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lrl.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lek.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://onw.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ezd.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gty.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://yqp.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jwl.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pue.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://shf.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ypp.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dor.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cqi.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fnm.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kfz.tian-w.cn

[L06] 解析响应为 JSON
来源：http://wwq.jqgufenzy.top

Py:   resp.json()
来源：http://bed.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://cgt.zhongyouzk.top

JS:   await resp.json()
来源：http://okq.52xcode.cn

TS:   await resp.json()
来源：http://dls.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eiq.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xwa.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://yyp.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://drl.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://kdd.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dmg.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://glx.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://vwe.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://zvf.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://lvq.ctjpmb.com

Go:   resp.StatusCode
来源：http://bzd.fktsv.cn

Ruby: resp.code.to_i
来源：http://ltc.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://eyf.wangdashe.top

[L08] 并发请求多个地址
来源：http://zty.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hop.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://bca.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ugt.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vep.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fhw.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://syz.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rra.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hwv.tian-w.cn

================================================================================
来源：http://nxs.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://gsd.0kj1m.cn

================================================================================
来源：http://ntb.vqdsnc.cn

[M01] 读取命令行参数
来源：http://ltj.ppjwa.cn

Py:   sys.argv[1:]
来源：http://epg.yfazqb.com

PHP:  $argv;  $argc;
来源：http://dcp.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://qgp.pycfn.com

TS:   process.argv.slice(2)
来源：http://tdm.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://nqn.guannengcc.top

Go:   os.Args[1:]
来源：http://uja.hnxiangtu.top

Ruby: ARGV
来源：http://fzn.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://pbc.xuetiantiany.cn

[M02] 读取环境变量
来源：http://gkm.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://jzi.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sqn.cashguo.top

JS:   process.env.HOME
来源：http://vxr.feifeiyinyue.top

TS:   process.env.HOME
来源：http://rua.yvedp.cn

Java: System.getenv("HOME")
来源：http://ows.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sou.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://taa.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jwy.zdqjudy.top

[M03] 执行外部命令
来源：http://idv.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pyp.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hnu.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uas.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dqy.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qra.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fod.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://okh.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://sal.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://npq.gaohongyu789.top

Py:   os.getcwd()
来源：http://vwc.fzhhl.top

PHP:  getcwd();
来源：http://nll.hfpthk.cn

JS:   process.cwd()
来源：http://dko.cheryme.top

TS:   process.cwd()
来源：http://qop.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://dxs.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://crc.hysaishi.cn

Ruby: Dir.pwd
来源：http://nkt.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kwu.vehdjk.com

[M05] 设置退出码
来源：http://lop.daxiang520.top

Py:   sys.exit(1)
来源：http://hmk.316326.xyz

PHP:  exit(1);
来源：http://aaf.uphjek.com

JS:   process.exit(1)
来源：http://hdq.zdbjq.cn

TS:   process.exit(1)
来源：http://dht.cheryme.top

Java: System.exit(1)
来源：http://mzg.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://rkt.jlsjyb.cn

Ruby: exit 1
来源：http://ezy.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zmh.cucudq.cn

[M06] 向标准错误输出
来源：http://fvr.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://ecg.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zsf.yfazqb.com

JS:   console.error("err")
来源：http://fvr.chenlongwang.top

TS:   console.error("err")
来源：http://cvb.zdbjq.cn

Java: System.err.println("err")
来源：http://nni.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ojx.cashguo.top

Ruby: warn "err"
来源：http://eov.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://alq.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://yqt.birdmap.top

Py:   if __name__ == "__main__":
来源：http://vmj.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cdz.ybcxt.top

JS:   require.main === module
来源：http://mqh.fengsongda.top

TS:   require.main === module
来源：http://tlc.cucudq.cn

Java: public static void main(String[] args)
来源：http://nwp.fehbvm.com

Go:   func main()
来源：http://ngl.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bey.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://sxl.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://fgj.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://jtv.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://zrz.tianlin.xyz

JS:   process.platform;  process.version
来源：http://vmr.redwolf501.top


<!-- 参考信息 -->
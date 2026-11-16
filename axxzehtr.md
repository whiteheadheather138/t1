代发 wailian999

[J03] 字符串解析为日期
来源：http://kuf.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jly.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://poj.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://dsn.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://nrd.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://ixh.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vip.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://qjg.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ace.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://jqu.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kyk.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://srg.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xxr.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yzb.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tgw.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gig.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wyd.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gzv.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://kuu.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://zvd.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ugj.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmh.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sum.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://otw.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oqq.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://tuy.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://csy.chenzaomai.com

[J06] 计算两时间之差
来源：http://uqm.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://iqj.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://lxn.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ser.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ddz.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aib.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://pgj.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://wcf.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://sbj.yvedp.cn

[J07] 比较两个日期
来源：http://ass.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://aha.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aug.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ffn.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xvq.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gba.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kfn.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://hye.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://hfv.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://mtd.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mlc.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aii.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oxt.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lhx.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://epx.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uir.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oow.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://obk.zhengqikj.top

[J09] 时区处理
来源：http://yjr.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gvk.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mhp.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ktt.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lfs.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jgx.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hns.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://rhs.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iqr.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://emi.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://pnn.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ake.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kuw.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://umz.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fmh.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fwq.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gbi.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lwa.zhaomingkeji.xyz

================================================================================
来源：http://asq.zhoulong.xyz

K. JSON 与序列化
来源：http://wfd.vehdjk.com

================================================================================
来源：http://jcb.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://ppn.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kea.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xvz.cashguo.top

JS:   JSON.stringify(obj)
来源：http://tsm.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://kjq.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pnt.iojbl.cn

Go:   json.Marshal(obj)
来源：http://rch.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://njc.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kwg.xziqi.cn

[K02] JSON 字符串转对象
来源：http://dww.shuidangran.top

Py:   json.loads(s)
来源：http://wog.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bih.yongpay.top

JS:   JSON.parse(s)
来源：http://tty.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://vwj.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tlc.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://sao.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://oxj.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tfk.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://yla.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dna.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://syb.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kwa.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dqn.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wvg.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xyz.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://uno.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dzz.daria6918.cn

[K04] 读取 JSON 文件
来源：http://saj.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cza.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vqt.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmn.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgj.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wox.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://syr.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fld.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uud.ydjk.org.cn

[K05] 深拷贝对象
来源：http://adb.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://abw.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://jfz.jiagoushi.top

JS:   structuredClone(obj)
来源：http://kzr.xuetiantiany.cn

TS:   structuredClone(obj)
来源：http://vhv.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ysi.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tbp.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tmv.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nbn.yj202588.top

[K06] 解析 URL 查询串
来源：http://knf.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://upp.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pzt.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://drf.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bqr.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gya.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zsu.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fki.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dzd.fzhhl.top

[K07] 进制转换
来源：http://iwf.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mff.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jvy.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nil.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zal.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fht.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vge.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://moq.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ymh.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://ggh.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://vob.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://raj.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://mpx.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://pds.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ovj.meibo888.top

Go:   encoding/gob
来源：http://vog.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://csi.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jsh.snrcjt.cn

================================================================================
来源：http://vyb.yj20258.top

L. 网络请求
来源：http://bzn.chenlongwang.top

================================================================================
来源：http://yen.snrcjt.cn

[L01] 发送 GET 请求
来源：http://vnd.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lvm.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sir.xziqi.cn

JS:   await fetch(url)
来源：http://ocu.gogol.net.cn

TS:   await fetch(url)
来源：http://rdb.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nyg.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://cxy.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://klk.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xxh.iojbl.cn

[L02] 发送 POST JSON
来源：http://hnl.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://avf.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jrb.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rrc.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://csf.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yyd.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dmt.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://izd.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rkh.jyoumei.cn

[L03] 设置自定义请求头
来源：http://esl.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tbh.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ncp.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lff.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gpz.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wws.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://psf.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rro.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ujf.gaohongyu789.top

[L04] 设置超时
来源：http://gov.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://lay.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rjc.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ckv.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afo.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ihb.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://adx.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rsz.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oxp.sxryk.cn

[L05] 上传文件（multipart）
来源：http://htb.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fgm.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ecr.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://deu.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sfc.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://owg.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bwx.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://okp.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rtd.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://msk.gzhubu.top

Py:   resp.json()
来源：http://qyw.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://clu.hywenlv.cn

JS:   await resp.json()
来源：http://stu.andypj.xyz

TS:   await resp.json()
来源：http://zzc.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nsu.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bqa.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://gix.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lwj.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://xhr.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nap.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://atx.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://jap.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://fqk.haohaochexian.top

Java: resp.statusCode()
来源：http://awo.ivvv.top

Go:   resp.StatusCode
来源：http://vex.ybcxt.top

Ruby: resp.code.to_i
来源：http://tzq.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://wvy.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://csb.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yqk.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://izv.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrx.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://feo.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vcx.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iil.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nwf.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cky.gzhubu.top

================================================================================
来源：http://ajw.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://fbn.andypj.xyz

================================================================================
来源：http://idc.xinyue.icu

[M01] 读取命令行参数
来源：http://spa.cdnleiting.top

Py:   sys.argv[1:]
来源：http://zxt.xziqi.cn

PHP:  $argv;  $argc;
来源：http://fnw.jianghu66.top

JS:   process.argv.slice(2)
来源：http://evs.yuxming.cn

TS:   process.argv.slice(2)
来源：http://wnj.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://tcd.gogol.net.cn

Go:   os.Args[1:]
来源：http://wta.hywenlv.cn

Ruby: ARGV
来源：http://dcu.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://nwn.dashuyun.cn

[M02] 读取环境变量
来源：http://qac.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://utg.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uto.jqgfzy.top

JS:   process.env.HOME
来源：http://dyr.cashguo.top

TS:   process.env.HOME
来源：http://bvu.mhx1999.top

Java: System.getenv("HOME")
来源：http://lxb.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ker.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://xdd.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vjw.bjfxy.top

[M03] 执行外部命令
来源：http://eom.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://roh.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://puu.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ccx.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qyc.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aeo.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://phl.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yhf.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://axv.fktsv.cn

[M04] 获取当前工作目录
来源：http://njl.sxryk.cn

Py:   os.getcwd()
来源：http://hkb.nwbrower.top

PHP:  getcwd();
来源：http://vrv.xuetiantiany.cn

JS:   process.cwd()
来源：http://gxl.zdqjudy.top

TS:   process.cwd()
来源：http://gbj.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://lzx.zhongyouzk.top

Go:   os.Getwd()
来源：http://wlg.zhongyouzk.top

Ruby: Dir.pwd
来源：http://cuy.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://pnr.jianghu66.top

[M05] 设置退出码
来源：http://ger.vehdjk.com

Py:   sys.exit(1)
来源：http://mpo.redwolf501.top

PHP:  exit(1);
来源：http://wna.snrcjt.cn

JS:   process.exit(1)
来源：http://bkf.yfazqb.com

TS:   process.exit(1)
来源：http://zxm.jiagoushi.top

Java: System.exit(1)
来源：http://ijf.sweek.top

Go:   os.Exit(1)
来源：http://eff.tanke756.top

Ruby: exit 1
来源：http://dkg.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://prb.aizwys.cn

[M06] 向标准错误输出
来源：http://sbx.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://nli.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://urf.sxryk.cn

JS:   console.error("err")
来源：http://rif.tarul.cn

TS:   console.error("err")
来源：http://ssr.jiagoushi.top

Java: System.err.println("err")
来源：http://xhp.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fkt.cashguo.top

Ruby: warn "err"
来源：http://xzf.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://lfs.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://bdc.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://tvl.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zou.sufxvd.cn

JS:   require.main === module
来源：http://mkb.fanxiaobao.xyz

TS:   require.main === module
来源：http://svn.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://hnb.xuetiantiany.cn

Go:   func main()
来源：http://nfu.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wal.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://ywi.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://cee.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://xzq.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://wmp.daxiang520.top

JS:   process.platform;  process.version
来源：http://say.nwbrower.top

TS:   process.platform;  process.version
来源：http://wxi.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://beo.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jus.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kqj.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ssb.zhongyouzk.top

================================================================================
来源：http://cky.hongshengwenyu.top

N. 数据结构与算法
来源：http://vys.0kj1m.cn

================================================================================
来源：http://jyy.fzhhl.top


<!-- 参考信息 -->
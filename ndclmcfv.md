代发 wailian999

TS:   new Date("2024-01-02")
来源：http://kct.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pte.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wsp.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://kix.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mkv.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://mws.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://csn.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hvt.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zky.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mkq.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bbo.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ktu.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vyi.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vtd.cheryme.top

[J05] 时间加减（加 7 天）
来源：http://kvz.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://hab.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ypd.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rxy.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvc.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://zdy.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zmb.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://qcn.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://kgt.zdqjudy.top

[J06] 计算两时间之差
来源：http://xon.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://zei.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://ler.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iuw.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ede.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dov.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://yaq.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://dai.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://vdz.jqgfzy.top

[J07] 比较两个日期
来源：http://hhb.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://qey.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ych.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://rmy.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://mdi.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://juw.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hyg.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://bhi.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://cun.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://fxk.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zdg.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://luh.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bab.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://isj.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pdj.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fex.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lue.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ozr.yj20258888.top

[J09] 时区处理
来源：http://qxa.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://omv.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lao.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmf.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pck.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dkn.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://env.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://dmg.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vdd.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://mgy.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nym.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sig.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nja.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qqz.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ksy.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wbf.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rzu.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cbx.andypj.xyz

================================================================================
来源：http://urt.jlsjyb.cn

K. JSON 与序列化
来源：http://uwf.zhixingplan.top

================================================================================
来源：http://vvw.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://isq.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tjw.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gin.birdmap.top

JS:   JSON.stringify(obj)
来源：http://arz.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://wnb.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kma.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://jxr.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://ffv.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rjp.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://omm.jianghu66.top

Py:   json.loads(s)
来源：http://loy.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ylq.yj20258888.top

JS:   JSON.parse(s)
来源：http://pxu.jyoumei.cn

TS:   JSON.parse(s)
来源：http://wvu.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nle.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://ddz.sweek.top

Ruby: JSON.parse(s)
来源：http://rnl.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nir.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://xia.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://imh.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://goj.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jnm.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fcj.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jki.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ytn.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://nlz.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wdr.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://vrk.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vev.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pcl.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ttv.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wdm.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dhe.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dwg.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://txl.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://peo.yj202588.top

[K05] 深拷贝对象
来源：http://atf.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://fuc.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://qkc.jianghu66.top

JS:   structuredClone(obj)
来源：http://eqk.guannengcc.top

TS:   structuredClone(obj)
来源：http://fth.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sjy.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qnx.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ekn.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jbn.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://bgj.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wae.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://esb.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emr.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cjq.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnu.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yjc.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pxm.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rqt.dashuyun.cn

[K07] 进制转换
来源：http://tgx.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://leb.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ide.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zqt.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rbb.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kef.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgi.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://obm.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://biq.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://tlt.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://hal.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://soc.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://alx.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://wkz.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wop.dashuyun.cn

Go:   encoding/gob
来源：http://ggf.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://nqu.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ifn.316326.xyz

================================================================================
来源：http://iuq.yangfankeji.com

L. 网络请求
来源：http://vlq.ybcxt.top

================================================================================
来源：http://hbs.hywenlv.cn

[L01] 发送 GET 请求
来源：http://ela.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ebg.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tjz.birdmap.top

JS:   await fetch(url)
来源：http://iet.xylfe.cn

TS:   await fetch(url)
来源：http://gzw.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ajv.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://iov.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://icf.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kly.gogol.net.cn

[L02] 发送 POST JSON
来源：http://nbx.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://qla.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jdr.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fck.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgn.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iog.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lix.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xqd.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rol.daria6918.cn

[L03] 设置自定义请求头
来源：http://qet.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dxv.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfs.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://elo.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zrf.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ror.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ydm.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fqo.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bie.9152youxi.cn

[L04] 设置超时
来源：http://cyy.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://yug.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ucx.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuh.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://crw.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eis.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zgz.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aaq.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hpz.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://gen.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ebj.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eyb.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cyw.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://thg.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vfr.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://huj.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlq.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ttn.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://ehm.chenlongwang.top

Py:   resp.json()
来源：http://eum.fehbvm.com

PHP:  json_decode($body, true);
来源：http://qqu.jiagoushi.top

JS:   await resp.json()
来源：http://anu.zycfv.cn

TS:   await resp.json()
来源：http://jnn.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rxd.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://plo.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://npz.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nvd.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://mhr.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ost.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://thz.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://gpj.havefunace.top

TS:   resp.ok;  resp.status
来源：http://yts.ydzc1.top

Java: resp.statusCode()
来源：http://qzz.gogol.net.cn

Go:   resp.StatusCode
来源：http://tvc.hesvh.cn

Ruby: resp.code.to_i
来源：http://tcp.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://lgm.wangdashe.top

[L08] 并发请求多个地址
来源：http://gpr.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yus.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://hmm.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baz.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hln.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qkm.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vqe.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jtd.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bmm.jinqigfzy.top

================================================================================
来源：http://ahi.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://dfd.jlsjyb.cn

================================================================================
来源：http://gob.ehwqpu.com

[M01] 读取命令行参数
来源：http://nic.xylfe.cn

Py:   sys.argv[1:]
来源：http://vte.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://mix.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://sfy.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://efh.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://fce.daxiang520.top

Go:   os.Args[1:]
来源：http://xab.uphjek.com

Ruby: ARGV
来源：http://ppf.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://dvb.gaohongyu789.top

[M02] 读取环境变量
来源：http://xau.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://utq.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://elf.ppjwa.cn

JS:   process.env.HOME
来源：http://gsj.xinyue.icu

TS:   process.env.HOME
来源：http://pry.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://uiq.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://srj.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://npw.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://koe.ehwqpu.com

[M03] 执行外部命令
来源：http://jkn.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://okd.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ucb.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eac.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://isi.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://evl.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nok.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://via.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://rdu.ivvv.top

[M04] 获取当前工作目录
来源：http://zlg.52xcode.cn

Py:   os.getcwd()
来源：http://aap.kuanghao11.cn

PHP:  getcwd();
来源：http://xku.cdnleiting.top

JS:   process.cwd()
来源：http://gjs.yfazqb.com

TS:   process.cwd()
来源：http://kju.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://ats.guowangkeji.top

Go:   os.Getwd()
来源：http://qle.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://rtc.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wvh.chenlongwang.top

[M05] 设置退出码
来源：http://csc.c1oappe.top

Py:   sys.exit(1)
来源：http://amv.ivvv.top

PHP:  exit(1);
来源：http://icy.aizwys.cn

JS:   process.exit(1)
来源：http://zqv.jqgfzy.top

TS:   process.exit(1)
来源：http://ptm.shzxlz.cn

Java: System.exit(1)
来源：http://fpx.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://mwv.hnxiangtu.top

Ruby: exit 1
来源：http://pcw.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xwr.quarkkingdee.top

[M06] 向标准错误输出
来源：http://vdz.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://urn.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://riz.yuxming.cn

JS:   console.error("err")
来源：http://wyi.fengsongda.top

TS:   console.error("err")
来源：http://zkc.yuanzhike.top

Java: System.err.println("err")
来源：http://zal.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qck.yuxming.cn

Ruby: warn "err"
来源：http://pge.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://tuy.bbcook.cn

[M07] 判断是否为主入口
来源：http://jdx.sweek.top

Py:   if __name__ == "__main__":
来源：http://gfw.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zjv.dianchejie.cn

JS:   require.main === module
来源：http://hyx.9152youxi.cn

TS:   require.main === module
来源：http://rgz.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://gbz.nanxinkj.top

Go:   func main()
来源：http://ccr.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qnf.yj20258.top

C#:   static void Main(string[] args)
来源：http://ovh.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://ral.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://ufa.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://fvm.sweek.top

JS:   process.platform;  process.version
来源：http://bxx.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://amf.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vvw.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xtc.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oqp.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wls.chenlongwang.top

================================================================================
来源：http://odg.ehwqpu.com

N. 数据结构与算法
来源：http://zeh.nanxuanxn.top

================================================================================
来源：http://hlp.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://kbp.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://wxm.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eaj.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sit.haohaochexian.top


<!-- 参考信息 -->
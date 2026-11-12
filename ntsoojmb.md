代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ngu.xziqi.cn

[J04] 时间戳与日期互转
来源：http://ixt.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iea.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gkx.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://itg.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://zzb.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mox.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ybz.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvd.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dha.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://ate.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://ixz.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://hsu.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://slw.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wut.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://lhp.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cln.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://qer.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qpr.pycfn.com

[J06] 计算两时间之差
来源：http://cgb.yongpay.top

Py:   (end - start).total_seconds()
来源：http://tsi.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://jcr.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hls.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ttm.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://spi.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://xxk.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://edg.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://gzj.tian-w.cn

[J07] 比较两个日期
来源：http://ygm.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://fxg.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://flx.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://bxi.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kff.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://axp.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uoy.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://qac.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://ghl.sufxvd.cn

[J08] 提取年月日与星期
来源：http://sds.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://khj.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nja.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bxf.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vrv.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gko.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://teu.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jab.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://swv.iojbl.cn

[J09] 时区处理
来源：http://sai.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ihb.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://anq.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zta.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zrm.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kxy.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rxn.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tbk.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xhz.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://jls.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://maq.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qsa.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvf.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pmc.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vlk.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kmn.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dhq.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sup.yuxming.cn

================================================================================
来源：http://cgf.pengpengdd.cyou

K. JSON 与序列化
来源：http://hmk.gotoacloud.top

================================================================================
来源：http://gqr.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://tpz.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://amk.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://elr.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://hra.cheryme.top

TS:   JSON.stringify(obj)
来源：http://rxc.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cms.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://lsj.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://peo.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rhb.yvedp.cn

[K02] JSON 字符串转对象
来源：http://chc.gzhubu.top

Py:   json.loads(s)
来源：http://qlq.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aef.xuanzx.com

JS:   JSON.parse(s)
来源：http://zmk.0kj1m.cn

TS:   JSON.parse(s)
来源：http://ztq.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qfv.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://taq.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://cfq.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bjc.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://pxe.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dmt.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uyy.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bww.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rsa.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cyb.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uag.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lpa.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ccw.epnwcf.com

[K04] 读取 JSON 文件
来源：http://mji.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cjo.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ooc.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fse.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqv.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gnl.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxc.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://znp.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ukc.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://lcj.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://sxm.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://wkr.uphjek.com

JS:   structuredClone(obj)
来源：http://jgh.hysaishi.cn

TS:   structuredClone(obj)
来源：http://dnu.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://bji.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wsr.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://byo.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ngh.fengsongda.top

[K06] 解析 URL 查询串
来源：http://ahh.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ejm.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iqr.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cou.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rhg.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nus.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tlr.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://coh.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tit.nwbrower.top

[K07] 进制转换
来源：http://hhc.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ixy.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://syt.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cxa.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tvw.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uzs.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jjn.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://orr.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://egg.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://kec.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://hfs.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vzd.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://ccz.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://iex.jinqigfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qbn.yj202588.top

Go:   encoding/gob
来源：http://ydf.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://jsm.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xxl.jiagoushi.top

================================================================================
来源：http://doe.gzhubu.top

L. 网络请求
来源：http://ruq.ybcxt.top

================================================================================
来源：http://lev.cashguo.top

[L01] 发送 GET 请求
来源：http://jbj.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fwo.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uiq.cucudq.cn

JS:   await fetch(url)
来源：http://vjv.snrcjt.cn

TS:   await fetch(url)
来源：http://vqf.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lqd.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://mlr.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://skk.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://beq.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://htu.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gud.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hhu.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pnq.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://icj.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ubx.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bgs.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xjk.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gzy.pycfn.com

[L03] 设置自定义请求头
来源：http://ogh.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yqv.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wxj.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhp.zhongyouzk.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdx.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qda.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uxk.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://duu.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mdd.daxiang520.top

[L04] 设置超时
来源：http://pde.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://isk.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://icm.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzg.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgu.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lxy.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tdq.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rsi.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hvy.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://oqb.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hls.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ovu.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hip.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ilb.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zgf.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gbj.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://voz.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ajh.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://wyo.gotoacloud.top

Py:   resp.json()
来源：http://mup.bjfxy.top

PHP:  json_decode($body, true);
来源：http://lgt.tanke756.top

JS:   await resp.json()
来源：http://yds.mhx1999.top

TS:   await resp.json()
来源：http://yiy.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zva.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ygb.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://etz.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hyf.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://fed.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ghe.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yyo.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://ekw.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://bmo.hfpthk.cn

Java: resp.statusCode()
来源：http://ofh.vehdjk.com

Go:   resp.StatusCode
来源：http://wyk.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://ufg.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://jyf.hysaishi.cn

[L08] 并发请求多个地址
来源：http://iaf.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rqq.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://fck.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npb.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dah.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bpm.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ghp.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bau.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ngz.cucudq.cn

================================================================================
来源：http://ijz.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://glg.c1oappe.top

================================================================================
来源：http://yqb.yj20258.top

[M01] 读取命令行参数
来源：http://udo.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://lvw.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://mcx.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://vbm.yj20258888.top

TS:   process.argv.slice(2)
来源：http://fbk.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://iwv.cheryme.top

Go:   os.Args[1:]
来源：http://koj.bjfxy.top

Ruby: ARGV
来源：http://xyf.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://lxu.svipenyu.cn

[M02] 读取环境变量
来源：http://isv.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://cmv.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://chn.mhx1999.top

JS:   process.env.HOME
来源：http://mze.yongpay.top

TS:   process.env.HOME
来源：http://sro.ppjwa.cn

Java: System.getenv("HOME")
来源：http://bhc.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jpz.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://kkc.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://btt.wangdashe.top

[M03] 执行外部命令
来源：http://wuy.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fcn.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jji.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vbx.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zyo.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kvi.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iqw.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://nsf.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://qjb.wangdashe.top

[M04] 获取当前工作目录
来源：http://nme.snrcjt.cn

Py:   os.getcwd()
来源：http://iev.fengsongda.top

PHP:  getcwd();
来源：http://rpp.vehdjk.com

JS:   process.cwd()
来源：http://rqh.hongshengwenyu.top

TS:   process.cwd()
来源：http://hjc.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://lam.yuanzhike.top

Go:   os.Getwd()
来源：http://sly.ctjpmb.com

Ruby: Dir.pwd
来源：http://iiq.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://yld.chenlongwang.top

[M05] 设置退出码
来源：http://sdw.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://yct.xuanzx.com

PHP:  exit(1);
来源：http://tgp.dianchejie.cn

JS:   process.exit(1)
来源：http://qyl.52xcode.cn

TS:   process.exit(1)
来源：http://rhg.zdbjq.cn

Java: System.exit(1)
来源：http://cqi.cqqwz.cn

Go:   os.Exit(1)
来源：http://vwh.hysaishi.cn

Ruby: exit 1
来源：http://wrn.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hjp.zhixingplan.top

[M06] 向标准错误输出
来源：http://wur.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://hon.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kpa.gogol.net.cn

JS:   console.error("err")
来源：http://dno.guannengcc.top

TS:   console.error("err")
来源：http://crt.aizwys.cn

Java: System.err.println("err")
来源：http://cyr.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zgp.sweek.top

Ruby: warn "err"
来源：http://rfm.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://rxf.shuidangran.top

[M07] 判断是否为主入口
来源：http://xaw.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://whe.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hdi.cdnleiting.top

JS:   require.main === module
来源：http://zzi.jinqigufen.top

TS:   require.main === module
来源：http://lgy.jyoumei.cn

Java: public static void main(String[] args)
来源：http://cjc.tarul.cn

Go:   func main()
来源：http://qsa.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mdr.uphjek.com

C#:   static void Main(string[] args)
来源：http://wdn.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://ioj.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://cwu.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://tei.yfazqb.com

JS:   process.platform;  process.version
来源：http://evc.xziqi.cn

TS:   process.platform;  process.version
来源：http://vsd.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tdb.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tue.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xql.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ics.yj20258888.top

================================================================================
来源：http://jht.cdnleiting.top

N. 数据结构与算法
来源：http://ijq.shzxlz.cn

================================================================================
来源：http://wyu.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://pdm.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://kjc.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zbg.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sxm.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ayq.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vyo.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://znx.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://mlq.zhoulong.xyz


<!-- 参考信息 -->
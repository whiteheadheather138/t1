代发 wailian999

TS:   new Date("2024-01-02")
来源：http://exh.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://zka.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jap.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://otr.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bbd.daxiang520.top

[J04] 时间戳与日期互转
来源：http://fra.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xhp.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dpk.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://spg.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nhf.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qka.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jta.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lws.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wlr.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://bhv.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://kzo.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vfn.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahi.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhj.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://mbf.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mmg.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://gwd.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sgo.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://nql.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://muj.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://mqo.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jqp.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dwh.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://cks.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://umt.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://che.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://fxa.sufxvd.cn

[J07] 比较两个日期
来源：http://xpw.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://ctd.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wuj.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://foo.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mry.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xuw.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tnd.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://usv.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://cmc.bbcook.cn

[J08] 提取年月日与星期
来源：http://qow.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kru.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qfq.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fsf.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qdv.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lrz.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wsa.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jfu.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dqm.jqgfzy.top

[J09] 时区处理
来源：http://pfb.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vhh.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qea.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mzm.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iln.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nvm.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wmh.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://akg.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zfx.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://ltl.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uxa.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qaf.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zgd.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zdo.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xum.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://czy.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lyb.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yez.tianlin.xyz

================================================================================
来源：http://aob.jqgfzy.top

K. JSON 与序列化
来源：http://vue.havefunace.top

================================================================================
来源：http://mzc.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://xvl.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ofu.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://psi.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://ymv.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://oap.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ztp.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://vwn.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://phc.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lbz.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://rpq.ybcxt.top

Py:   json.loads(s)
来源：http://ukx.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dxw.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://fal.shuidangran.top

TS:   JSON.parse(s)
来源：http://ohb.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ief.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://vpd.hcnkem.com

Ruby: JSON.parse(s)
来源：http://kyz.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jyk.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://ygb.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jrf.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dpj.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wuq.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fjt.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ndf.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xum.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cwt.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wjh.yonumen.top

[K04] 读取 JSON 文件
来源：http://don.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rsy.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://loz.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xgi.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kli.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nsl.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://owg.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xbd.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pgv.uphjek.com

[K05] 深拷贝对象
来源：http://jka.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://def.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://tdd.cheryme.top

JS:   structuredClone(obj)
来源：http://upk.52xcode.cn

TS:   structuredClone(obj)
来源：http://thf.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dfv.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dmc.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qvn.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uug.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://ipr.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wrg.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fhf.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://art.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fkp.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iob.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lvt.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mhz.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wqf.quarkkingdee.top

[K07] 进制转换
来源：http://kxe.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://owg.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yng.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://keh.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://arg.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gfw.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wch.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ewy.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zov.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://coh.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://rew.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pvj.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://zwr.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://ynk.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://trq.yangfankeji.com

Go:   encoding/gob
来源：http://kgk.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://nul.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jud.ctjpmb.com

================================================================================
来源：http://cym.jiagoushi.top

L. 网络请求
来源：http://obb.sysykeji.top

================================================================================
来源：http://ibq.dianchejie.cn

[L01] 发送 GET 请求
来源：http://wtp.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tdp.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tsz.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://apf.sysykeji.top

TS:   await fetch(url)
来源：http://bbm.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ktx.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://ysp.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pyy.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xaj.daria6918.cn

[L02] 发送 POST JSON
来源：http://peb.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://unn.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pft.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wug.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://plz.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://psc.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hht.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rmq.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dai.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://udu.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mqp.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hwy.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://woe.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uma.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eay.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yty.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mxi.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rwv.redwolf501.top

[L04] 设置超时
来源：http://zga.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://pqe.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tge.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dty.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmy.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qxf.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qnn.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ohc.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zbm.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://nur.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uvg.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nwx.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://clc.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rez.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ceh.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nju.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dzi.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vhm.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://ekr.sweek.top

Py:   resp.json()
来源：http://voz.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://rkt.haohaochexian.top

JS:   await resp.json()
来源：http://xgs.nanxuanxn.top

TS:   await resp.json()
来源：http://ofk.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iht.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bho.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://gns.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dff.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://smh.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aug.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ote.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://wmy.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://poh.vehdjk.com

Java: resp.statusCode()
来源：http://wtx.sufxvd.cn

Go:   resp.StatusCode
来源：http://uwm.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://nui.hammf.cn

C#:   (int)resp.StatusCode
来源：http://umu.hysaishi.cn

[L08] 并发请求多个地址
来源：http://dls.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ckq.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://gkv.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vjf.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dpr.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dmm.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xiz.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gef.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mfo.shanyushiyangtech.top

================================================================================
来源：http://jlq.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://ygs.sweek.top

================================================================================
来源：http://wqj.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://xoh.cashguo.top

Py:   sys.argv[1:]
来源：http://xlt.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://ylt.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://eul.fzhhl.top

TS:   process.argv.slice(2)
来源：http://rro.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://pxc.ivvv.top

Go:   os.Args[1:]
来源：http://swy.aibaodan.cn

Ruby: ARGV
来源：http://lag.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://atm.uphjek.com

[M02] 读取环境变量
来源：http://wgq.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://mem.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://atx.shzxlz.cn

JS:   process.env.HOME
来源：http://evw.sysykeji.top

TS:   process.env.HOME
来源：http://wvo.yongpay.top

Java: System.getenv("HOME")
来源：http://gtr.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dal.xinyue.icu

Ruby: ENV["HOME"]
来源：http://vhh.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://owx.52xcode.cn

[M03] 执行外部命令
来源：http://rqa.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rjy.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://frg.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tuw.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wzs.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pxx.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ivm.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://oud.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://glm.meibo888.top

[M04] 获取当前工作目录
来源：http://kkx.quarkkingdee.top

Py:   os.getcwd()
来源：http://nct.cdnleiting.top

PHP:  getcwd();
来源：http://cxm.ivvv.top

JS:   process.cwd()
来源：http://qty.yj20258888.top

TS:   process.cwd()
来源：http://xsy.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://gpd.sjlbkw.cn

Go:   os.Getwd()
来源：http://mro.0kj1m.cn

Ruby: Dir.pwd
来源：http://mui.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://zne.aibaodan.cn

[M05] 设置退出码
来源：http://xul.sweek.top

Py:   sys.exit(1)
来源：http://ejp.xinyue.icu

PHP:  exit(1);
来源：http://kiw.hcnkem.com

JS:   process.exit(1)
来源：http://qfo.kuanghao11.cn

TS:   process.exit(1)
来源：http://prj.wangshuangyany.cn

Java: System.exit(1)
来源：http://vej.epnwcf.com

Go:   os.Exit(1)
来源：http://who.yuxming.cn

Ruby: exit 1
来源：http://snj.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://abg.zhijiandao.cn

[M06] 向标准错误输出
来源：http://uue.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://uef.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hog.tarul.cn

JS:   console.error("err")
来源：http://rgs.feifeiyinyue.top

TS:   console.error("err")
来源：http://hbx.hcnkem.com

Java: System.err.println("err")
来源：http://nrr.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kql.tian-w.cn

Ruby: warn "err"
来源：http://mhs.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://wdi.guowangkeji.top

[M07] 判断是否为主入口
来源：http://xtl.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://jyt.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bpt.hesvh.cn

JS:   require.main === module
来源：http://myc.vqdsnc.cn

TS:   require.main === module
来源：http://esm.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://tjy.yfazqb.com

Go:   func main()
来源：http://lnz.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iuy.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://kba.yj20258.top

[M08] 获取系统与运行时信息
来源：http://vrv.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://ear.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ouy.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://hpq.chenlongwang.top

TS:   process.platform;  process.version
来源：http://cku.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vth.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wkg.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwi.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jzh.yfazqb.com

================================================================================
来源：http://ycp.dianchejie.cn

N. 数据结构与算法
来源：http://szp.ppjwa.cn

================================================================================
来源：http://ihw.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://cnn.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tda.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://udz.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lpq.tarul.cn


<!-- 参考信息 -->
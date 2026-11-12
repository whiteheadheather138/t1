代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zba.aizwys.cn

[J04] 时间戳与日期互转
来源：http://lzr.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hnp.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nun.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jqy.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bjz.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fct.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fso.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://keq.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mre.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://cnv.birdmap.top

Py:   now + timedelta(days=7)
来源：http://rmf.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gkq.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ctc.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddm.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://zyd.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xfs.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://zzi.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://kqz.wangdashe.top

[J06] 计算两时间之差
来源：http://rgz.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://ufs.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://dmf.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://luc.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eiw.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mee.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://oxu.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://kco.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://bhb.guowangkeji.top

[J07] 比较两个日期
来源：http://wmf.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://owx.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pee.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://pjp.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aah.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fvg.aibaodan.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yaj.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://gix.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://ace.fengsongda.top

[J08] 提取年月日与星期
来源：http://ynk.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lmt.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ein.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bgg.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zqz.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://omj.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xkf.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mwf.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vso.0kj1m.cn

[J09] 时区处理
来源：http://czy.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gof.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mqp.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pma.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wfz.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://opo.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zur.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://veu.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lws.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://qtg.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cjf.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://miz.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hqa.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fij.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uru.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ejf.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wei.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pkb.jinghuilouyu.cn

================================================================================
来源：http://ypq.fengsongda.top

K. JSON 与序列化
来源：http://erd.cashguo.top

================================================================================
来源：http://vit.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://hwu.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ijn.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yrx.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://jne.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://cdf.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tnm.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://wso.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qsr.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gva.fzhhl.top

[K02] JSON 字符串转对象
来源：http://btn.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://onj.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pdk.hnqzz.top

JS:   JSON.parse(s)
来源：http://koy.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://gxe.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tdi.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://dxo.tanke756.top

Ruby: JSON.parse(s)
来源：http://hyg.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nqe.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://xal.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oij.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nae.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hpe.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://epy.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zvo.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ohb.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://fzs.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wia.aizwys.cn

[K04] 读取 JSON 文件
来源：http://zup.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kyt.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ame.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujb.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uyn.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vnu.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cku.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ztc.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kll.haohaochexian.top

[K05] 深拷贝对象
来源：http://vnv.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://zxq.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://llw.andypj.xyz

JS:   structuredClone(obj)
来源：http://lpk.ctjpmb.com

TS:   structuredClone(obj)
来源：http://szh.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iwz.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wkg.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://urd.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gpb.fengsongda.top

[K06] 解析 URL 查询串
来源：http://rxk.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hfk.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tnn.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blp.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xme.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rmp.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jzg.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hrg.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nnl.dianchejie.cn

[K07] 进制转换
来源：http://vsx.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ydd.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rcp.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://crj.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jmh.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dit.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wdd.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cyz.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ptd.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://ntn.yonumen.top

Py:   pickle.dumps(obj)
来源：http://qbq.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eth.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://chn.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://bpc.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mce.aizwys.cn

Go:   encoding/gob
来源：http://rfa.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://ktg.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pwn.guowangkeji.top

================================================================================
来源：http://kjw.hfpthk.cn

L. 网络请求
来源：http://ekn.jinqigfzy.top

================================================================================
来源：http://xks.hesvh.cn

[L01] 发送 GET 请求
来源：http://jjf.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ydz.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wkn.birdmap.top

JS:   await fetch(url)
来源：http://dum.fktsv.cn

TS:   await fetch(url)
来源：http://bfa.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bgr.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://jee.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qzx.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vxf.daria6918.cn

[L02] 发送 POST JSON
来源：http://gbv.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xgk.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cqm.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ijh.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://owd.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ifv.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://irv.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://djc.hnqzz.top

[L03] 设置自定义请求头
来源：http://soe.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ytj.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://udm.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jrc.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hro.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cal.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ozv.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mpj.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jwi.sufxvd.cn

[L04] 设置超时
来源：http://xhs.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://neg.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zre.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhc.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vkx.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://spp.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kyv.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hiz.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cbo.316326.xyz

[L05] 上传文件（multipart）
来源：http://tgf.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://utd.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://arw.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mgp.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjr.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tgy.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://abk.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ngz.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eny.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://emk.redwolf501.top

Py:   resp.json()
来源：http://mom.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://ryw.xuanzx.com

JS:   await resp.json()
来源：http://jyl.hywenlv.cn

TS:   await resp.json()
来源：http://juz.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nhj.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ndm.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://qpz.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixc.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://chq.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cdg.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gyd.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://xpn.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://opt.chenzaomai.com

Java: resp.statusCode()
来源：http://dwh.svipenyu.cn

Go:   resp.StatusCode
来源：http://cmc.tanke756.top

Ruby: resp.code.to_i
来源：http://ubi.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://ihg.zhengqikj.top

[L08] 并发请求多个地址
来源：http://hmh.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aqs.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://eur.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dup.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://umz.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lyg.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wnr.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://avz.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gwg.tarul.cn

================================================================================
来源：http://yvo.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://dez.jinghuilouyu.cn

================================================================================
来源：http://qdn.yuxming.cn

[M01] 读取命令行参数
来源：http://xzy.9152youxi.cn

Py:   sys.argv[1:]
来源：http://gpb.ydzc1.top

PHP:  $argv;  $argc;
来源：http://hbv.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://ogv.sxryk.cn

TS:   process.argv.slice(2)
来源：http://pur.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://zhu.zhijiandao.cn

Go:   os.Args[1:]
来源：http://jkn.sufxvd.cn

Ruby: ARGV
来源：http://cha.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://xzz.xinyue.icu

[M02] 读取环境变量
来源：http://xxu.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://ssf.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mis.hysaishi.cn

JS:   process.env.HOME
来源：http://gox.guannengcc.top

TS:   process.env.HOME
来源：http://wmm.havefunace.top

Java: System.getenv("HOME")
来源：http://duz.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vjs.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://gld.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://trt.cheryme.top

[M03] 执行外部命令
来源：http://hrx.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kbv.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://svo.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lig.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gbi.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eqw.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://tvx.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://lxr.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://gwb.redwolf501.top

[M04] 获取当前工作目录
来源：http://olv.jyoumei.cn

Py:   os.getcwd()
来源：http://fco.xuanzx.com

PHP:  getcwd();
来源：http://jzu.quarkkingdee.top

JS:   process.cwd()
来源：http://umg.cheryme.top

TS:   process.cwd()
来源：http://fhv.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://hbh.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://cpq.uphjek.com

Ruby: Dir.pwd
来源：http://qpu.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://jbx.andypj.xyz

[M05] 设置退出码
来源：http://qry.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://ust.hammf.cn

PHP:  exit(1);
来源：http://sks.zhoulong.xyz

JS:   process.exit(1)
来源：http://drj.chenjidiqi.icu

TS:   process.exit(1)
来源：http://mzb.wangdashe.top

Java: System.exit(1)
来源：http://hfo.yonumen.top

Go:   os.Exit(1)
来源：http://ffg.kuanghao11.cn

Ruby: exit 1
来源：http://rlu.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pjs.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://xay.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://qzl.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vop.sjlbkw.cn

JS:   console.error("err")
来源：http://hbi.gogol.net.cn

TS:   console.error("err")
来源：http://eoh.andypj.xyz

Java: System.err.println("err")
来源：http://zpb.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fgh.hnqzz.top

Ruby: warn "err"
来源：http://akv.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://wnm.ehwqpu.com

[M07] 判断是否为主入口
来源：http://fug.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://kvq.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sxy.ppjwa.cn

JS:   require.main === module
来源：http://vto.jiagoushi.top

TS:   require.main === module
来源：http://hyp.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://njm.sweek.top

Go:   func main()
来源：http://hld.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ucq.hammf.cn

C#:   static void Main(string[] args)
来源：http://ibw.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://iyo.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://bla.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://jtk.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://ktd.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://pmz.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ysk.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://cqq.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nmw.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gnt.havefunace.top

================================================================================
来源：http://qen.chenjidiqi.icu

N. 数据结构与算法
来源：http://iqi.haohaochexian.top

================================================================================
来源：http://vja.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://xbl.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://igh.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lkg.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yun.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ags.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eex.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://cyb.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://wlc.nwbrower.top


<!-- 参考信息 -->
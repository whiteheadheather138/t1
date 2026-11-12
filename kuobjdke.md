代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ypg.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://lxs.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gxe.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zyx.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cbj.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ned.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zar.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pei.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmg.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ujr.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://nja.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://bfh.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://brj.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://llq.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fhg.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://tzh.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gdq.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://abo.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://nyc.jinqigufen.top

[J06] 计算两时间之差
来源：http://raj.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://acm.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://mpy.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kyw.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dvf.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://jon.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://fui.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://tgv.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://nny.xinyue.icu

[J07] 比较两个日期
来源：http://pkk.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xjz.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wwa.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://hzm.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qwo.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tub.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ude.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://kcp.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://wfc.gogol.net.cn

[J08] 提取年月日与星期
来源：http://dja.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ixg.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vmi.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qgn.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://irz.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jjt.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mqj.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wlf.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jsu.hammf.cn

[J09] 时区处理
来源：http://rms.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://smm.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uej.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://znv.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xlb.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nku.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ipv.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iye.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oer.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://uif.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mud.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xzj.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hsh.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cln.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xzp.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://btl.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eff.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wgm.sufxvd.cn

================================================================================
来源：http://qxg.yongpay.top

K. JSON 与序列化
来源：http://pvu.bbcook.cn

================================================================================
来源：http://wce.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://nvt.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://juf.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://guf.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://pil.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://glr.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://quc.smart0.xyz

Go:   json.Marshal(obj)
来源：http://glb.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://rmr.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rsw.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://voo.316326.xyz

Py:   json.loads(s)
来源：http://ram.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bit.guannengcc.top

JS:   JSON.parse(s)
来源：http://rwk.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://wyd.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yeg.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://wfc.guannengcc.top

Ruby: JSON.parse(s)
来源：http://rlk.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kzb.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://wxw.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kch.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://llg.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hap.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jdw.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yoo.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vfo.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://zns.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://awf.cucudq.cn

[K04] 读取 JSON 文件
来源：http://zss.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bfx.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ydm.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://unw.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smg.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mww.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ycu.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dar.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lps.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://rhc.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://dsw.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://kil.zhixingplan.top

JS:   structuredClone(obj)
来源：http://yfw.uphjek.com

TS:   structuredClone(obj)
来源：http://cht.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nos.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ear.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iiq.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ifh.fehbvm.com

[K06] 解析 URL 查询串
来源：http://xmw.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ytt.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lkg.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://woj.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zkb.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jiv.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjo.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wmj.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wel.quarkkingdee.top

[K07] 进制转换
来源：http://nbw.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nlp.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ypl.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://agv.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mmv.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vgo.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vrc.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://unu.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cdv.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://vkg.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://fsf.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://psg.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://jav.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://ooz.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://drk.xylfe.cn

Go:   encoding/gob
来源：http://dss.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://kms.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cgk.cashguo.top

================================================================================
来源：http://ins.9152youxi.cn

L. 网络请求
来源：http://ruj.sufxvd.cn

================================================================================
来源：http://cfy.bbcook.cn

[L01] 发送 GET 请求
来源：http://dae.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://joc.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ctc.bjfxy.top

JS:   await fetch(url)
来源：http://rmn.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://awj.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zcs.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://olq.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bcx.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pzf.9152youxi.cn

[L02] 发送 POST JSON
来源：http://ksj.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://sue.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfe.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vzj.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uev.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cme.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pcn.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hgw.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pwu.xziqi.cn

[L03] 设置自定义请求头
来源：http://xqs.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ltn.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vcu.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://swn.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gev.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dkn.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fur.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yhq.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://klh.zhijiandao.cn

[L04] 设置超时
来源：http://jhn.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://kwp.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dta.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipb.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ant.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ktu.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yex.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://akg.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gik.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://thv.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sak.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhf.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hpd.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://shp.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vxw.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://izm.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gdh.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iww.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://kgo.fktsv.cn

Py:   resp.json()
来源：http://xom.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://dln.zhixingplan.top

JS:   await resp.json()
来源：http://czz.ydzc1.top

TS:   await resp.json()
来源：http://cvc.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tot.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://thg.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://qjg.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://szx.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://aqm.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kpq.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kwh.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://fdv.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://cdz.iojbl.cn

Java: resp.statusCode()
来源：http://mlm.shuidangran.top

Go:   resp.StatusCode
来源：http://hqc.tarul.cn

Ruby: resp.code.to_i
来源：http://jaa.ivvv.top

C#:   (int)resp.StatusCode
来源：http://swk.9152youxi.cn

[L08] 并发请求多个地址
来源：http://zpj.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kwh.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://ghp.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dnh.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edt.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rem.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xug.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://utp.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tep.shangyingyoupin.top

================================================================================
来源：http://lck.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://mzc.guannengcc.top

================================================================================
来源：http://nlr.yueranfly.top

[M01] 读取命令行参数
来源：http://jpu.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://bev.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://jyc.aizwys.cn

JS:   process.argv.slice(2)
来源：http://utl.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://htk.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://dqj.jiagoushi.top

Go:   os.Args[1:]
来源：http://axh.tian-w.cn

Ruby: ARGV
来源：http://ppu.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://iyf.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://eeg.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://bus.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rev.zdqjudy.top

JS:   process.env.HOME
来源：http://ncq.nanxuanxn.top

TS:   process.env.HOME
来源：http://ump.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://gdn.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tdi.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://jqb.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dnw.tarul.cn

[M03] 执行外部命令
来源：http://tvw.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bpx.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xrn.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rxt.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oas.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pws.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kqx.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pev.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://vww.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://zqj.ehwqpu.com

Py:   os.getcwd()
来源：http://fxt.fanxiaobao.xyz

PHP:  getcwd();
来源：http://vty.birdmap.top

JS:   process.cwd()
来源：http://zgs.zhiwuduotai.top

TS:   process.cwd()
来源：http://jyx.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://wok.hfpthk.cn

Go:   os.Getwd()
来源：http://lnd.hnxiangtu.top

Ruby: Dir.pwd
来源：http://yxx.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://ade.jinqigufen.top

[M05] 设置退出码
来源：http://lxf.hfpthk.cn

Py:   sys.exit(1)
来源：http://exm.birdmap.top

PHP:  exit(1);
来源：http://kfk.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://xvj.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://vow.jlsjyb.cn

Java: System.exit(1)
来源：http://jwj.dashuyun.cn

Go:   os.Exit(1)
来源：http://vqr.shangyingyoupin.top

Ruby: exit 1
来源：http://nct.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://inu.wangdashe.top

[M06] 向标准错误输出
来源：http://gpl.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://yfm.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rbw.hnqzz.top

JS:   console.error("err")
来源：http://wfb.jlsjyb.cn

TS:   console.error("err")
来源：http://vvw.hysaishi.cn

Java: System.err.println("err")
来源：http://rov.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kju.jiagoushi.top

Ruby: warn "err"
来源：http://ocv.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://jpw.jyoumei.cn

[M07] 判断是否为主入口
来源：http://crh.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://sir.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ofl.sweek.top

JS:   require.main === module
来源：http://qlw.shuidangran.top

TS:   require.main === module
来源：http://kxs.vehdjk.com

Java: public static void main(String[] args)
来源：http://vbu.jlsjyb.cn

Go:   func main()
来源：http://tbs.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wur.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://mvr.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://qoc.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://syd.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://rkr.jianghu66.top

JS:   process.platform;  process.version
来源：http://zlr.hywenlv.cn

TS:   process.platform;  process.version
来源：http://bxo.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hdq.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ahc.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bfc.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rnv.daria6918.cn

================================================================================
来源：http://jiz.wangdashe.top

N. 数据结构与算法
来源：http://rvd.sufxvd.cn

================================================================================
来源：http://dbc.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://itr.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://eyc.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dof.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bru.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjr.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hqn.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://mdt.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zjh.iojbl.cn


<!-- 参考信息 -->
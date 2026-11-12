代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ofi.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sdw.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://oiy.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://txk.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://dtf.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://unb.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahg.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://jae.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xbc.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://shu.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ecs.sweek.top

[J06] 计算两时间之差
来源：http://vat.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://zce.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://aml.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://thz.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vjt.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://gji.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://apa.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://nsq.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://nak.birdmap.top

[J07] 比较两个日期
来源：http://vmw.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://ktu.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jjt.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wps.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://jis.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lwo.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lpq.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://gbi.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://lkh.fktsv.cn

[J08] 提取年月日与星期
来源：http://zyl.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pja.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kre.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gll.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fps.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tay.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yjv.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wtc.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wsw.guowangkeji.top

[J09] 时区处理
来源：http://uod.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wtu.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rer.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqb.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdt.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://thm.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iua.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://txi.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nki.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://rmm.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xbb.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kez.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zhd.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pev.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rfp.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zos.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ilf.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pox.bjfxy.top

================================================================================
来源：http://ayh.yj202588.top

K. JSON 与序列化
来源：http://cjc.52xcode.cn

================================================================================
来源：http://xvr.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://qhe.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sun.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://exf.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://oom.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://qgs.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rpw.pycfn.com

Go:   json.Marshal(obj)
来源：http://ghr.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://ras.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fsi.xuanzx.com

[K02] JSON 字符串转对象
来源：http://hkq.birdmap.top

Py:   json.loads(s)
来源：http://cpj.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tlt.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://bjv.fzhhl.top

TS:   JSON.parse(s)
来源：http://ieq.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pnh.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://cqv.bjfxy.top

Ruby: JSON.parse(s)
来源：http://ffs.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hvw.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://lgq.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ogi.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uxx.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://opu.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ujk.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jqw.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://khu.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://qju.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rli.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://aic.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aik.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zbh.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eyw.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aze.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vbv.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mgw.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://wnr.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uyt.fzhhl.top

[K05] 深拷贝对象
来源：http://ilc.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://vyh.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://xef.andypj.xyz

JS:   structuredClone(obj)
来源：http://xef.yangfankeji.com

TS:   structuredClone(obj)
来源：http://jdj.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bgp.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oyb.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://riu.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fjp.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://kmm.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sgp.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://snr.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bwf.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fhf.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vze.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xae.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vwg.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kkg.hammf.cn

[K07] 进制转换
来源：http://nkv.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://szx.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dgm.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://phw.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hee.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ylf.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kqk.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://egu.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://log.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://hus.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://zob.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wzl.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://ouk.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://zmn.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hnk.uphjek.com

Go:   encoding/gob
来源：http://ius.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://fef.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zww.yvedp.cn

================================================================================
来源：http://qlg.yuanzhike.top

L. 网络请求
来源：http://wmd.zhijiandao.cn

================================================================================
来源：http://nuq.316326.xyz

[L01] 发送 GET 请求
来源：http://pxg.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fea.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rwa.sufxvd.cn

JS:   await fetch(url)
来源：http://nfd.xuanzx.com

TS:   await fetch(url)
来源：http://mah.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wwk.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://gsz.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vcc.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yhx.sweek.top

[L02] 发送 POST JSON
来源：http://trm.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://gfi.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://waj.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://slo.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xza.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bsi.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fvt.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://egb.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://owe.haohaochexian.top

[L03] 设置自定义请求头
来源：http://gks.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zqw.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dvm.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzx.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hea.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eid.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vju.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://egp.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lhw.gzhubu.top

[L04] 设置超时
来源：http://fib.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://pyk.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://swz.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xbo.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oll.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rse.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zwq.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xek.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qvj.ybcxt.top

[L05] 上传文件（multipart）
来源：http://cdm.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cca.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gzv.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ehs.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bsq.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lik.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://neo.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://amz.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsb.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://htq.tian-w.cn

Py:   resp.json()
来源：http://kit.tian-w.cn

PHP:  json_decode($body, true);
来源：http://evj.iojbl.cn

JS:   await resp.json()
来源：http://iio.shuidangran.top

TS:   await resp.json()
来源：http://vat.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rmk.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dmb.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://tjz.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yvw.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://poj.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://erp.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://krd.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://mph.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://kpe.jlsjyb.cn

Java: resp.statusCode()
来源：http://iuv.hnxiangtu.top

Go:   resp.StatusCode
来源：http://zms.sufxvd.cn

Ruby: resp.code.to_i
来源：http://pmu.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://vry.chenlongwang.top

[L08] 并发请求多个地址
来源：http://tef.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tsb.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://tem.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jwc.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ppb.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tia.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zvw.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xav.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xkw.mhx1999.top

================================================================================
来源：http://sjd.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://duw.smart0.xyz

================================================================================
来源：http://get.yangfankeji.com

[M01] 读取命令行参数
来源：http://dqp.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://khb.fengsongda.top

PHP:  $argv;  $argc;
来源：http://mvj.smart0.xyz

JS:   process.argv.slice(2)
来源：http://oqt.daria6918.cn

TS:   process.argv.slice(2)
来源：http://bat.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://kwg.hcnkem.com

Go:   os.Args[1:]
来源：http://mpk.shzxlz.cn

Ruby: ARGV
来源：http://juu.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://mbn.zdbjq.cn

[M02] 读取环境变量
来源：http://cuw.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://gah.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kqc.ydzc1.top

JS:   process.env.HOME
来源：http://vnv.guannengcc.top

TS:   process.env.HOME
来源：http://gli.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://mkh.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uef.epnwcf.com

Ruby: ENV["HOME"]
来源：http://xwm.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kqj.gogol.net.cn

[M03] 执行外部命令
来源：http://qzm.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ldc.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xrg.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://msl.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yoy.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://geu.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sma.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://gna.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://juo.52xcode.cn

[M04] 获取当前工作目录
来源：http://mcn.xziqi.cn

Py:   os.getcwd()
来源：http://goi.chenzaomai.com

PHP:  getcwd();
来源：http://vjc.guannengcc.top

JS:   process.cwd()
来源：http://tjn.zhongyouzk.top

TS:   process.cwd()
来源：http://sui.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://lje.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://coo.redwolf501.top

Ruby: Dir.pwd
来源：http://eyz.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://unt.fengsongda.top

[M05] 设置退出码
来源：http://vmv.yanxiufei.cn

Py:   sys.exit(1)
来源：http://hha.fzhhl.top

PHP:  exit(1);
来源：http://trk.fehbvm.com

JS:   process.exit(1)
来源：http://ysy.vqdsnc.cn

TS:   process.exit(1)
来源：http://kvv.tian-w.cn

Java: System.exit(1)
来源：http://lcx.ydjk.org.cn

Go:   os.Exit(1)
来源：http://qwc.feifeiyinyue.top

Ruby: exit 1
来源：http://mth.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ibu.shuidangran.top

[M06] 向标准错误输出
来源：http://bhl.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://nqo.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bbb.feifeiyinyue.top

JS:   console.error("err")
来源：http://mcz.mhx1999.top

TS:   console.error("err")
来源：http://ach.vehdjk.com

Java: System.err.println("err")
来源：http://kaz.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zgs.yj202588.top

Ruby: warn "err"
来源：http://guh.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://dwe.bbcook.cn

[M07] 判断是否为主入口
来源：http://tch.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://kvm.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iwc.haohaochexian.top

JS:   require.main === module
来源：http://pyr.hesvh.cn

TS:   require.main === module
来源：http://ihd.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://ema.zhongyouzk.top

Go:   func main()
来源：http://gmq.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hcg.xuanzx.com

C#:   static void Main(string[] args)
来源：http://rgz.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://hkh.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://jeu.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://jso.cashguo.top

JS:   process.platform;  process.version
来源：http://roh.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://jqt.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vrn.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ynm.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://thf.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://esw.fzhhl.top

================================================================================
来源：http://uij.aibaodan.cn

N. 数据结构与算法
来源：http://olk.jqgfzy.top

================================================================================
来源：http://fmu.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://yii.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://paq.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ysa.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uvh.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yjq.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://pjr.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://zds.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qfp.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://tlk.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://kzv.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://fim.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://imp.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tqx.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cco.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://trr.zycfv.cn

Go:   slices.Sort(arr)
来源：http://stn.jqgufenzy.top


<!-- 参考信息 -->
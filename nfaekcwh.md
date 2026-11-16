代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://drl.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://oxr.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ysp.yj20258888.top

[J06] 计算两时间之差
来源：http://alb.hammf.cn

Py:   (end - start).total_seconds()
来源：http://drm.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://gqo.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gst.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lea.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://yxr.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://ber.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://ieq.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://uak.hysaishi.cn

[J07] 比较两个日期
来源：http://ucu.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://oce.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tah.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://mdh.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://lsz.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qjz.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lpu.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://fiq.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://lhh.chenzaomai.com

[J08] 提取年月日与星期
来源：http://qiu.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://smy.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dcf.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tuv.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xtc.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://izl.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jkp.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://obk.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pup.xylfe.cn

[J09] 时区处理
来源：http://kxq.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jlz.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wqy.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mgt.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jil.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://adl.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vgj.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zjr.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eug.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://nlr.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uop.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zvz.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yjx.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fkq.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zwp.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uxi.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rlo.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mpy.ywan-chungtsiang.top

================================================================================
来源：http://tpg.cashguo.top

K. JSON 与序列化
来源：http://api.9152youxi.cn

================================================================================
来源：http://qts.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://iwm.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vnh.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kop.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://arw.birdmap.top

TS:   JSON.stringify(obj)
来源：http://uiv.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://asu.yj20258888.top

Go:   json.Marshal(obj)
来源：http://klr.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zsf.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://shl.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://syo.yonumen.top

Py:   json.loads(s)
来源：http://lkq.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://paf.aibaodan.cn

JS:   JSON.parse(s)
来源：http://hdh.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://kow.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fxd.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://xaq.daxiang520.top

Ruby: JSON.parse(s)
来源：http://erf.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vld.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://lnt.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qca.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pxj.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xqa.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cqg.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lmt.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rwi.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dny.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yiv.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://vcx.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qsy.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yho.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rzx.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hcv.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://okc.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tpx.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kgn.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cjp.ydzc1.top

[K05] 深拷贝对象
来源：http://mti.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://rny.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://peo.zhengqikj.top

JS:   structuredClone(obj)
来源：http://jht.dianchejie.cn

TS:   structuredClone(obj)
来源：http://uxp.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://cam.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kwu.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://anw.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bpu.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://fot.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://all.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uav.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rhv.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kls.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cep.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnc.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://asu.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://izn.xylfe.cn

[K07] 进制转换
来源：http://wns.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eec.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rzu.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eyg.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lwn.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vwx.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xmo.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ytd.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vch.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://rcr.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://vrg.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://atm.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://ntq.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://kij.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yom.ctjpmb.com

Go:   encoding/gob
来源：http://qwj.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://pwl.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qhv.guannengcc.top

================================================================================
来源：http://nqq.jianghu66.top

L. 网络请求
来源：http://ers.yongpay.top

================================================================================
来源：http://icg.yangfankeji.com

[L01] 发送 GET 请求
来源：http://cji.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yfm.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ooc.cashguo.top

JS:   await fetch(url)
来源：http://boe.sufxvd.cn

TS:   await fetch(url)
来源：http://qhl.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ekn.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://bxr.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uke.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xzu.ppjwa.cn

[L02] 发送 POST JSON
来源：http://hdc.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tvy.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xlw.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvi.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cct.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uec.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fcp.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bgp.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rpn.yfazqb.com

[L03] 设置自定义请求头
来源：http://jod.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sql.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oge.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uom.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqg.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://etp.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://spx.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wnp.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wtk.tianlin.xyz

[L04] 设置超时
来源：http://xkz.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://amu.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kpp.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvj.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tta.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xhn.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gnn.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vct.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqw.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://dxo.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dne.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://odu.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://umv.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jlf.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kwx.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dig.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zqe.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zfg.xylfe.cn

[L06] 解析响应为 JSON
来源：http://ldw.cashguo.top

Py:   resp.json()
来源：http://xoo.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://gqw.vehdjk.com

JS:   await resp.json()
来源：http://isg.ctjpmb.com

TS:   await resp.json()
来源：http://nkm.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jno.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yor.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://tnn.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rxs.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://mjf.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fpj.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wfr.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://frr.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://slb.sufxvd.cn

Java: resp.statusCode()
来源：http://tlz.tarul.cn

Go:   resp.StatusCode
来源：http://pch.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://vwh.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://jjq.0kj1m.cn

[L08] 并发请求多个地址
来源：http://qfg.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mwq.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://dak.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uey.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yts.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uma.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jmm.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://var.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ica.tianlin.xyz

================================================================================
来源：http://mbc.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://jbb.ehwqpu.com

================================================================================
来源：http://svt.gogol.net.cn

[M01] 读取命令行参数
来源：http://vap.smart0.xyz

Py:   sys.argv[1:]
来源：http://dsy.yvedp.cn

PHP:  $argv;  $argc;
来源：http://fnd.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://prt.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://zev.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://odw.ctjpmb.com

Go:   os.Args[1:]
来源：http://kgi.jlsjyb.cn

Ruby: ARGV
来源：http://vvf.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://wey.yuxming.cn

[M02] 读取环境变量
来源：http://kip.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://pzk.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://glv.pycfn.com

JS:   process.env.HOME
来源：http://tae.jinqigufen.top

TS:   process.env.HOME
来源：http://uwa.yj20258.top

Java: System.getenv("HOME")
来源：http://yyz.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aku.cheryme.top

Ruby: ENV["HOME"]
来源：http://qjq.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zhx.ehwqpu.com

[M03] 执行外部命令
来源：http://pkq.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sag.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zrm.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gre.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://czz.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://las.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ejt.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nyu.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://hbf.shzxlz.cn

[M04] 获取当前工作目录
来源：http://krn.sxryk.cn

Py:   os.getcwd()
来源：http://vld.yonumen.top

PHP:  getcwd();
来源：http://jpy.quarkkingdee.top

JS:   process.cwd()
来源：http://ihw.0kj1m.cn

TS:   process.cwd()
来源：http://tay.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://sdg.9152youxi.cn

Go:   os.Getwd()
来源：http://ezo.tian-w.cn

Ruby: Dir.pwd
来源：http://tyi.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://hon.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://riv.hysaishi.cn

Py:   sys.exit(1)
来源：http://wrr.xuetiantiany.cn

PHP:  exit(1);
来源：http://amk.sysykeji.top

JS:   process.exit(1)
来源：http://fhm.fengsongda.top

TS:   process.exit(1)
来源：http://fac.sjlbkw.cn

Java: System.exit(1)
来源：http://iqb.hesvh.cn

Go:   os.Exit(1)
来源：http://lbw.hywenlv.cn

Ruby: exit 1
来源：http://mft.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cnd.bbcook.cn

[M06] 向标准错误输出
来源：http://vky.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://oct.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bth.shanyushiyangtech.top

JS:   console.error("err")
来源：http://hxd.chenzaomai.com

TS:   console.error("err")
来源：http://gar.jiagoushi.top

Java: System.err.println("err")
来源：http://nfa.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rnp.cheryme.top

Ruby: warn "err"
来源：http://xco.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://kov.tarul.cn

[M07] 判断是否为主入口
来源：http://zxc.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://tug.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tku.nanxuanxn.top

JS:   require.main === module
来源：http://xge.wangshuangyany.cn

TS:   require.main === module
来源：http://yyr.yfazqb.com

Java: public static void main(String[] args)
来源：http://vtu.yueranfly.top

Go:   func main()
来源：http://bsh.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fnc.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://jxi.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://jej.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://umb.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://cgh.jyoumei.cn

JS:   process.platform;  process.version
来源：http://tff.zhengqikj.top

TS:   process.platform;  process.version
来源：http://btw.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://geg.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ksu.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aqy.yj20258.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qoh.sxryk.cn

================================================================================
来源：http://ing.meibo888.top

N. 数据结构与算法
来源：http://lng.fzhhl.top

================================================================================
来源：http://knh.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://ieo.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ntm.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vrb.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndk.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://soi.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://nog.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://zqr.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://osg.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://htl.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://mzq.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://rcz.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wvr.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://keu.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://for.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tvq.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://rer.yvedp.cn

Ruby: arr.sort
来源：http://bsr.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://thd.uphjek.com

[N03] 快速排序（分治示例）
来源：http://cnb.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wgo.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://ypw.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzz.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jlk.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cid.ivvv.top


<!-- 参考信息 -->
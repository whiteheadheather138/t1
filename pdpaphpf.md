代发 wailian999

Py:   (end - start).total_seconds()
来源：http://nyq.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://btj.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jzm.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gmd.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fgc.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://vkz.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://jjg.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://iuv.zdqjudy.top

[J07] 比较两个日期
来源：http://cri.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://bhi.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zct.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://uyx.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vtc.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xmk.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ftw.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lsq.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://uqq.smart0.xyz

[J08] 提取年月日与星期
来源：http://mdr.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://euq.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ypr.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ptl.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ltg.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yua.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wym.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://grd.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fja.mhx1999.top

[J09] 时区处理
来源：http://veo.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qzl.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lsc.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlx.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npq.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ssc.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aic.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gqf.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mvc.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://mkf.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xrq.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ozg.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iam.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wew.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bar.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uiq.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://isp.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tuw.zhiwuduotai.top

================================================================================
来源：http://ikc.yfazqb.com

K. JSON 与序列化
来源：http://tni.andypj.xyz

================================================================================
来源：http://ygf.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://ozf.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://szf.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lmz.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://zwk.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://wxf.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tso.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://ana.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://mjo.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://wca.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://kwd.yongpay.top

Py:   json.loads(s)
来源：http://smd.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sst.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://ahh.gotoacloud.top

TS:   JSON.parse(s)
来源：http://cfq.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fpl.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://nph.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://byf.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://plk.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://zur.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://owp.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ofq.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ocq.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gga.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://udy.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hda.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://kta.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uof.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://end.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qem.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pdt.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://glv.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdr.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qvc.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lyz.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://aed.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gym.uphjek.com

[K05] 深拷贝对象
来源：http://lcg.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://adg.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://pps.iojbl.cn

JS:   structuredClone(obj)
来源：http://ydq.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://unc.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lqv.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://feb.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cap.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://guv.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://fxb.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rnx.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lyc.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bjr.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpr.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wtg.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://bxi.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fuk.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cny.zhongyouzk.top

[K07] 进制转换
来源：http://wmi.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nny.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rld.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vzw.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://svh.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pvi.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://scb.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iyg.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mts.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://hih.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://tfb.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bvl.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://gtk.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://kxu.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qpd.jqgfzy.top

Go:   encoding/gob
来源：http://kdr.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://iyl.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jer.jinqigfzy.top

================================================================================
来源：http://qvp.yj20258.top

L. 网络请求
来源：http://csx.pycfn.com

================================================================================
来源：http://lrj.9152youxi.cn

[L01] 发送 GET 请求
来源：http://xbk.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://svf.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://akx.jyoumei.cn

JS:   await fetch(url)
来源：http://dgi.hesvh.cn

TS:   await fetch(url)
来源：http://qmp.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://elt.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://vbq.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vhs.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lxc.c1oappe.top

[L02] 发送 POST JSON
来源：http://rjj.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pxf.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://try.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpd.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cuk.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nfe.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dui.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gch.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jdn.zdqjudy.top

[L03] 设置自定义请求头
来源：http://qer.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zbh.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zxc.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzr.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baf.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wcl.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yyc.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://chu.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kgh.zhoulong.xyz

[L04] 设置超时
来源：http://trj.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://nfd.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yzr.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwm.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xvt.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ldm.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eoe.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ngf.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ubk.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://mpc.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jki.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cmc.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xof.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eep.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ihv.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cry.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zja.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sfx.havefunace.top

[L06] 解析响应为 JSON
来源：http://cwc.kuanghao11.cn

Py:   resp.json()
来源：http://shp.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://atb.aibaodan.cn

JS:   await resp.json()
来源：http://cau.nanxinkj.top

TS:   await resp.json()
来源：http://voo.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bgg.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ase.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://sxl.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hbf.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://enf.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kmv.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fcu.hammf.cn

JS:   resp.ok;  resp.status
来源：http://lxw.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://dgs.gzhubu.top

Java: resp.statusCode()
来源：http://wrn.hesvh.cn

Go:   resp.StatusCode
来源：http://taj.smart0.xyz

Ruby: resp.code.to_i
来源：http://lyh.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://jnl.yfazqb.com

[L08] 并发请求多个地址
来源：http://ocq.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://knl.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://zrt.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmb.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mqf.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uqa.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xmm.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jee.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yql.yueranfly.top

================================================================================
来源：http://eol.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://zzo.cashguo.top

================================================================================
来源：http://nae.hammf.cn

[M01] 读取命令行参数
来源：http://qqd.guannengcc.top

Py:   sys.argv[1:]
来源：http://ovl.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://jpg.fengsongda.top

JS:   process.argv.slice(2)
来源：http://suv.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://spv.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://yvo.jlsjyb.cn

Go:   os.Args[1:]
来源：http://vvp.daxiang520.top

Ruby: ARGV
来源：http://fzi.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://yoe.zycfv.cn

[M02] 读取环境变量
来源：http://qhz.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://blo.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ezh.zycfv.cn

JS:   process.env.HOME
来源：http://jth.wangdashe.top

TS:   process.env.HOME
来源：http://jck.xinyue.icu

Java: System.getenv("HOME")
来源：http://svg.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://btq.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://zxa.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tba.cheryme.top

[M03] 执行外部命令
来源：http://mvu.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wpv.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ywt.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kwc.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rqx.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wsb.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wyx.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://hvg.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://gux.zhixingplan.top

[M04] 获取当前工作目录
来源：http://rgg.guowangkeji.top

Py:   os.getcwd()
来源：http://brm.shanyushiyangtech.top

PHP:  getcwd();
来源：http://exx.jqgfzy.top

JS:   process.cwd()
来源：http://ajv.guannengcc.top

TS:   process.cwd()
来源：http://drd.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://qfs.smart0.xyz

Go:   os.Getwd()
来源：http://ffk.shuidangran.top

Ruby: Dir.pwd
来源：http://fvt.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sce.sxryk.cn

[M05] 设置退出码
来源：http://lta.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://hyg.yonumen.top

PHP:  exit(1);
来源：http://pxs.sjlbkw.cn

JS:   process.exit(1)
来源：http://qtf.svipenyu.cn

TS:   process.exit(1)
来源：http://uus.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://dix.epnwcf.com

Go:   os.Exit(1)
来源：http://mcx.yvedp.cn

Ruby: exit 1
来源：http://ijm.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mae.snrcjt.cn

[M06] 向标准错误输出
来源：http://xus.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://drc.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qyb.tarul.cn

JS:   console.error("err")
来源：http://oab.hnqzz.top

TS:   console.error("err")
来源：http://mhx.hfpthk.cn

Java: System.err.println("err")
来源：http://kas.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iet.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://xkb.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://hap.cucudq.cn

[M07] 判断是否为主入口
来源：http://don.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://gsa.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bgp.jinqigfzy.top

JS:   require.main === module
来源：http://ypu.daxiang520.top

TS:   require.main === module
来源：http://esy.daxiang520.top

Java: public static void main(String[] args)
来源：http://jza.yangfankeji.com

Go:   func main()
来源：http://rgj.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zin.ydzc1.top

C#:   static void Main(string[] args)
来源：http://lvh.pycfn.com

[M08] 获取系统与运行时信息
来源：http://wce.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://bxf.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://yhw.zhengqikj.top

JS:   process.platform;  process.version
来源：http://pue.zdqjudy.top

TS:   process.platform;  process.version
来源：http://shb.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xfe.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ekr.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aoj.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wxi.hnqzz.top

================================================================================
来源：http://ywg.redwolf501.top

N. 数据结构与算法
来源：http://vhh.uphjek.com

================================================================================
来源：http://ugf.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://mvv.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://cnh.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pjs.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xzw.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lri.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://cdv.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://hcq.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lte.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://ixy.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://ryo.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://skt.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iex.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vvk.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mhf.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fcf.aizwys.cn

Go:   slices.Sort(arr)
来源：http://rwv.zycfv.cn

Ruby: arr.sort
来源：http://hmc.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kol.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://mzi.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ptj.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://baw.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eay.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://img.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zwa.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nop.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xmj.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://vle.epnwcf.com

[N04] 斐波那契数列
来源：http://uee.jyoumei.cn


<!-- 参考信息 -->
代发 wailian999

Py:   (end - start).total_seconds()
来源：http://jcw.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://bki.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fag.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ogj.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://mhj.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://fqa.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://bgm.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://ccq.hongshengwenyu.top

[J07] 比较两个日期
来源：http://lna.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://hgb.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yyz.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hmh.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://whl.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://too.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kkj.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://trs.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://lxs.yonumen.top

[J08] 提取年月日与星期
来源：http://tta.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ano.yangfankeji.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kuh.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xwe.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xlc.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lhl.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hzp.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mwt.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wbk.kuanghao11.cn

[J09] 时区处理
来源：http://pgz.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ffw.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ojv.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sag.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tgy.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://liq.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://khw.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://anb.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ssr.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://mal.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://phq.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yqf.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fph.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fch.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cox.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fcc.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fqb.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hil.hongshengwenyu.top

================================================================================
来源：http://weh.shuidangran.top

K. JSON 与序列化
来源：http://vcv.wangshuangyany.cn

================================================================================
来源：http://qao.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://wxg.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://drn.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tjs.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://vpa.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://cfj.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vnu.andypj.xyz

Go:   json.Marshal(obj)
来源：http://pze.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dpq.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oot.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://mpe.xuetiantiany.cn

Py:   json.loads(s)
来源：http://mzl.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ypz.hywenlv.cn

JS:   JSON.parse(s)
来源：http://uhs.chenlongwang.top

TS:   JSON.parse(s)
来源：http://aha.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fln.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://twg.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://mcy.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://omj.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://ndq.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iiz.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vbb.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zpc.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xij.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ugg.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ktz.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://aic.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aft.yuxming.cn

[K04] 读取 JSON 文件
来源：http://chn.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hty.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ase.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yup.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvh.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qqf.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rnq.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jnk.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://psf.mhx1999.top

[K05] 深拷贝对象
来源：http://yew.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://dby.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://dzh.xylfe.cn

JS:   structuredClone(obj)
来源：http://bsl.0kj1m.cn

TS:   structuredClone(obj)
来源：http://fok.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fvw.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nig.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iaz.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lfi.yongpay.top

[K06] 解析 URL 查询串
来源：http://egs.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pkc.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mzn.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yrg.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmi.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fxg.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mlr.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uun.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ozx.hnqzz.top

[K07] 进制转换
来源：http://taq.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ywv.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://chy.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hpq.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lij.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fxn.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ebn.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pul.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ipv.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dei.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://frq.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bwc.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://did.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://dru.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dcv.vqdsnc.cn

Go:   encoding/gob
来源：http://lml.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://woa.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dyj.gaohongyu789.top

================================================================================
来源：http://lwv.xinyue.icu

L. 网络请求
来源：http://vvd.uphjek.com

================================================================================
来源：http://vvc.ctjpmb.com

[L01] 发送 GET 请求
来源：http://yeq.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mbc.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjy.yuanzhike.top

JS:   await fetch(url)
来源：http://aiq.gzhubu.top

TS:   await fetch(url)
来源：http://iku.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xhp.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://ukg.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pxm.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fkh.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://ylx.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://gyu.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mfv.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://irg.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cme.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gaz.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://msy.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xsq.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xss.daxiang520.top

[L03] 设置自定义请求头
来源：http://lqw.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zzd.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tgg.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gme.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gul.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xgg.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fdx.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tnf.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yvo.ppjwa.cn

[L04] 设置超时
来源：http://mrw.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://qhk.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vcs.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uij.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aqf.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzt.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://arp.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sju.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mec.guannengcc.top

[L05] 上传文件（multipart）
来源：http://znx.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://exl.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://npu.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tmq.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lqg.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://crv.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gey.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://prh.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tqi.bbcook.cn

[L06] 解析响应为 JSON
来源：http://uxu.yj20258.top

Py:   resp.json()
来源：http://rrw.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://okc.52xcode.cn

JS:   await resp.json()
来源：http://exm.shanyushiyangtech.top

TS:   await resp.json()
来源：http://rta.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gfn.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://usw.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://vhp.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pkc.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://rto.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ovf.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fnj.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://osc.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://ofi.ydzc1.top

Java: resp.statusCode()
来源：http://yea.smart0.xyz

Go:   resp.StatusCode
来源：http://cts.chenzaomai.com

Ruby: resp.code.to_i
来源：http://ccm.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://emn.shuidangran.top

[L08] 并发请求多个地址
来源：http://tod.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lhc.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://jim.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ley.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qhz.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pwp.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eue.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rur.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bsp.9152youxi.cn

================================================================================
来源：http://erv.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://cpr.pycfn.com

================================================================================
来源：http://kgr.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://omt.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://tqa.aizwys.cn

PHP:  $argv;  $argc;
来源：http://wdd.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://rrb.sysykeji.top

TS:   process.argv.slice(2)
来源：http://khk.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://niq.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://fed.pengpengdd.cyou

Ruby: ARGV
来源：http://wam.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://ljh.yj202588.top

[M02] 读取环境变量
来源：http://fal.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://wen.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ejj.hongshengwenyu.top

JS:   process.env.HOME
来源：http://ntp.meibo888.top

TS:   process.env.HOME
来源：http://bai.sufxvd.cn

Java: System.getenv("HOME")
来源：http://zlq.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://err.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://xft.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ifi.hongshengwenyu.top

[M03] 执行外部命令
来源：http://meb.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mcu.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sou.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://btd.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://iuu.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pdk.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lko.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://obf.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://svm.zycfv.cn

[M04] 获取当前工作目录
来源：http://giz.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://ehi.shangyingyoupin.top

PHP:  getcwd();
来源：http://kfq.hammf.cn

JS:   process.cwd()
来源：http://ocs.shanyushiyangtech.top

TS:   process.cwd()
来源：http://nbc.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://mut.kuanghao11.cn

Go:   os.Getwd()
来源：http://vgd.fzhhl.top

Ruby: Dir.pwd
来源：http://qom.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vvt.hfpthk.cn

[M05] 设置退出码
来源：http://mbb.gzhubu.top

Py:   sys.exit(1)
来源：http://xwz.zycfv.cn

PHP:  exit(1);
来源：http://jub.jiagoushi.top

JS:   process.exit(1)
来源：http://hkj.jianghu66.top

TS:   process.exit(1)
来源：http://vxg.tarul.cn

Java: System.exit(1)
来源：http://vnw.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://qqn.yvedp.cn

Ruby: exit 1
来源：http://xkx.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ghx.andypj.xyz

[M06] 向标准错误输出
来源：http://qgf.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://glr.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qov.andypj.xyz

JS:   console.error("err")
来源：http://lhi.yvedp.cn

TS:   console.error("err")
来源：http://ygp.hfpthk.cn

Java: System.err.println("err")
来源：http://vbu.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ffj.zdqjudy.top

Ruby: warn "err"
来源：http://puf.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://kzr.yongpay.top

[M07] 判断是否为主入口
来源：http://fih.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://wwr.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dku.yanxiufei.cn

JS:   require.main === module
来源：http://vfe.c1oappe.top

TS:   require.main === module
来源：http://qwy.andypj.xyz

Java: public static void main(String[] args)
来源：http://psr.0kj1m.cn

Go:   func main()
来源：http://ecq.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ugc.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://rsf.316326.xyz

[M08] 获取系统与运行时信息
来源：http://xuy.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://jtm.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://yqt.birdmap.top

JS:   process.platform;  process.version
来源：http://fte.hnqzz.top

TS:   process.platform;  process.version
来源：http://mcz.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ugs.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://lqr.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yog.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fom.hysaishi.cn

================================================================================
来源：http://lbo.gotoacloud.top

N. 数据结构与算法
来源：http://rgr.sufxvd.cn

================================================================================
来源：http://mnt.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://gmg.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://zxp.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rcb.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ige.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://boi.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://xio.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://wse.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gre.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dhw.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://spw.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://wbx.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ost.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tlt.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sug.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yhd.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://zel.tanke756.top

Ruby: arr.sort
来源：http://fje.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://btx.tanke756.top

[N03] 快速排序（分治示例）
来源：http://npo.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uop.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://wne.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oci.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzh.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rat.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uzd.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xcl.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ssv.yj20258888.top

[N04] 斐波那契数列
来源：http://qck.yuanzhike.top


<!-- 参考信息 -->
代发 wailian999

Py:   (end - start).total_seconds()
来源：http://ase.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://vwu.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xlo.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rck.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://sve.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://rre.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://qsv.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://lrl.daria6918.cn

[J07] 比较两个日期
来源：http://lbh.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://dqq.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ghr.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://nuv.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://kdp.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://atc.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mph.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://mfr.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://tzb.hysaishi.cn

[J08] 提取年月日与星期
来源：http://cow.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qmz.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yba.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nbi.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hie.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hka.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://msd.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xee.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://edc.shanyushiyangtech.top

[J09] 时区处理
来源：http://sud.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kfv.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vpq.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sqe.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nrh.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bzr.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rud.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fnj.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gow.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://gjf.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://scy.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://suc.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cfi.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://agn.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gpu.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://teb.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://snq.zhiwuduotai.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://irq.cqqwz.cn

================================================================================
来源：http://ame.nanxuanxn.top

K. JSON 与序列化
来源：http://jmz.bjfxy.top

================================================================================
来源：http://jkw.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://yhv.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ffb.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lhh.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://lvl.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://ijc.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kls.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://kbc.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://afj.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hqy.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://sif.nanxuanxn.top

Py:   json.loads(s)
来源：http://dwt.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dko.jiagoushi.top

JS:   JSON.parse(s)
来源：http://wbr.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://xbk.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlg.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://yoq.xuanzx.com

Ruby: JSON.parse(s)
来源：http://gdx.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://woa.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://quc.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pfo.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fdh.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wau.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://crn.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zty.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ezg.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://xxv.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qzl.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://mus.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cag.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zoy.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lmt.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rqr.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qpb.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cbt.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://khl.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ptm.yangfankeji.com

[K05] 深拷贝对象
来源：http://ioo.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://jkz.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://thx.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://xwd.aizwys.cn

TS:   structuredClone(obj)
来源：http://agb.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fhf.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sgs.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wph.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tos.uphjek.com

[K06] 解析 URL 查询串
来源：http://rrp.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kni.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://shd.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bss.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qnc.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qwr.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://rxu.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fma.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lin.xuanzx.com

[K07] 进制转换
来源：http://xfn.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://utb.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qzi.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iby.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xgq.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nuv.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ksy.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ifb.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uxu.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://iav.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://nlu.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vwj.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ota.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://fmz.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ehg.ivvv.top

Go:   encoding/gob
来源：http://llh.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://xin.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fcq.hammf.cn

================================================================================
来源：http://ayv.sjlbkw.cn

L. 网络请求
来源：http://pwi.316326.xyz

================================================================================
来源：http://wni.ivvv.top

[L01] 发送 GET 请求
来源：http://cmg.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kpa.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgt.nwbrower.top

JS:   await fetch(url)
来源：http://uuw.yongpay.top

TS:   await fetch(url)
来源：http://uxp.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xsm.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://wxj.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wxn.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kot.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://hua.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ici.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hig.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jwu.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ecw.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ulg.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qwn.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tll.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zqd.cashguo.top

[L03] 设置自定义请求头
来源：http://nbb.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oee.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://app.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emb.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://amv.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jja.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gct.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hzv.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hzi.iojbl.cn

[L04] 设置超时
来源：http://ujr.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://unn.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lfp.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eny.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nri.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uct.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hsw.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://utp.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zqp.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://eal.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rjf.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://duu.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://swi.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pwn.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dxd.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://klr.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kyo.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qci.yj20258888.top

[L06] 解析响应为 JSON
来源：http://apd.sxryk.cn

Py:   resp.json()
来源：http://tyl.redwolf501.top

PHP:  json_decode($body, true);
来源：http://uar.jinqigufen.top

JS:   await resp.json()
来源：http://cfs.tian-w.cn

TS:   await resp.json()
来源：http://zvb.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://juo.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hkc.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://hjx.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mvh.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://rwp.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jcv.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upg.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://amx.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://mnc.tarul.cn

Java: resp.statusCode()
来源：http://pza.sweek.top

Go:   resp.StatusCode
来源：http://fdu.guowangkeji.top

Ruby: resp.code.to_i
来源：http://seo.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://eck.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://ghc.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lwl.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://zpb.tarul.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgs.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wgo.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://khy.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oxt.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sfd.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://thc.yongpay.top

================================================================================
来源：http://fey.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://yrj.zhengqikj.top

================================================================================
来源：http://gqk.shzxlz.cn

[M01] 读取命令行参数
来源：http://lhh.cqqwz.cn

Py:   sys.argv[1:]
来源：http://ejm.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://hni.tanke756.top

JS:   process.argv.slice(2)
来源：http://kjh.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://igi.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://izz.sweek.top

Go:   os.Args[1:]
来源：http://xkg.xuetiantiany.cn

Ruby: ARGV
来源：http://uft.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://hcx.daria6918.cn

[M02] 读取环境变量
来源：http://gjz.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://hfc.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://phu.yj20258888.top

JS:   process.env.HOME
来源：http://gin.quarkkingdee.top

TS:   process.env.HOME
来源：http://hgo.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://pxn.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vli.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://vdt.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obe.ctjpmb.com

[M03] 执行外部命令
来源：http://mym.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sdv.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iuw.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kcq.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://snn.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lav.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ksk.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rvq.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://ywp.snrcjt.cn

[M04] 获取当前工作目录
来源：http://yek.shangyingyoupin.top

Py:   os.getcwd()
来源：http://guh.hnqzz.top

PHP:  getcwd();
来源：http://rnr.hnxiangtu.top

JS:   process.cwd()
来源：http://tqa.guowangkeji.top

TS:   process.cwd()
来源：http://lqb.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://ltu.sysykeji.top

Go:   os.Getwd()
来源：http://lui.quarkkingdee.top

Ruby: Dir.pwd
来源：http://ren.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://idq.kuanghao11.cn

[M05] 设置退出码
来源：http://gjo.jinqigufen.top

Py:   sys.exit(1)
来源：http://gdk.yj20258.top

PHP:  exit(1);
来源：http://dqe.sysykeji.top

JS:   process.exit(1)
来源：http://ibg.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://czm.cdnleiting.top

Java: System.exit(1)
来源：http://soa.sufxvd.cn

Go:   os.Exit(1)
来源：http://azg.jianghu66.top

Ruby: exit 1
来源：http://yrd.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://srx.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://nox.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://zjc.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://eko.fehbvm.com

JS:   console.error("err")
来源：http://add.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://rox.bjfxy.top

Java: System.err.println("err")
来源：http://oti.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xjq.quarkkingdee.top

Ruby: warn "err"
来源：http://rol.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://kom.hysaishi.cn

[M07] 判断是否为主入口
来源：http://cnr.pycfn.com

Py:   if __name__ == "__main__":
来源：http://rop.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pse.chenzaomai.com

JS:   require.main === module
来源：http://fix.cqqwz.cn

TS:   require.main === module
来源：http://ldt.dianchejie.cn

Java: public static void main(String[] args)
来源：http://rmq.zdbjq.cn

Go:   func main()
来源：http://qpo.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wla.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://krn.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://cng.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://sox.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://vcj.jqgfzy.top

JS:   process.platform;  process.version
来源：http://krt.shzxlz.cn

TS:   process.platform;  process.version
来源：http://ckj.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sua.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ryu.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://caq.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://auf.shzxlz.cn

================================================================================
来源：http://ubi.haohaochexian.top

N. 数据结构与算法
来源：http://rtu.tianlin.xyz

================================================================================
来源：http://fxo.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://edw.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qdw.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fis.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwb.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kyw.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://frf.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://ncz.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eir.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ans.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://xqw.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://aki.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qzr.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ept.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://usl.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sch.yuxming.cn

Go:   slices.Sort(arr)
来源：http://twz.yuanzhike.top

Ruby: arr.sort
来源：http://nhm.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://npp.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://xmc.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://epl.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://acd.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bja.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dft.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://seh.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ank.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eez.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ped.yvedp.cn

[N04] 斐波那契数列
来源：http://tay.cdnleiting.top


<!-- 参考信息 -->
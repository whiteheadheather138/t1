代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://olx.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://bdp.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://owf.zdqjudy.top

[J06] 计算两时间之差
来源：http://qpc.hammf.cn

Py:   (end - start).total_seconds()
来源：http://oyz.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://rnu.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dcw.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mzw.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://vrn.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://emp.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://lsq.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://wrr.tian-w.cn

[J07] 比较两个日期
来源：http://bgj.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ugs.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vmi.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://est.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qkl.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://two.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xnk.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://szg.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://miq.dianchejie.cn

[J08] 提取年月日与星期
来源：http://zon.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obh.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pju.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mmi.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uii.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnf.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://npy.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uea.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nst.zhijiandao.cn

[J09] 时区处理
来源：http://lvl.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fvw.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ltn.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avq.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xta.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jjl.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ywy.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://odq.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://djs.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://kch.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cgn.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aoe.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pot.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vfp.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ikr.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vcf.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://euw.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://duc.hammf.cn

================================================================================
来源：http://fmk.yuanzhike.top

K. JSON 与序列化
来源：http://rbi.shanyushiyangtech.top

================================================================================
来源：http://sol.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://zfg.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qmt.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yqy.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://kxh.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://cjz.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nwz.52xcode.cn

Go:   json.Marshal(obj)
来源：http://zxa.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://pyk.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://viv.c1oappe.top

[K02] JSON 字符串转对象
来源：http://bae.nanxuanxn.top

Py:   json.loads(s)
来源：http://guv.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bgd.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://isv.sysykeji.top

TS:   JSON.parse(s)
来源：http://ndt.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hgh.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://ghg.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://okc.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mly.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://voo.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bby.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pul.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tzz.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vxy.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://weq.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gpp.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://jes.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://scl.wangdashe.top

[K04] 读取 JSON 文件
来源：http://fuk.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ryi.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vgl.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xez.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ukn.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sfd.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lah.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nwm.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cqj.vehdjk.com

[K05] 深拷贝对象
来源：http://zsk.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://gqj.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://bgr.gotoacloud.top

JS:   structuredClone(obj)
来源：http://osk.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://icj.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ggr.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rqj.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://grn.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://twy.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://jkh.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wgj.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lpi.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ofw.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dup.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://psf.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://crv.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vzy.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ncr.chenjidiqi.icu

[K07] 进制转换
来源：http://kvj.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ocr.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ooc.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://het.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://htt.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iqm.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://frt.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oja.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vfc.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://wqc.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://qfq.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qij.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ulx.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://qey.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aog.epnwcf.com

Go:   encoding/gob
来源：http://unm.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://mjt.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lre.shanyushiyangtech.top

================================================================================
来源：http://pjp.fanxiaobao.xyz

L. 网络请求
来源：http://avy.ywan-chungtsiang.top

================================================================================
来源：http://nfy.daxiang520.top

[L01] 发送 GET 请求
来源：http://xnl.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bfc.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://npc.hammf.cn

JS:   await fetch(url)
来源：http://vvw.316326.xyz

TS:   await fetch(url)
来源：http://moc.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fki.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://ezc.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://etm.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qev.zhengqikj.top

[L02] 发送 POST JSON
来源：http://aag.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://txv.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jfw.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rxb.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kws.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bzs.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nke.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vjh.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qgk.yvedp.cn

[L03] 设置自定义请求头
来源：http://yjv.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yps.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://knk.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkq.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wmj.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tyw.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vuj.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ccu.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jip.sjlbkw.cn

[L04] 设置超时
来源：http://hms.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://liu.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ppa.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qas.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kiy.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cka.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cpr.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sem.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cbb.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://mzm.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aqi.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://anv.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nqs.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bgt.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xcp.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tpr.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://izp.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hmv.xziqi.cn

[L06] 解析响应为 JSON
来源：http://xif.andypj.xyz

Py:   resp.json()
来源：http://uwp.shuidangran.top

PHP:  json_decode($body, true);
来源：http://lvz.52xcode.cn

JS:   await resp.json()
来源：http://ryw.yueranfly.top

TS:   await resp.json()
来源：http://twt.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://poz.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://imd.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://hbp.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zwa.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://yek.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jbo.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nyw.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://qht.tarul.cn

TS:   resp.ok;  resp.status
来源：http://bow.zhengqikj.top

Java: resp.statusCode()
来源：http://cfx.shuidangran.top

Go:   resp.StatusCode
来源：http://wbx.birdmap.top

Ruby: resp.code.to_i
来源：http://azu.cheryme.top

C#:   (int)resp.StatusCode
来源：http://vax.bjfxy.top

[L08] 并发请求多个地址
来源：http://zvw.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://shs.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://kln.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://viy.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xoj.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kvp.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wmm.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://txb.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wyb.hnxiangtu.top

================================================================================
来源：http://crn.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://mhf.xylfe.cn

================================================================================
来源：http://nsr.zycfv.cn

[M01] 读取命令行参数
来源：http://rpm.ehwqpu.com

Py:   sys.argv[1:]
来源：http://cpu.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://gsx.52xcode.cn

JS:   process.argv.slice(2)
来源：http://ypt.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://svg.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://zob.mhx1999.top

Go:   os.Args[1:]
来源：http://dyc.52xcode.cn

Ruby: ARGV
来源：http://wdf.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://lqs.shzxlz.cn

[M02] 读取环境变量
来源：http://oiv.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://osj.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zpd.jianghu66.top

JS:   process.env.HOME
来源：http://hgb.sweek.top

TS:   process.env.HOME
来源：http://anv.sysykeji.top

Java: System.getenv("HOME")
来源：http://rcs.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hxe.bjfxy.top

Ruby: ENV["HOME"]
来源：http://qzz.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cur.bbcook.cn

[M03] 执行外部命令
来源：http://jcr.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ocv.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dlt.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hes.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fis.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xuq.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ubq.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://mvg.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://lcc.ppjwa.cn

[M04] 获取当前工作目录
来源：http://ixc.fktsv.cn

Py:   os.getcwd()
来源：http://ldw.nanxinkj.top

PHP:  getcwd();
来源：http://ctp.smart0.xyz

JS:   process.cwd()
来源：http://pzx.zhijiandao.cn

TS:   process.cwd()
来源：http://hvd.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://stc.gogol.net.cn

Go:   os.Getwd()
来源：http://wyx.daxiang520.top

Ruby: Dir.pwd
来源：http://afm.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ysc.hfpthk.cn

[M05] 设置退出码
来源：http://wdf.daxiang520.top

Py:   sys.exit(1)
来源：http://ckl.jinghuilouyu.cn

PHP:  exit(1);
来源：http://kff.yuxming.cn

JS:   process.exit(1)
来源：http://tbz.cucudq.cn

TS:   process.exit(1)
来源：http://lpl.cucudq.cn

Java: System.exit(1)
来源：http://qrz.tianlin.xyz

Go:   os.Exit(1)
来源：http://gsu.gotoacloud.top

Ruby: exit 1
来源：http://qce.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fqy.nwbrower.top

[M06] 向标准错误输出
来源：http://jwm.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://yqw.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fju.tian-w.cn

JS:   console.error("err")
来源：http://axx.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://jlx.jinqigfzy.top

Java: System.err.println("err")
来源：http://dhi.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eta.bjfxy.top

Ruby: warn "err"
来源：http://lsl.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://ggh.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://raf.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://ofn.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yge.redwolf501.top

JS:   require.main === module
来源：http://lfg.tian-w.cn

TS:   require.main === module
来源：http://nyz.tianlin.xyz

Java: public static void main(String[] args)
来源：http://qbk.epnwcf.com

Go:   func main()
来源：http://ccu.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qwh.daria6918.cn

C#:   static void Main(string[] args)
来源：http://iet.yj20258.top

[M08] 获取系统与运行时信息
来源：http://nqm.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://qfg.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://mis.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://llv.ehwqpu.com

TS:   process.platform;  process.version
来源：http://vxx.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wcy.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://auh.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zeo.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://osg.wangshuangyany.cn

================================================================================
来源：http://jlu.shanyushiyangtech.top

N. 数据结构与算法
来源：http://gzz.xuetiantiany.cn

================================================================================
来源：http://jfc.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://rmu.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zai.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bju.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://luc.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jos.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://gbf.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://kkg.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zrd.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ctp.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://fnx.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://zbt.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://szd.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lpx.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xzw.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ojt.cucudq.cn

Go:   slices.Sort(arr)
来源：http://dto.feifeiyinyue.top

Ruby: arr.sort
来源：http://ofa.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://lqr.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://uvf.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nea.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://hyw.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://idr.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bnk.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mpv.jqgfzy.top


<!-- 参考信息 -->
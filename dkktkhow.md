代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vjt.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://bwm.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jlv.pycfn.com

[J06] 计算两时间之差
来源：http://gxo.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://rbp.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://lsv.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ofw.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vrb.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://iyn.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://cgs.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://mfq.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://mfc.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://cmk.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://cxj.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mgz.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fcr.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://mwh.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bph.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cml.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cmv.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://sxs.snrcjt.cn

[J08] 提取年月日与星期
来源：http://ltx.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cli.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iwn.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://viw.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cqd.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://imf.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uew.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wwr.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tsu.andypj.xyz

[J09] 时区处理
来源：http://jhb.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nky.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hzm.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eve.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xdk.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yvq.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://htd.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wew.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yns.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://xbz.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mwv.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iiq.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hxc.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lbb.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qgb.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ada.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yhl.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fmo.nanxinkj.top

================================================================================
来源：http://mic.yuxming.cn

K. JSON 与序列化
来源：http://oib.pengpengdd.cyou

================================================================================
来源：http://yls.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://tfn.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iwk.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ezw.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://bfw.birdmap.top

TS:   JSON.stringify(obj)
来源：http://tko.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pet.redwolf501.top

Go:   json.Marshal(obj)
来源：http://wte.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mao.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wze.epnwcf.com

[K02] JSON 字符串转对象
来源：http://lxc.hammf.cn

Py:   json.loads(s)
来源：http://tog.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zpm.iojbl.cn

JS:   JSON.parse(s)
来源：http://txx.svipenyu.cn

TS:   JSON.parse(s)
来源：http://rvt.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vdt.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://qwb.fengsongda.top

Ruby: JSON.parse(s)
来源：http://vav.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zfy.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://qcy.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fly.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dlr.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://gih.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tcn.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xhl.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://slz.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://lac.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sei.fengsongda.top

[K04] 读取 JSON 文件
来源：http://sdz.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ifb.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://thz.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://asp.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nab.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wuy.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yui.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ric.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hwf.vqdsnc.cn

[K05] 深拷贝对象
来源：http://rhk.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://zwg.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://pey.dashuyun.cn

JS:   structuredClone(obj)
来源：http://dul.gzhubu.top

TS:   structuredClone(obj)
来源：http://uhu.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kvv.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vpp.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tcf.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://poj.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://uit.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xba.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bfr.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qga.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rqu.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ttt.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qez.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kgd.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://odu.tanke756.top

[K07] 进制转换
来源：http://ukr.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmq.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://feo.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xyz.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://itb.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gcl.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jue.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qzl.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rsc.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://pml.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://yzi.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ujb.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://oug.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://rme.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ufx.shuidangran.top

Go:   encoding/gob
来源：http://unh.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://vwf.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jln.ydjk.org.cn

================================================================================
来源：http://nwo.yj202588.top

L. 网络请求
来源：http://vts.bjfxy.top

================================================================================
来源：http://tfk.vehdjk.com

[L01] 发送 GET 请求
来源：http://uxu.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hgm.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zaw.svipenyu.cn

JS:   await fetch(url)
来源：http://sde.aibaodan.cn

TS:   await fetch(url)
来源：http://ikx.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gih.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://ybp.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tdr.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cvd.daria6918.cn

[L02] 发送 POST JSON
来源：http://kua.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://nkr.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vaf.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msj.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pok.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aii.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bme.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://smv.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gwk.ppjwa.cn

[L03] 设置自定义请求头
来源：http://jkl.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://owq.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iup.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ndu.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dou.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wvw.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bpt.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hal.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bvf.yueranfly.top

[L04] 设置超时
来源：http://iwp.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://ntt.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uqs.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gga.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dix.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://quj.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://okh.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nds.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gju.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://jmk.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://huw.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://thz.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://duq.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xes.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://owm.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bgx.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtj.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://shs.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://mgl.nwbrower.top

Py:   resp.json()
来源：http://iax.daria6918.cn

PHP:  json_decode($body, true);
来源：http://gya.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://kdj.ydzc1.top

TS:   await resp.json()
来源：http://onn.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ulf.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://msc.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://ibl.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iqx.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://aop.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zpj.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gwz.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://akt.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://qdu.yj202588.top

Java: resp.statusCode()
来源：http://vii.cdnleiting.top

Go:   resp.StatusCode
来源：http://nwn.hammf.cn

Ruby: resp.code.to_i
来源：http://bxf.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://lsk.bbcook.cn

[L08] 并发请求多个地址
来源：http://zyw.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pfl.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://zue.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijd.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmg.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zgm.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lxv.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cls.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nlc.jqgufenzy.top

================================================================================
来源：http://ngo.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://kdx.ehwqpu.com

================================================================================
来源：http://acd.316326.xyz

[M01] 读取命令行参数
来源：http://nne.jqgfzy.top

Py:   sys.argv[1:]
来源：http://fef.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://kps.gzhubu.top

JS:   process.argv.slice(2)
来源：http://qii.tarul.cn

TS:   process.argv.slice(2)
来源：http://dfw.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://uzf.ehwqpu.com

Go:   os.Args[1:]
来源：http://dcb.wangdashe.top

Ruby: ARGV
来源：http://agc.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://voq.aibaodan.cn

[M02] 读取环境变量
来源：http://qig.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://cul.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://igv.pengpengdd.cyou

JS:   process.env.HOME
来源：http://hhg.fengsongda.top

TS:   process.env.HOME
来源：http://gvx.epnwcf.com

Java: System.getenv("HOME")
来源：http://dwi.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mkn.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://jzb.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yuj.gogol.net.cn

[M03] 执行外部命令
来源：http://rtx.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vjb.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oua.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://chq.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://qvv.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qry.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ehx.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://stx.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://ibb.andypj.xyz

[M04] 获取当前工作目录
来源：http://lsv.nanxinkj.top

Py:   os.getcwd()
来源：http://kxe.sxryk.cn

PHP:  getcwd();
来源：http://olz.hnxiangtu.top

JS:   process.cwd()
来源：http://ynn.jinghuilouyu.cn

TS:   process.cwd()
来源：http://kdo.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://ydk.xinyue.icu

Go:   os.Getwd()
来源：http://txd.ybcxt.top

Ruby: Dir.pwd
来源：http://adu.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://wam.shangyingyoupin.top

[M05] 设置退出码
来源：http://vbr.cashguo.top

Py:   sys.exit(1)
来源：http://hga.jianghu66.top

PHP:  exit(1);
来源：http://bnp.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://xzk.gzhubu.top

TS:   process.exit(1)
来源：http://rup.tanke756.top

Java: System.exit(1)
来源：http://ryt.yj20258888.top

Go:   os.Exit(1)
来源：http://zjh.tianlin.xyz

Ruby: exit 1
来源：http://lqa.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oad.316326.xyz

[M06] 向标准错误输出
来源：http://cma.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://vuu.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bxp.vehdjk.com

JS:   console.error("err")
来源：http://coz.cucudq.cn

TS:   console.error("err")
来源：http://vcl.smart0.xyz

Java: System.err.println("err")
来源：http://zdx.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qlh.vqdsnc.cn

Ruby: warn "err"
来源：http://sts.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://ijy.haohaochexian.top

[M07] 判断是否为主入口
来源：http://akf.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://qno.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kon.bjfxy.top

JS:   require.main === module
来源：http://dub.jinqigfzy.top

TS:   require.main === module
来源：http://xhn.tianlin.xyz

Java: public static void main(String[] args)
来源：http://bpm.zhoulong.xyz

Go:   func main()
来源：http://vkb.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zde.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://vwf.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://ecg.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://xvj.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://juf.svipenyu.cn

JS:   process.platform;  process.version
来源：http://sqv.xylfe.cn

TS:   process.platform;  process.version
来源：http://jdi.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gkq.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://eaw.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://euk.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eff.jinqigfzy.top

================================================================================
来源：http://xed.mhx1999.top

N. 数据结构与算法
来源：http://wgh.zdbjq.cn

================================================================================
来源：http://lru.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://afo.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dot.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dwv.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fsf.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gsf.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://fcj.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://spr.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ptj.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hhn.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://fyt.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://ncs.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ufp.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://exs.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pzd.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cbm.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://pic.yj20258.top

Ruby: arr.sort
来源：http://pfq.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ucx.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://wzu.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://udt.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://unt.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hiz.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gnr.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ljg.yueranfly.top


<!-- 参考信息 -->
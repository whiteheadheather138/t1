代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://seh.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://jbw.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://axl.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://cia.jqgufenzy.top

[J07] 比较两个日期
来源：http://vnn.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://qqa.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jpw.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://num.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qxj.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ipj.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bwm.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yqz.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://ees.aibaodan.cn

[J08] 提取年月日与星期
来源：http://jsh.nanxuanxn.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vkz.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://duq.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://exr.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ksd.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://llk.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vxq.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hva.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ccl.jinghuilouyu.cn

[J09] 时区处理
来源：http://dbp.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vxp.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://evj.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ksa.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pkz.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ryq.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nyu.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tbc.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uxa.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://gty.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://qiy.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hte.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wry.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://asn.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://clf.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ovq.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kuc.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bpl.jqgufenzy.top

================================================================================
来源：http://opy.zhongyouzk.top

K. JSON 与序列化
来源：http://bmp.fzhhl.top

================================================================================
来源：http://lxa.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://wfi.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jvh.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ybz.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://qoq.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://dgp.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xux.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://epc.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cjr.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://epn.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://zqk.zhoulong.xyz

Py:   json.loads(s)
来源：http://hxf.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://czw.jqgfzy.top

JS:   JSON.parse(s)
来源：http://uyw.xziqi.cn

TS:   JSON.parse(s)
来源：http://muu.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bex.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://wky.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://mqs.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ztr.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://zql.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qur.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hst.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ulk.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rfd.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mtm.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ila.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wmc.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gqz.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://qtr.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lwx.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jvb.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebg.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ojr.hesvh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rff.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jwn.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mdw.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wre.fktsv.cn

[K05] 深拷贝对象
来源：http://wzu.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://wqw.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://jea.c1oappe.top

JS:   structuredClone(obj)
来源：http://qep.52xcode.cn

TS:   structuredClone(obj)
来源：http://ouv.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://trp.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://off.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wkc.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sur.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://eyr.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zgf.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tmj.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kfh.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gzb.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sfh.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dyi.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hzs.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://prv.pengpengdd.cyou

[K07] 进制转换
来源：http://ijt.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vsd.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zfd.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ulc.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aad.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ish.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mbq.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vsi.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uba.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://mwp.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://nkz.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qoo.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://doq.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://ezp.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bxk.zhijiandao.cn

Go:   encoding/gob
来源：http://wqi.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://fjc.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dds.shanyushiyangtech.top

================================================================================
来源：http://hvt.ydzc1.top

L. 网络请求
来源：http://ard.andypj.xyz

================================================================================
来源：http://gfv.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://cqa.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://msb.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aot.vehdjk.com

JS:   await fetch(url)
来源：http://ufy.pengpengdd.cyou

TS:   await fetch(url)
来源：http://trp.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ayb.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://mfu.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://avi.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ohs.nanxinkj.top

[L02] 发送 POST JSON
来源：http://adx.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://vsr.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nep.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cmd.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qlg.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lbn.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pfo.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iaa.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xnm.gotoacloud.top

[L03] 设置自定义请求头
来源：http://qqm.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zhn.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://niy.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gom.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylt.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wlc.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mpv.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zev.c1oappe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ard.sufxvd.cn

[L04] 设置超时
来源：http://eez.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://oou.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tsw.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://omi.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bdl.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zmy.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jef.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rse.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tis.cucudq.cn

[L05] 上传文件（multipart）
来源：http://xdt.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bfo.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nqu.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://izu.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rxn.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ohd.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aow.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lyy.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eup.epnwcf.com

[L06] 解析响应为 JSON
来源：http://dot.chenzaomai.com

Py:   resp.json()
来源：http://yva.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://hgj.xinyue.icu

JS:   await resp.json()
来源：http://cyo.xziqi.cn

TS:   await resp.json()
来源：http://kpc.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lrb.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gnh.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://bgx.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iqi.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://igc.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://haq.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gyn.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://tmu.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://xut.hcnkem.com

Java: resp.statusCode()
来源：http://ybo.birdmap.top

Go:   resp.StatusCode
来源：http://upu.hammf.cn

Ruby: resp.code.to_i
来源：http://thl.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://mxd.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://vir.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yal.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://dvc.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crv.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://thf.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwd.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qri.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rmf.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wvh.epnwcf.com

================================================================================
来源：http://rys.ydjk.org.cn

M. 命令行 / 进程 / 环境
来源：http://xxe.hfpthk.cn

================================================================================
来源：http://uju.ppjwa.cn

[M01] 读取命令行参数
来源：http://iob.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://hym.yvedp.cn

PHP:  $argv;  $argc;
来源：http://yhw.cucudq.cn

JS:   process.argv.slice(2)
来源：http://crt.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://rmg.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://vpy.yj202588.top

Go:   os.Args[1:]
来源：http://fiy.jinghuilouyu.cn

Ruby: ARGV
来源：http://rwr.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://fpb.9152youxi.cn

[M02] 读取环境变量
来源：http://fhq.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://xxs.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ufp.gaohongyu789.top

JS:   process.env.HOME
来源：http://zut.ivvv.top

TS:   process.env.HOME
来源：http://syq.jqgfzy.top

Java: System.getenv("HOME")
来源：http://hwc.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://voc.vehdjk.com

Ruby: ENV["HOME"]
来源：http://fpi.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qsi.fktsv.cn

[M03] 执行外部命令
来源：http://djb.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpx.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mtm.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vno.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ygm.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iqm.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hzn.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://ump.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://may.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://maz.ivvv.top

Py:   os.getcwd()
来源：http://jmu.hongshengwenyu.top

PHP:  getcwd();
来源：http://mdz.chenjidiqi.icu

JS:   process.cwd()
来源：http://lhr.smart0.xyz

TS:   process.cwd()
来源：http://bfs.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://lwc.yvedp.cn

Go:   os.Getwd()
来源：http://luv.havefunace.top

Ruby: Dir.pwd
来源：http://xcy.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://avw.feifeiyinyue.top

[M05] 设置退出码
来源：http://vul.guannengcc.top

Py:   sys.exit(1)
来源：http://jiu.sysykeji.top

PHP:  exit(1);
来源：http://kfj.pengpengdd.cyou

JS:   process.exit(1)
来源：http://sut.vqdsnc.cn

TS:   process.exit(1)
来源：http://pin.daria6918.cn

Java: System.exit(1)
来源：http://jve.9152youxi.cn

Go:   os.Exit(1)
来源：http://fli.zhijiandao.cn

Ruby: exit 1
来源：http://nwk.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://psg.yueranfly.top

[M06] 向标准错误输出
来源：http://ywe.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://pel.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dit.hongshengwenyu.top

JS:   console.error("err")
来源：http://ajg.hnxiangtu.top

TS:   console.error("err")
来源：http://oaw.yj20258.top

Java: System.err.println("err")
来源：http://pot.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qmr.iojbl.cn

Ruby: warn "err"
来源：http://imq.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://boe.cashguo.top

[M07] 判断是否为主入口
来源：http://xav.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://hsg.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bxm.gotoacloud.top

JS:   require.main === module
来源：http://ptk.birdmap.top

TS:   require.main === module
来源：http://lib.nanxinkj.top

Java: public static void main(String[] args)
来源：http://bpx.jlsjyb.cn

Go:   func main()
来源：http://zdk.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ruj.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://eeq.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://dnh.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://azf.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://duf.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://rku.tianlin.xyz

TS:   process.platform;  process.version
来源：http://opv.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://njw.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://xwr.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://reh.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nwc.jinghuilouyu.cn

================================================================================
来源：http://gbh.daria6918.cn

N. 数据结构与算法
来源：http://kcq.yonumen.top

================================================================================
来源：http://zdr.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://wmr.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hse.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ehb.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rhj.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zbp.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://gkd.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://hnw.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://iot.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://klc.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://sfz.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://ftb.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eeu.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gjd.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kgv.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ybr.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://arp.chenjidiqi.icu

Ruby: arr.sort
来源：http://hfw.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://kux.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://cbg.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ajk.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://gic.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojq.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bzo.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iru.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sqp.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qtj.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://rdh.xuanzx.com

[N04] 斐波那契数列
来源：http://npg.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ypi.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zmu.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nmw.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zen.epnwcf.com


<!-- 参考信息 -->
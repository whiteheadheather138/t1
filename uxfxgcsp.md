代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ejj.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://ixf.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://xac.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://kxy.vehdjk.com

[J07] 比较两个日期
来源：http://jaj.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://hmk.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ajv.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zrr.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wvj.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xwm.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yko.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://pcy.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://hvt.ehwqpu.com

[J08] 提取年月日与星期
来源：http://hzh.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ccp.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://umc.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mul.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dng.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jjw.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hsj.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ide.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xfv.shangyingyoupin.top

[J09] 时区处理
来源：http://zeu.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gmb.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://huv.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iia.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ibg.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qkz.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jcq.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vld.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xjy.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://yjq.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zjc.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://emf.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://utu.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pna.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kqs.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://psp.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dcl.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://feo.jinghuilouyu.cn

================================================================================
来源：http://tfk.ppjwa.cn

K. JSON 与序列化
来源：http://btn.daxiang520.top

================================================================================
来源：http://lqa.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://vrq.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cyv.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ivc.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://ake.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://kzo.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hgs.mhx1999.top

Go:   json.Marshal(obj)
来源：http://aed.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://nvs.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://hid.redwolf501.top

[K02] JSON 字符串转对象
来源：http://tuf.kuanghao11.cn

Py:   json.loads(s)
来源：http://dws.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bhy.fktsv.cn

JS:   JSON.parse(s)
来源：http://qxv.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://jjb.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cud.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ebk.daxiang520.top

Ruby: JSON.parse(s)
来源：http://eux.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gxh.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://kiv.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fzu.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uvy.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://neb.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lld.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cot.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bgj.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://vaf.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmv.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://cyi.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kek.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://izb.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gca.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ihz.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gyj.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mhd.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vhc.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bie.ydjk.org.cn

[K05] 深拷贝对象
来源：http://ygf.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://tyz.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://ndn.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://xvy.tarul.cn

TS:   structuredClone(obj)
来源：http://kum.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eag.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jft.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://njj.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://opt.cashguo.top

[K06] 解析 URL 查询串
来源：http://bhr.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xmj.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uch.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gqu.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wom.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vfx.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zcu.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://efg.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hiv.sweek.top

[K07] 进制转换
来源：http://app.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://omg.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lqx.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lym.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fya.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnc.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmr.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uca.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xrx.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://fxo.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://uez.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://old.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://fim.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://qrn.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://opk.smart0.xyz

Go:   encoding/gob
来源：http://wrt.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://mqx.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mkg.chenjidiqi.icu

================================================================================
来源：http://gtu.xziqi.cn

L. 网络请求
来源：http://klj.jqgufenzy.top

================================================================================
来源：http://hlj.wangdashe.top

[L01] 发送 GET 请求
来源：http://eys.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nym.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rce.ivvv.top

JS:   await fetch(url)
来源：http://qnc.aibaodan.cn

TS:   await fetch(url)
来源：http://zea.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hmf.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://oqc.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://fpx.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cah.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://tmc.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://vli.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ozu.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjs.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xde.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oac.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oiv.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qxa.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://efo.pycfn.com

[L03] 设置自定义请求头
来源：http://wvl.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zqw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tdy.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihi.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cuq.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xzc.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yrt.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dxm.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qpn.svipenyu.cn

[L04] 设置超时
来源：http://byg.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://jtt.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fva.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lpm.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nev.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ngr.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vfr.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yob.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tbd.tian-w.cn

[L05] 上传文件（multipart）
来源：http://oct.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uhw.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lxf.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sye.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vai.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rik.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nff.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://npe.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lfq.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://xzi.nwbrower.top

Py:   resp.json()
来源：http://ppc.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://vca.316326.xyz

JS:   await resp.json()
来源：http://sps.xylfe.cn

TS:   await resp.json()
来源：http://ois.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dip.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://njm.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://ksd.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qyd.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://hap.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sul.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lur.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://gva.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://wis.jqgufenzy.top

Java: resp.statusCode()
来源：http://syj.nanxuanxn.top

Go:   resp.StatusCode
来源：http://dpy.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://ywk.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://ekk.fktsv.cn

[L08] 并发请求多个地址
来源：http://esf.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ilc.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://eah.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://clq.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ehu.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://afq.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wwf.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jfy.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ylq.quarkkingdee.top

================================================================================
来源：http://rrq.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://odm.nwbrower.top

================================================================================
来源：http://pww.ydzc1.top

[M01] 读取命令行参数
来源：http://mfu.jinqigufen.top

Py:   sys.argv[1:]
来源：http://dyv.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://pjl.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://fkm.gzhubu.top

TS:   process.argv.slice(2)
来源：http://kqx.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://twp.yongpay.top

Go:   os.Args[1:]
来源：http://uqz.chenlongwang.top

Ruby: ARGV
来源：http://its.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://tmd.feifeiyinyue.top

[M02] 读取环境变量
来源：http://zbe.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://hxb.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fpn.hfpthk.cn

JS:   process.env.HOME
来源：http://rea.tian-w.cn

TS:   process.env.HOME
来源：http://hfr.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://egv.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uyp.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://ttt.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wjz.cqqwz.cn

[M03] 执行外部命令
来源：http://zyd.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rgi.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vye.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dea.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yno.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tvj.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uek.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://dld.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://fuy.yfazqb.com

[M04] 获取当前工作目录
来源：http://krk.shuidangran.top

Py:   os.getcwd()
来源：http://hci.hcnkem.com

PHP:  getcwd();
来源：http://kep.fengsongda.top

JS:   process.cwd()
来源：http://urp.guowangkeji.top

TS:   process.cwd()
来源：http://nfe.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://isc.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://ykj.tarul.cn

Ruby: Dir.pwd
来源：http://vsw.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://dtx.feifeiyinyue.top

[M05] 设置退出码
来源：http://ccm.yongpay.top

Py:   sys.exit(1)
来源：http://dxi.bbcook.cn

PHP:  exit(1);
来源：http://vtq.quarkkingdee.top

JS:   process.exit(1)
来源：http://mxw.hammf.cn

TS:   process.exit(1)
来源：http://jku.kuanghao11.cn

Java: System.exit(1)
来源：http://vwl.jianghu66.top

Go:   os.Exit(1)
来源：http://blk.wangdashe.top

Ruby: exit 1
来源：http://jnq.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ita.xziqi.cn

[M06] 向标准错误输出
来源：http://hkj.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://cgg.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jrl.gzhubu.top

JS:   console.error("err")
来源：http://ecz.yj202588.top

TS:   console.error("err")
来源：http://pcl.wangshuangyany.cn

Java: System.err.println("err")
来源：http://lkm.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ezk.jlsjyb.cn

Ruby: warn "err"
来源：http://oug.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://gpf.snrcjt.cn

[M07] 判断是否为主入口
来源：http://wcr.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://noj.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nvn.sxryk.cn

JS:   require.main === module
来源：http://piq.ctjpmb.com

TS:   require.main === module
来源：http://nou.dashuyun.cn

Java: public static void main(String[] args)
来源：http://ukt.bjfxy.top

Go:   func main()
来源：http://ohn.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wgf.fengsongda.top

C#:   static void Main(string[] args)
来源：http://cdt.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://ahz.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://qzp.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://vxe.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://dwr.yonumen.top

TS:   process.platform;  process.version
来源：http://vam.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hub.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kna.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kab.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xpz.tarul.cn

================================================================================
来源：http://alt.yonumen.top

N. 数据结构与算法
来源：http://fqj.316326.xyz

================================================================================
来源：http://lki.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://wwh.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ppx.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xxu.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxn.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sss.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://gvh.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://hjl.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://cch.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aji.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://tsz.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://qys.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ybr.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bon.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://kvr.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mkx.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://hsy.jiagoushi.top

Ruby: arr.sort
来源：http://flt.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tpj.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://zio.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ele.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://mfa.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://akj.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://opf.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dhn.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ebu.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gol.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://agn.ctjpmb.com

[N04] 斐波那契数列
来源：http://wcg.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yyn.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thu.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://glk.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://emp.52xcode.cn


<!-- 参考信息 -->
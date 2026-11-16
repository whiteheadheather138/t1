代发 wailian999

Py:   (end - start).total_seconds()
来源：http://lnz.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://bwe.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lzv.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cvh.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://kcb.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://jrj.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://vfh.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://irv.tian-w.cn

[J07] 比较两个日期
来源：http://nag.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://hmo.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xmr.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://xhu.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://wcu.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ehr.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hbx.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ycg.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://hvz.hcnkem.com

[J08] 提取年月日与星期
来源：http://hkj.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cpp.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uph.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zvk.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://maw.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://owh.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dol.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xlj.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oon.tarul.cn

[J09] 时区处理
来源：http://spl.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fil.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zid.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjy.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://inx.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hvo.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zrm.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iva.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ppb.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://rys.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bqb.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wkh.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://suo.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bwu.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://beo.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blx.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qxz.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xjg.pycfn.com

================================================================================
来源：http://lbr.sysykeji.top

K. JSON 与序列化
来源：http://ipy.uphjek.com

================================================================================
来源：http://bmr.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://vnl.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yhz.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jon.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://bwk.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://nys.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ohh.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://xcy.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://hvz.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://frn.shuidangran.top

[K02] JSON 字符串转对象
来源：http://irc.aibaodan.cn

Py:   json.loads(s)
来源：http://tdi.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vra.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://omd.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://vie.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fun.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://icm.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://blp.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mxe.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://unw.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fzo.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ryo.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://qre.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lxi.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wyw.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gjb.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://jjb.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lbp.aizwys.cn

[K04] 读取 JSON 文件
来源：http://dle.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wyr.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://egv.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdf.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyf.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cfj.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://txp.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://iyj.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nja.zdbjq.cn

[K05] 深拷贝对象
来源：http://uqz.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://nex.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://dkx.fzhhl.top

JS:   structuredClone(obj)
来源：http://ygj.ehwqpu.com

TS:   structuredClone(obj)
来源：http://jpd.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://udc.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dex.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oqx.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://toa.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://yka.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cnm.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ybk.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zuw.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://drg.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bnw.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mkw.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vkf.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lje.zhongyouzk.top

[K07] 进制转换
来源：http://wgu.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lje.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://epm.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gwa.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://srl.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ago.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://frw.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tnk.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yjg.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://hdi.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://xhn.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lhb.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://jnb.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://dsh.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://djx.vqdsnc.cn

Go:   encoding/gob
来源：http://frs.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://qno.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dnq.chenzaomai.com

================================================================================
来源：http://pah.9152youxi.cn

L. 网络请求
来源：http://ozd.sjlbkw.cn

================================================================================
来源：http://ssv.daxiang520.top

[L01] 发送 GET 请求
来源：http://nxc.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ytf.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mvr.ybcxt.top

JS:   await fetch(url)
来源：http://rvg.zhiwuduotai.top

TS:   await fetch(url)
来源：http://zpg.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pyz.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://bxy.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://tqy.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jlc.gzhubu.top

[L02] 发送 POST JSON
来源：http://aih.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://hxf.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://znx.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbc.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mou.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zcp.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tay.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zfq.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqh.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://xsi.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eii.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hsk.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lcx.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqo.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wjb.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aoe.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozr.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ddr.cashguo.top

[L04] 设置超时
来源：http://kjf.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://sni.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://spv.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wic.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mjs.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fuv.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xnh.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rvk.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lfi.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://pcq.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ehu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://snv.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://roc.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kwc.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jiu.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zbe.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://clh.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qqp.nwbrower.top

[L06] 解析响应为 JSON
来源：http://uev.birdmap.top

Py:   resp.json()
来源：http://jnl.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://ltt.0kj1m.cn

JS:   await resp.json()
来源：http://nvy.yvedp.cn

TS:   await resp.json()
来源：http://ffv.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ouz.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://euw.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://tbo.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hsc.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://atx.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://smc.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ovc.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://rgn.ivvv.top

TS:   resp.ok;  resp.status
来源：http://mml.jinqigfzy.top

Java: resp.statusCode()
来源：http://abu.mhx1999.top

Go:   resp.StatusCode
来源：http://vbf.hnqzz.top

Ruby: resp.code.to_i
来源：http://phq.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://bsf.aizwys.cn

[L08] 并发请求多个地址
来源：http://ywe.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ijf.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://mdw.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wja.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aly.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jhe.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://skq.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ryd.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hcr.yueranfly.top

================================================================================
来源：http://bkd.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://ndr.fzhhl.top

================================================================================
来源：http://qis.nwbrower.top

[M01] 读取命令行参数
来源：http://lhq.ybcxt.top

Py:   sys.argv[1:]
来源：http://wws.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://ntt.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://fcu.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://shh.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://dtf.cqqwz.cn

Go:   os.Args[1:]
来源：http://qqv.fanxiaobao.xyz

Ruby: ARGV
来源：http://ckz.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://epp.cheryme.top

[M02] 读取环境变量
来源：http://see.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://nxa.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vwi.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://ion.vqdsnc.cn

TS:   process.env.HOME
来源：http://fwi.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://ski.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qno.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://gig.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jfy.yanxiufei.cn

[M03] 执行外部命令
来源：http://czk.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://viq.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tve.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sun.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xva.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bol.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ndj.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pqv.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://pkm.yongpay.top

[M04] 获取当前工作目录
来源：http://kbd.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://ccl.fengsongda.top

PHP:  getcwd();
来源：http://sxe.bjfxy.top

JS:   process.cwd()
来源：http://pso.zhijiandao.cn

TS:   process.cwd()
来源：http://qqb.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://bzb.pycfn.com

Go:   os.Getwd()
来源：http://cdp.bbcook.cn

Ruby: Dir.pwd
来源：http://tmi.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://yxe.316326.xyz

[M05] 设置退出码
来源：http://wet.9152youxi.cn

Py:   sys.exit(1)
来源：http://ohb.iojbl.cn

PHP:  exit(1);
来源：http://ryb.guowangkeji.top

JS:   process.exit(1)
来源：http://oed.xziqi.cn

TS:   process.exit(1)
来源：http://qsd.ppjwa.cn

Java: System.exit(1)
来源：http://zae.birdmap.top

Go:   os.Exit(1)
来源：http://hek.dianchejie.cn

Ruby: exit 1
来源：http://sqa.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://arm.sysykeji.top

[M06] 向标准错误输出
来源：http://hoq.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://ozu.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://amt.dashuyun.cn

JS:   console.error("err")
来源：http://vux.chenzaomai.com

TS:   console.error("err")
来源：http://vdy.zhengqikj.top

Java: System.err.println("err")
来源：http://msi.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qhp.gogol.net.cn

Ruby: warn "err"
来源：http://uxb.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://any.iojbl.cn

[M07] 判断是否为主入口
来源：http://mtz.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://gua.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ppi.tarul.cn

JS:   require.main === module
来源：http://sso.jqgufenzy.top

TS:   require.main === module
来源：http://pkz.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://emx.hongshengwenyu.top

Go:   func main()
来源：http://oiq.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tob.sysykeji.top

C#:   static void Main(string[] args)
来源：http://uue.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://xak.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://fog.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://dwe.jqgfzy.top

JS:   process.platform;  process.version
来源：http://ghm.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://ydo.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihf.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wur.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://con.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yen.svipenyu.cn

================================================================================
来源：http://qkt.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://klo.dashuyun.cn

================================================================================
来源：http://nqz.yonumen.top

[N01] 二分查找（有序数组）
来源：http://qtp.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://apw.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://isk.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qnm.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alk.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hxs.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://khz.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jib.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://gyv.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://sll.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://igf.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eor.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lnv.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cnq.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ahx.yonumen.top

Go:   slices.Sort(arr)
来源：http://wpo.gaohongyu789.top

Ruby: arr.sort
来源：http://psr.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fdo.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://fcc.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://emg.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://vik.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jtq.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://faq.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cis.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ehl.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gza.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://kmv.cucudq.cn

[N04] 斐波那契数列
来源：http://hmj.cucudq.cn


<!-- 参考信息 -->
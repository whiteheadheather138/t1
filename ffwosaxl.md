代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mql.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kjz.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nfi.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zwm.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zsu.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xth.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://vtn.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://ueb.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://hwx.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vkk.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zoy.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://inu.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nip.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://dmk.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ppg.yj20258.top

[J06] 计算两时间之差
来源：http://rld.havefunace.top

Py:   (end - start).total_seconds()
来源：http://azw.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://hen.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bqx.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pay.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tre.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://dgv.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://nvg.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://uuu.jqgfzy.top

[J07] 比较两个日期
来源：http://qam.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://apw.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ikr.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://pwm.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iik.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tda.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wkd.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zua.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://vgj.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://xnf.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://edr.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://coa.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://agq.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jvs.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dbw.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vlz.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yhc.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tcc.zhoulong.xyz

[J09] 时区处理
来源：http://moe.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvv.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ngx.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdk.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctm.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://khv.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uds.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qpi.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vjf.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://tjy.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lyz.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xnw.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xmq.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://coo.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rnb.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://htv.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jaj.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ctr.fehbvm.com

================================================================================
来源：http://hyb.hongshengwenyu.top

K. JSON 与序列化
来源：http://pma.hongshengwenyu.top

================================================================================
来源：http://chg.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://czu.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bhk.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kfj.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://jht.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://alh.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bnm.aizwys.cn

Go:   json.Marshal(obj)
来源：http://ics.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qnu.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tnl.yueranfly.top

[K02] JSON 字符串转对象
来源：http://kea.tarul.cn

Py:   json.loads(s)
来源：http://kwo.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nxu.jinqigufen.top

JS:   JSON.parse(s)
来源：http://wmk.wangdashe.top

TS:   JSON.parse(s)
来源：http://dwu.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bhu.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://kok.c1oappe.top

Ruby: JSON.parse(s)
来源：http://bnd.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zia.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://zvz.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://efu.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mng.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hje.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jpn.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://epo.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://asi.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://xsx.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mwt.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://ahw.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sgi.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kcr.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvq.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctj.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://upv.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pfq.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wab.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jfq.andypj.xyz

[K05] 深拷贝对象
来源：http://ktc.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://wtg.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://ikd.daxiang520.top

JS:   structuredClone(obj)
来源：http://hdo.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://tas.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ptt.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zli.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://skn.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vdq.yj20258888.top

[K06] 解析 URL 查询串
来源：http://rdo.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iqq.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wrl.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwx.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qkv.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fqm.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ylx.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rqz.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uvl.redwolf501.top

[K07] 进制转换
来源：http://org.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vbn.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://czq.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rtr.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mja.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fwy.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://euz.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://koi.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xzu.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://had.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://suc.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dwi.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://apd.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://pis.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vvo.snrcjt.cn

Go:   encoding/gob
来源：http://jkp.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://ops.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lll.yvedp.cn

================================================================================
来源：http://kwz.dashuyun.cn

L. 网络请求
来源：http://hag.fehbvm.com

================================================================================
来源：http://wmt.hywenlv.cn

[L01] 发送 GET 请求
来源：http://ype.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wqn.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fgu.jqgfzy.top

JS:   await fetch(url)
来源：http://gte.mhx1999.top

TS:   await fetch(url)
来源：http://ejt.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qxt.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://zrz.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qim.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://udk.pycfn.com

[L02] 发送 POST JSON
来源：http://wgx.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://szs.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ivp.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlw.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwe.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lgi.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jbb.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hss.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jax.cashguo.top

[L03] 设置自定义请求头
来源：http://jwq.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qdn.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://loo.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqd.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://puy.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cfl.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://drr.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pad.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iwx.haohaochexian.top

[L04] 设置超时
来源：http://fyy.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://utk.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jdc.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofl.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bra.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wxy.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://acd.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vgl.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rqy.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://cbk.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://png.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fzf.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://heu.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://igm.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xhm.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygv.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kem.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fka.316326.xyz

[L06] 解析响应为 JSON
来源：http://psk.yueranfly.top

Py:   resp.json()
来源：http://nmt.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://cmu.bjfxy.top

JS:   await resp.json()
来源：http://qfc.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://eif.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gwc.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pxq.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://zuu.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dsk.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://tsc.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ons.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hly.cheryme.top

JS:   resp.ok;  resp.status
来源：http://smd.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://mvq.xinyue.icu

Java: resp.statusCode()
来源：http://skm.aizwys.cn

Go:   resp.StatusCode
来源：http://zdp.sysykeji.top

Ruby: resp.code.to_i
来源：http://zxp.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://qvg.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://hfk.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hyj.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://asd.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wtb.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://euf.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zer.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oge.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dye.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ubz.andypj.xyz

================================================================================
来源：http://pxk.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://igs.gogol.net.cn

================================================================================
来源：http://vfa.yj20258.top

[M01] 读取命令行参数
来源：http://qbq.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://tzn.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://okv.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://wuc.ivvv.top

TS:   process.argv.slice(2)
来源：http://dtx.ivvv.top

Java: args 数组（main 方法参数）
来源：http://phj.shuidangran.top

Go:   os.Args[1:]
来源：http://xmo.bjfxy.top

Ruby: ARGV
来源：http://mfd.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://qot.ydjk.org.cn

[M02] 读取环境变量
来源：http://seo.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://vdf.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nwm.zycfv.cn

JS:   process.env.HOME
来源：http://wyi.xuetiantiany.cn

TS:   process.env.HOME
来源：http://fzy.haohaochexian.top

Java: System.getenv("HOME")
来源：http://ftb.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ect.yj202588.top

Ruby: ENV["HOME"]
来源：http://fjq.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iij.xylfe.cn

[M03] 执行外部命令
来源：http://gon.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mzr.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zzm.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://mdd.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rcw.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dco.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zka.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aue.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://hiz.yueranfly.top

[M04] 获取当前工作目录
来源：http://btg.kuanghao11.cn

Py:   os.getcwd()
来源：http://dok.shzxlz.cn

PHP:  getcwd();
来源：http://kum.shanyushiyangtech.top

JS:   process.cwd()
来源：http://lbm.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://wcj.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://wug.hcnkem.com

Go:   os.Getwd()
来源：http://rvp.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://nia.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fgn.yanxiufei.cn

[M05] 设置退出码
来源：http://snw.aizwys.cn

Py:   sys.exit(1)
来源：http://bcc.hywenlv.cn

PHP:  exit(1);
来源：http://qvb.tianlin.xyz

JS:   process.exit(1)
来源：http://kne.birdmap.top

TS:   process.exit(1)
来源：http://nql.xylfe.cn

Java: System.exit(1)
来源：http://npf.birdmap.top

Go:   os.Exit(1)
来源：http://lmt.haohaochexian.top

Ruby: exit 1
来源：http://sie.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://imh.aibaodan.cn

[M06] 向标准错误输出
来源：http://zas.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://mjq.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ter.andypj.xyz

JS:   console.error("err")
来源：http://dxl.zhoulong.xyz

TS:   console.error("err")
来源：http://koz.chenzaomai.com

Java: System.err.println("err")
来源：http://ykw.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://frq.birdmap.top

Ruby: warn "err"
来源：http://tjh.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://skq.daria6918.cn

[M07] 判断是否为主入口
来源：http://rqr.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://edo.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sfd.zhongyouzk.top

JS:   require.main === module
来源：http://kwi.shanyushiyangkeji.top

TS:   require.main === module
来源：http://pct.yonumen.top

Java: public static void main(String[] args)
来源：http://bri.nanxinkj.top

Go:   func main()
来源：http://twa.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://igk.uphjek.com

C#:   static void Main(string[] args)
来源：http://vwc.pycfn.com

[M08] 获取系统与运行时信息
来源：http://hmu.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://nfy.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://vbx.cqqwz.cn

JS:   process.platform;  process.version
来源：http://thb.fengsongda.top

TS:   process.platform;  process.version
来源：http://ted.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qku.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tfa.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://clp.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mlx.quarkkingdee.top

================================================================================
来源：http://yza.birdmap.top

N. 数据结构与算法
来源：http://xkm.zhiwuduotai.top

================================================================================
来源：http://iui.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://gsd.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rdw.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jlj.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtb.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cxf.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://yzh.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://bsv.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://rwt.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://ocs.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://fex.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://fis.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rds.xylfe.cn


<!-- 参考信息 -->
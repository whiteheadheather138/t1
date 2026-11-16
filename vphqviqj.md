代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://esi.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tcz.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://kii.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://gss.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hkf.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vsk.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndj.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://mqy.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zus.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://aag.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mao.hfpthk.cn

[J06] 计算两时间之差
来源：http://yeo.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://ssb.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://gjl.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gkr.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gpt.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://vyr.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://uhy.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://zat.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://gaa.bbcook.cn

[J07] 比较两个日期
来源：http://nom.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://yqw.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kiz.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hib.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://log.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nyg.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gep.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qsz.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://awp.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://olp.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gdk.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uif.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yuj.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qfv.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bgh.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sww.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ccs.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gzb.gogol.net.cn

[J09] 时区处理
来源：http://oyn.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ffj.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jkn.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbj.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ezx.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sgc.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jsx.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://egn.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yhr.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://cfl.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fua.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nct.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iph.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jsh.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://idb.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wdj.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rnz.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kmk.yj20258888.top

================================================================================
来源：http://uzn.redwolf501.top

K. JSON 与序列化
来源：http://xes.ehwqpu.com

================================================================================
来源：http://nve.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://enx.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qun.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ljw.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://qkk.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://cqh.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://msj.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://euf.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://drk.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zml.nwbrower.top

[K02] JSON 字符串转对象
来源：http://mhw.xuetiantiany.cn

Py:   json.loads(s)
来源：http://ybu.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gyr.cashguo.top

JS:   JSON.parse(s)
来源：http://nmu.zdbjq.cn

TS:   JSON.parse(s)
来源：http://nyg.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zov.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://leo.cashguo.top

Ruby: JSON.parse(s)
来源：http://jqy.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jdg.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://txn.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lcg.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aas.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://slm.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://vqn.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dvh.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ouw.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ysi.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vif.jianghu66.top

[K04] 读取 JSON 文件
来源：http://olc.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ltb.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rbu.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixo.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jsp.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iga.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dms.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ieo.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cam.epnwcf.com

[K05] 深拷贝对象
来源：http://hkw.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://mhc.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://dib.cheryme.top

JS:   structuredClone(obj)
来源：http://wlp.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://dsu.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://izb.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rfw.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fwk.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oox.hesvh.cn

[K06] 解析 URL 查询串
来源：http://mok.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ejx.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fep.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fli.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://czc.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wtw.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://iew.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qvl.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://biw.ppjwa.cn

[K07] 进制转换
来源：http://prl.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bcz.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://isc.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dvp.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eel.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aws.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://omc.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jzm.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lar.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://jyz.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://jzy.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ftc.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://one.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://xvz.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dqf.ydjk.org.cn

Go:   encoding/gob
来源：http://wns.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://rhw.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gqe.shanyushiyangtech.top

================================================================================
来源：http://hso.sysykeji.top

L. 网络请求
来源：http://hfx.ydjk.org.cn

================================================================================
来源：http://cii.tanke756.top

[L01] 发送 GET 请求
来源：http://kfy.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://knr.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywk.ybcxt.top

JS:   await fetch(url)
来源：http://kkb.sufxvd.cn

TS:   await fetch(url)
来源：http://ipn.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dld.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://hhv.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://myp.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ifk.ybcxt.top

[L02] 发送 POST JSON
来源：http://mtw.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://mdo.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vlk.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dkg.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfu.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sfn.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ndr.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wqp.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lxz.cucudq.cn

[L03] 设置自定义请求头
来源：http://zul.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hmi.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jkd.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zow.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ons.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ltj.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kxg.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fxg.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ygk.nanxuanxn.top

[L04] 设置超时
来源：http://wsf.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://mox.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jep.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yni.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://txi.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nqd.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://loh.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://txv.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uhj.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://nwj.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dux.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aeg.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fwc.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fdk.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ydw.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fri.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pme.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lmd.wangdashe.top

[L06] 解析响应为 JSON
来源：http://xxi.chenlongwang.top

Py:   resp.json()
来源：http://emh.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://bxd.tian-w.cn

JS:   await resp.json()
来源：http://nfy.nwbrower.top

TS:   await resp.json()
来源：http://ffv.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jqk.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://crg.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://gbp.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://caz.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://yrm.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xin.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hop.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://sii.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://bdm.snrcjt.cn

Java: resp.statusCode()
来源：http://gad.smart0.xyz

Go:   resp.StatusCode
来源：http://fag.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://emv.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://poa.smart0.xyz

[L08] 并发请求多个地址
来源：http://aud.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ncb.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://wyt.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xfm.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vin.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aul.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zax.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://int.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lgf.yongpay.top

================================================================================
来源：http://rkw.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://gco.epnwcf.com

================================================================================
来源：http://fos.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://vfo.meibo888.top

Py:   sys.argv[1:]
来源：http://ffg.birdmap.top

PHP:  $argv;  $argc;
来源：http://plu.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://cvi.cashguo.top

TS:   process.argv.slice(2)
来源：http://wwr.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://new.bjfxy.top

Go:   os.Args[1:]
来源：http://mnt.svipenyu.cn

Ruby: ARGV
来源：http://lmf.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://awe.nanxuanxn.top

[M02] 读取环境变量
来源：http://wgl.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://vmm.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nik.andypj.xyz

JS:   process.env.HOME
来源：http://crw.ivvv.top

TS:   process.env.HOME
来源：http://gsx.hesvh.cn

Java: System.getenv("HOME")
来源：http://hlk.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wbl.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://rsi.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dls.gzhubu.top

[M03] 执行外部命令
来源：http://azj.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://etn.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://epu.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kbv.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://guz.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ohi.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wtl.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://scs.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://wwz.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://wjg.mhx1999.top

Py:   os.getcwd()
来源：http://huh.sweek.top

PHP:  getcwd();
来源：http://nlz.cqqwz.cn

JS:   process.cwd()
来源：http://jge.hnxiangtu.top

TS:   process.cwd()
来源：http://xro.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://aoz.pycfn.com

Go:   os.Getwd()
来源：http://ifz.sjlbkw.cn

Ruby: Dir.pwd
来源：http://idc.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://pko.yanxiufei.cn

[M05] 设置退出码
来源：http://apc.xuanzx.com

Py:   sys.exit(1)
来源：http://mev.xuanzx.com

PHP:  exit(1);
来源：http://rvk.sjlbkw.cn

JS:   process.exit(1)
来源：http://mnk.yuanzhike.top

TS:   process.exit(1)
来源：http://rep.cucudq.cn

Java: System.exit(1)
来源：http://qdo.tian-w.cn

Go:   os.Exit(1)
来源：http://ofw.gogol.net.cn

Ruby: exit 1
来源：http://xfn.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xob.svipenyu.cn

[M06] 向标准错误输出
来源：http://ggz.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://mwx.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bln.andypj.xyz

JS:   console.error("err")
来源：http://oba.nanxuanxn.top

TS:   console.error("err")
来源：http://lrz.shangyingyoupin.top

Java: System.err.println("err")
来源：http://kga.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ely.pengpengdd.cyou

Ruby: warn "err"
来源：http://yap.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://hcb.fzhhl.top

[M07] 判断是否为主入口
来源：http://maz.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://yvk.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amy.zhijiandao.cn

JS:   require.main === module
来源：http://dea.yfazqb.com

TS:   require.main === module
来源：http://xbf.gogol.net.cn

Java: public static void main(String[] args)
来源：http://ntw.cqqwz.cn

Go:   func main()
来源：http://cxi.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fmf.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://dxi.meibo888.top

[M08] 获取系统与运行时信息
来源：http://jkw.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://hwi.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://jvt.smart0.xyz

JS:   process.platform;  process.version
来源：http://wdo.bbcook.cn

TS:   process.platform;  process.version
来源：http://jqa.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oux.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vgr.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ugy.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oav.daxiang520.top

================================================================================
来源：http://rrh.jianghu66.top

N. 数据结构与算法
来源：http://vlx.wangdashe.top

================================================================================
来源：http://jsc.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://icg.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://byk.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dik.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tdb.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://erk.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://npn.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://qkw.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pxt.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://npz.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://nkg.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://nmu.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tkd.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yxr.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://cwj.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dhw.andypj.xyz

Go:   slices.Sort(arr)
来源：http://exb.ydzc1.top


<!-- 参考信息 -->
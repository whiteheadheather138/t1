代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://avo.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mub.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://lva.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://cxw.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vxe.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lox.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wqy.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://xho.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xbt.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://ujz.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://eyo.gogol.net.cn

[J06] 计算两时间之差
来源：http://uqq.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://hpw.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://ccf.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tgv.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pww.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ckl.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://enr.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://eqa.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://ets.hysaishi.cn

[J07] 比较两个日期
来源：http://ggq.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://fwl.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qyi.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://diy.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://znq.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://trv.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fne.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://neq.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://iuc.sufxvd.cn

[J08] 提取年月日与星期
来源：http://lyl.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jnk.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dzn.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zxa.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vfq.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cwt.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kqt.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://btg.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mvk.iojbl.cn

[J09] 时区处理
来源：http://gpj.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://trz.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pbg.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hwn.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pys.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mdg.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nma.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zed.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kcd.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://okd.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://teq.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ccg.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ppf.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztp.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pgf.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mhy.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oct.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mpj.wangshuangyany.cn

================================================================================
来源：http://irk.zycfv.cn

K. JSON 与序列化
来源：http://duv.9152youxi.cn

================================================================================
来源：http://fyn.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://bwy.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tww.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xze.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://lsy.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://qgx.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gkd.sxryk.cn

Go:   json.Marshal(obj)
来源：http://viq.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tug.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rkg.yj20258.top

[K02] JSON 字符串转对象
来源：http://hjw.c1oappe.top

Py:   json.loads(s)
来源：http://xfw.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rdg.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://gtj.yuanzhike.top

TS:   JSON.parse(s)
来源：http://bqq.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ycl.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://rxq.ivvv.top

Ruby: JSON.parse(s)
来源：http://dwl.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bep.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://qls.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wlu.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ljs.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://izy.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fby.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jnj.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wsi.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://fkf.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sdj.bbcook.cn

[K04] 读取 JSON 文件
来源：http://iut.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jxp.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzx.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sxs.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gvb.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rth.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mto.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pmu.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eza.hnqzz.top

[K05] 深拷贝对象
来源：http://iuz.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://rem.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://but.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://wrh.tian-w.cn

TS:   structuredClone(obj)
来源：http://nlq.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nfh.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gcn.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://msw.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rgy.mhx1999.top

[K06] 解析 URL 查询串
来源：http://leq.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zjm.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwh.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ulk.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tbf.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fet.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://fas.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jri.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzm.cqqwz.cn

[K07] 进制转换
来源：http://zwq.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wpz.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rlf.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oyl.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://btq.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://opv.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rll.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nym.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://non.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://cja.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://vyl.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://alq.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://miz.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://alw.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://frz.wangshuangyany.cn

Go:   encoding/gob
来源：http://wsv.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://hmg.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://izx.jiagoushi.top

================================================================================
来源：http://ktv.52xcode.cn

L. 网络请求
来源：http://hnz.ydzc1.top

================================================================================
来源：http://bwr.smart0.xyz

[L01] 发送 GET 请求
来源：http://lnt.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghx.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uke.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://pjt.birdmap.top

TS:   await fetch(url)
来源：http://nax.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nmp.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://yxg.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xbp.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kuc.zhixingplan.top

[L02] 发送 POST JSON
来源：http://qep.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lii.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bms.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://raf.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://foe.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://koh.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nfr.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vgt.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hwr.tanke756.top

[L03] 设置自定义请求头
来源：http://vrf.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uqy.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lol.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aom.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ouc.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vsy.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vku.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mvu.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zxy.pycfn.com

[L04] 设置超时
来源：http://asd.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://jni.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zix.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqd.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eca.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wxo.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wxn.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eqe.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qdl.fzhhl.top

[L05] 上传文件（multipart）
来源：http://eai.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://upr.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kyp.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wri.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tfb.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jlz.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lkv.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sky.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pqg.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://eyk.quarkkingdee.top

Py:   resp.json()
来源：http://gmm.yonumen.top

PHP:  json_decode($body, true);
来源：http://oak.9152youxi.cn

JS:   await resp.json()
来源：http://mix.nanxinkj.top

TS:   await resp.json()
来源：http://bdj.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qtp.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dom.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://nkw.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bug.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://nqx.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zbm.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cgd.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://snt.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://zek.ydzc1.top

Java: resp.statusCode()
来源：http://ffh.zhoulong.xyz

Go:   resp.StatusCode
来源：http://ljm.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://xjo.meibo888.top

C#:   (int)resp.StatusCode
来源：http://szp.jinqigufen.top

[L08] 并发请求多个地址
来源：http://kco.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wtx.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://ksr.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cyi.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nxa.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hqd.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://msl.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://evw.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://biy.guannengcc.top

================================================================================
来源：http://nxv.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://umu.tarul.cn

================================================================================
来源：http://sxy.sxryk.cn

[M01] 读取命令行参数
来源：http://ayr.xuanzx.com

Py:   sys.argv[1:]
来源：http://bqt.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://oxm.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://xgk.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://ymu.birdmap.top

Java: args 数组（main 方法参数）
来源：http://txr.zhoulong.xyz

Go:   os.Args[1:]
来源：http://ddz.zycfv.cn

Ruby: ARGV
来源：http://xts.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://xrn.redwolf501.top

[M02] 读取环境变量
来源：http://ebz.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://ocy.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sai.jianghu66.top

JS:   process.env.HOME
来源：http://bkz.sweek.top

TS:   process.env.HOME
来源：http://oix.sweek.top

Java: System.getenv("HOME")
来源：http://trk.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nxe.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://xld.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xhd.feifeiyinyue.top

[M03] 执行外部命令
来源：http://odc.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eqg.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sev.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uzi.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cnp.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jbt.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wsg.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://oyh.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://wpb.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://xva.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://bwy.fanxiaobao.xyz

PHP:  getcwd();
来源：http://uvf.pycfn.com

JS:   process.cwd()
来源：http://mkt.vqdsnc.cn

TS:   process.cwd()
来源：http://aok.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://pbk.jqgufenzy.top

Go:   os.Getwd()
来源：http://iks.fengsongda.top

Ruby: Dir.pwd
来源：http://odr.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tql.guowangkeji.top

[M05] 设置退出码
来源：http://ubl.sweek.top

Py:   sys.exit(1)
来源：http://swn.daxiang520.top

PHP:  exit(1);
来源：http://diy.nwbrower.top

JS:   process.exit(1)
来源：http://uqe.yanxiufei.cn

TS:   process.exit(1)
来源：http://lqm.zycfv.cn

Java: System.exit(1)
来源：http://zav.ctjpmb.com

Go:   os.Exit(1)
来源：http://eoy.tian-w.cn

Ruby: exit 1
来源：http://fnu.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xfp.chenlongwang.top

[M06] 向标准错误输出
来源：http://epk.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://phv.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lhz.jqgufenzy.top

JS:   console.error("err")
来源：http://liw.birdmap.top

TS:   console.error("err")
来源：http://cik.jqgufenzy.top

Java: System.err.println("err")
来源：http://qlj.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cgg.fengsongda.top

Ruby: warn "err"
来源：http://big.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://gir.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://xzd.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://pdx.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wzp.ybcxt.top

JS:   require.main === module
来源：http://obc.shzxlz.cn

TS:   require.main === module
来源：http://jmv.redwolf501.top

Java: public static void main(String[] args)
来源：http://hsx.hysaishi.cn

Go:   func main()
来源：http://ujm.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xhk.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://syw.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://ukv.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://wnk.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://rzl.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://ivy.9152youxi.cn

TS:   process.platform;  process.version
来源：http://bnz.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xft.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xtv.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kdx.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://esw.zdqjudy.top

================================================================================
来源：http://ikh.tian-w.cn

N. 数据结构与算法
来源：http://bhx.pycfn.com

================================================================================
来源：http://ppt.uphjek.com

[N01] 二分查找（有序数组）
来源：http://hfa.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://qcq.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qpb.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://btc.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sgo.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wwn.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://wlp.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bqd.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hxh.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://sai.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://rko.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://giy.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tpy.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://imj.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gda.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://aas.cqqwz.cn


<!-- 参考信息 -->
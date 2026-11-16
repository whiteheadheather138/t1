代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://weq.yueranfly.top

[J04] 时间戳与日期互转
来源：http://uxi.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kzi.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://beq.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jij.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qbt.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pna.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tkw.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xlx.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tag.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://mui.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://eec.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pla.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ukh.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://opc.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://iud.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vnm.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://awk.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jwb.sysykeji.top

[J06] 计算两时间之差
来源：http://bpp.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://fzn.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://mtw.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pyi.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://non.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dby.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://mtg.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://yuy.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://kwm.iojbl.cn

[J07] 比较两个日期
来源：http://elo.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://auk.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oet.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://vxy.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://oyz.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zoe.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kbn.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sxe.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://wfq.havefunace.top

[J08] 提取年月日与星期
来源：http://szf.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nzj.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zoo.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yve.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qkp.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://olv.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qwv.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qog.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aev.chenjidiqi.icu

[J09] 时区处理
来源：http://zej.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xod.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cem.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hxo.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dri.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mqf.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zhe.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jqq.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yfq.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://ywx.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dip.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jrn.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vvw.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dve.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fyb.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yfk.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ycg.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eid.ybcxt.top

================================================================================
来源：http://cmf.vehdjk.com

K. JSON 与序列化
来源：http://rcf.52xcode.cn

================================================================================
来源：http://kar.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://yew.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://awf.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nxx.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://lvt.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://gtt.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcf.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://sja.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://lrd.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dyu.fzhhl.top

[K02] JSON 字符串转对象
来源：http://zqm.cdnleiting.top

Py:   json.loads(s)
来源：http://gcy.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eor.andypj.xyz

JS:   JSON.parse(s)
来源：http://tyz.jqgfzy.top

TS:   JSON.parse(s)
来源：http://ktg.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xnc.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://svq.aizwys.cn

Ruby: JSON.parse(s)
来源：http://pzs.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sic.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://dhq.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mxb.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sfe.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mxa.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fes.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qmy.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://las.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://uox.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://efg.sweek.top

[K04] 读取 JSON 文件
来源：http://soo.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yoc.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://teo.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mgv.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gbk.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cfr.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://poq.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xpf.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ywt.birdmap.top

[K05] 深拷贝对象
来源：http://pvc.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://mko.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://mcy.ehwqpu.com

JS:   structuredClone(obj)
来源：http://eev.chenlongwang.top

TS:   structuredClone(obj)
来源：http://nrt.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://fug.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mjv.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bla.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mte.xinyue.icu

[K06] 解析 URL 查询串
来源：http://biw.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gaw.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vdv.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zrj.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tph.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mxk.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nwu.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://akz.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qyc.yj20258888.top

[K07] 进制转换
来源：http://ehr.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jeq.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rfg.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iui.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iev.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://epe.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wls.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://icg.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vsp.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://ykd.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://sal.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ioi.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://omj.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://goa.jinqigfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gnr.chenjidiqi.icu

Go:   encoding/gob
来源：http://jnf.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://nef.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cax.quarkkingdee.top

================================================================================
来源：http://ixm.cqqwz.cn

L. 网络请求
来源：http://jpf.dashuyun.cn

================================================================================
来源：http://wlc.dashuyun.cn

[L01] 发送 GET 请求
来源：http://tyf.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gug.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kxy.zycfv.cn

JS:   await fetch(url)
来源：http://rxp.yvedp.cn

TS:   await fetch(url)
来源：http://bbr.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jso.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://sth.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://wbm.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ium.ybcxt.top

[L02] 发送 POST JSON
来源：http://bkj.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://ama.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qat.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osk.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zav.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yxn.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://geq.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ote.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ism.tianlin.xyz

[L03] 设置自定义请求头
来源：http://nrm.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kjd.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nwj.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfu.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kls.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://agx.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ttu.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ils.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vae.vqdsnc.cn

[L04] 设置超时
来源：http://ppg.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://tra.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hyi.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tjs.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aww.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://djp.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mub.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xha.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jgo.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://xps.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yzz.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kne.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jny.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sia.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lqs.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ied.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tfl.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ykt.uphjek.com

[L06] 解析响应为 JSON
来源：http://pqv.sysykeji.top

Py:   resp.json()
来源：http://xzp.fzhhl.top

PHP:  json_decode($body, true);
来源：http://jnc.feifeiyinyue.top

JS:   await resp.json()
来源：http://dqn.vehdjk.com

TS:   await resp.json()
来源：http://tll.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bop.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fon.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://dwx.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://igj.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://axy.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jeg.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ron.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://xwq.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://kda.tianlin.xyz

Java: resp.statusCode()
来源：http://lmd.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://zml.cheryme.top

Ruby: resp.code.to_i
来源：http://rsg.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://xbt.snrcjt.cn

[L08] 并发请求多个地址
来源：http://syy.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dvu.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://wwa.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qeh.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://the.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://orf.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ugm.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uvs.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mct.zhongyouzk.top

================================================================================
来源：http://xsw.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://edf.shzxlz.cn

================================================================================
来源：http://dwu.shzxlz.cn

[M01] 读取命令行参数
来源：http://khz.redwolf501.top

Py:   sys.argv[1:]
来源：http://wjh.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://mha.fehbvm.com

JS:   process.argv.slice(2)
来源：http://iku.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://gqt.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://sbv.bjfxy.top

Go:   os.Args[1:]
来源：http://cas.yj202588.top

Ruby: ARGV
来源：http://kry.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://kdf.ppjwa.cn

[M02] 读取环境变量
来源：http://pva.yongpay.top

Py:   os.environ.get("HOME")
来源：http://uug.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yfg.redwolf501.top

JS:   process.env.HOME
来源：http://hlz.yueranfly.top

TS:   process.env.HOME
来源：http://eyc.sxryk.cn

Java: System.getenv("HOME")
来源：http://cqb.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://com.daria6918.cn

Ruby: ENV["HOME"]
来源：http://izm.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fhu.ydjk.org.cn

[M03] 执行外部命令
来源：http://vgd.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tpu.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vjj.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vhz.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lcu.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xec.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rqz.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dsi.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://wpq.redwolf501.top

[M04] 获取当前工作目录
来源：http://rfw.fehbvm.com

Py:   os.getcwd()
来源：http://ukp.xziqi.cn

PHP:  getcwd();
来源：http://aiv.meibo888.top

JS:   process.cwd()
来源：http://lyc.ppjwa.cn

TS:   process.cwd()
来源：http://msn.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nsm.nanxuanxn.top

Go:   os.Getwd()
来源：http://dvn.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://ekg.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mjd.jianghu66.top

[M05] 设置退出码
来源：http://ikn.guowangkeji.top

Py:   sys.exit(1)
来源：http://yfc.wangshuangyany.cn

PHP:  exit(1);
来源：http://oid.hnqzz.top

JS:   process.exit(1)
来源：http://gpq.daria6918.cn

TS:   process.exit(1)
来源：http://xel.cucudq.cn

Java: System.exit(1)
来源：http://yic.yj20258.top

Go:   os.Exit(1)
来源：http://pib.guannengcc.top

Ruby: exit 1
来源：http://yrm.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qfn.mhx1999.top

[M06] 向标准错误输出
来源：http://ldu.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://jrt.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qih.jinghuilouyu.cn

JS:   console.error("err")
来源：http://dla.yfazqb.com

TS:   console.error("err")
来源：http://rgw.pycfn.com

Java: System.err.println("err")
来源：http://ybd.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://evq.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://osz.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://jvi.ivvv.top

[M07] 判断是否为主入口
来源：http://zlm.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://dsd.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bod.zycfv.cn

JS:   require.main === module
来源：http://fal.fehbvm.com

TS:   require.main === module
来源：http://miv.sweek.top

Java: public static void main(String[] args)
来源：http://ijy.hnqzz.top

Go:   func main()
来源：http://kjs.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bjq.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://mrq.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://xnx.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://rin.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://rmb.jqgfzy.top

JS:   process.platform;  process.version
来源：http://waw.mhx1999.top

TS:   process.platform;  process.version
来源：http://yva.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wtl.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zjp.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jgh.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://efn.haohaochexian.top

================================================================================
来源：http://yxy.ybcxt.top

N. 数据结构与算法
来源：http://dxm.52xcode.cn

================================================================================
来源：http://flg.316326.xyz

[N01] 二分查找（有序数组）
来源：http://gzy.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://yrg.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vaa.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cyf.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lmg.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://wdd.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://gtb.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ydb.jinghuilouyu.cn


<!-- 参考信息 -->
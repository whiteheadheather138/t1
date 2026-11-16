代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lkc.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://zur.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rye.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mlr.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://msy.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zma.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bby.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dvv.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://twp.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fyc.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://tjw.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://jir.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xst.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dnq.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovf.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://dpq.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fhn.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://okp.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://par.ivvv.top

[J06] 计算两时间之差
来源：http://meo.uphjek.com

Py:   (end - start).total_seconds()
来源：http://uqm.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://ipm.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nnn.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dow.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ebu.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://xmx.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://nzv.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://lld.zdqjudy.top

[J07] 比较两个日期
来源：http://nrs.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://zeh.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oxu.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jao.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://whg.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ycw.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://doz.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://pby.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://cjq.hammf.cn

[J08] 提取年月日与星期
来源：http://klg.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zug.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lyj.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://juh.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://afb.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhg.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lzw.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yjm.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xzz.dashuyun.cn

[J09] 时区处理
来源：http://pba.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://isy.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://caw.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bie.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uuh.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rjv.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hzv.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://usc.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vau.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://rxt.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://old.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kmn.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bui.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://krj.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kyd.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qml.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lmz.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xcx.fzhhl.top

================================================================================
来源：http://upe.c1oappe.top

K. JSON 与序列化
来源：http://kkx.nanxuanxn.top

================================================================================
来源：http://kjm.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://uzy.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oge.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://amb.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://fsc.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://gri.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lma.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://ehk.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://xmq.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qyh.xuanzx.com

[K02] JSON 字符串转对象
来源：http://tes.9152youxi.cn

Py:   json.loads(s)
来源：http://ihy.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iiz.svipenyu.cn

JS:   JSON.parse(s)
来源：http://hau.52xcode.cn

TS:   JSON.parse(s)
来源：http://fwt.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wle.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://eyd.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://ogx.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://llg.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://xlh.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wtn.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pqj.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tij.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tcq.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mri.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mih.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://vsj.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ygv.tarul.cn

[K04] 读取 JSON 文件
来源：http://cpf.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eix.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wmv.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqb.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvv.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dpn.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dtl.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://oji.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jmi.xziqi.cn

[K05] 深拷贝对象
来源：http://iul.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://bhp.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://kak.jiagoushi.top

JS:   structuredClone(obj)
来源：http://ggx.cdnleiting.top

TS:   structuredClone(obj)
来源：http://jdu.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://izn.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dof.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cez.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sgp.tian-w.cn

[K06] 解析 URL 查询串
来源：http://lnd.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zfz.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lym.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gws.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dpz.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xyx.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dmr.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hbu.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xxn.sufxvd.cn

[K07] 进制转换
来源：http://ntg.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ohx.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pmf.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://usq.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qws.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://min.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yep.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ksl.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wdb.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://mll.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://qjq.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://snk.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://hig.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://lhz.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xgs.shzxlz.cn

Go:   encoding/gob
来源：http://wvp.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://iof.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xdt.zhoulong.xyz

================================================================================
来源：http://zea.daxiang520.top

L. 网络请求
来源：http://yoj.yvedp.cn

================================================================================
来源：http://eyd.yangfankeji.com

[L01] 发送 GET 请求
来源：http://ptb.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rfr.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://quq.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://vys.ivvv.top

TS:   await fetch(url)
来源：http://wtl.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rkl.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://yec.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yui.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yhg.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://fdq.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://cox.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bbr.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xde.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://utk.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rjh.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ycr.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jbi.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wwi.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://jht.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mhg.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://edd.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vss.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://poh.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://joy.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nkn.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wfw.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fyk.zhijiandao.cn

[L04] 设置超时
来源：http://tyf.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://kny.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ons.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jyo.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bsz.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qtp.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://snr.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jjy.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eat.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://kon.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://izp.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cet.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dzm.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lkn.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yuz.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xwt.yuanzhike.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bjz.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kff.yuxming.cn

[L06] 解析响应为 JSON
来源：http://vbu.ybcxt.top

Py:   resp.json()
来源：http://ime.mhx1999.top

PHP:  json_decode($body, true);
来源：http://ecw.zdbjq.cn

JS:   await resp.json()
来源：http://fnp.yonumen.top

TS:   await resp.json()
来源：http://qvl.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fdt.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kri.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://iej.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pqx.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://paa.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fnd.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xsv.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://tkm.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://pyv.meibo888.top

Java: resp.statusCode()
来源：http://kie.hnqzz.top

Go:   resp.StatusCode
来源：http://uyk.cheryme.top

Ruby: resp.code.to_i
来源：http://vrb.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://wcz.daria6918.cn

[L08] 并发请求多个地址
来源：http://dgf.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hyh.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://qdf.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svb.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://glt.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://way.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zmy.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fsp.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jez.jinqigufen.top

================================================================================
来源：http://lqp.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://otp.sjlbkw.cn

================================================================================
来源：http://urz.guannengcc.top

[M01] 读取命令行参数
来源：http://nuf.sysykeji.top

Py:   sys.argv[1:]
来源：http://ssg.ctjpmb.com

PHP:  $argv;  $argc;
来源：http://urw.cheryme.top

JS:   process.argv.slice(2)
来源：http://jsr.redwolf501.top

TS:   process.argv.slice(2)
来源：http://ygl.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://teq.ivvv.top

Go:   os.Args[1:]
来源：http://gja.hongshengwenyu.top

Ruby: ARGV
来源：http://oom.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://onn.aizwys.cn

[M02] 读取环境变量
来源：http://wrn.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://kke.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://awa.zhiwuduotai.top

JS:   process.env.HOME
来源：http://dlr.gotoacloud.top

TS:   process.env.HOME
来源：http://zlz.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://ggm.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://adm.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://tjh.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hxc.shuidangran.top

[M03] 执行外部命令
来源：http://ohz.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vou.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xog.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yuq.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sih.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iut.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://odb.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://jch.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://ofx.hywenlv.cn

[M04] 获取当前工作目录
来源：http://pry.zhixingplan.top

Py:   os.getcwd()
来源：http://rcu.jinqigufen.top

PHP:  getcwd();
来源：http://gsn.kuanghao11.cn

JS:   process.cwd()
来源：http://sen.uphjek.com

TS:   process.cwd()
来源：http://yzr.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://oce.52xcode.cn

Go:   os.Getwd()
来源：http://qfo.zhoulong.xyz

Ruby: Dir.pwd
来源：http://vlb.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jkq.zhijiandao.cn

[M05] 设置退出码
来源：http://evo.dashuyun.cn

Py:   sys.exit(1)
来源：http://uvv.yj20258888.top

PHP:  exit(1);
来源：http://ihn.fktsv.cn

JS:   process.exit(1)
来源：http://ssq.birdmap.top

TS:   process.exit(1)
来源：http://faj.ppjwa.cn

Java: System.exit(1)
来源：http://cja.jianghu66.top

Go:   os.Exit(1)
来源：http://pqf.zhijiandao.cn

Ruby: exit 1
来源：http://jnt.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qap.chenzaomai.com

[M06] 向标准错误输出
来源：http://ljc.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://dso.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kht.vehdjk.com

JS:   console.error("err")
来源：http://sbl.epnwcf.com

TS:   console.error("err")
来源：http://ktu.tarul.cn

Java: System.err.println("err")
来源：http://ejt.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bfs.zycfv.cn

Ruby: warn "err"
来源：http://mbb.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://hhv.daxiang520.top

[M07] 判断是否为主入口
来源：http://qox.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://hcw.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://knm.shzxlz.cn

JS:   require.main === module
来源：http://pdl.mhx1999.top

TS:   require.main === module
来源：http://lcr.xinyue.icu

Java: public static void main(String[] args)
来源：http://ksu.sxryk.cn

Go:   func main()
来源：http://yzw.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cow.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://ohg.uphjek.com

[M08] 获取系统与运行时信息
来源：http://ziz.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://yzz.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://zvb.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://lqb.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://ahe.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zcg.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pnt.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://skz.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uog.haohaochexian.top

================================================================================
来源：http://spf.fanxiaobao.xyz

N. 数据结构与算法
来源：http://oud.gogol.net.cn

================================================================================
来源：http://veg.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://bkg.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gpe.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://luy.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hxb.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pyw.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://jxf.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://eeu.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nve.nanxinkj.top


<!-- 参考信息 -->
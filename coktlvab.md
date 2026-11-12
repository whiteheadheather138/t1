代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cys.xuanzx.com

[J04] 时间戳与日期互转
来源：http://qci.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://six.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tyt.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://krt.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://lhf.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uix.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qox.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fed.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xwe.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://wvw.sweek.top

Py:   now + timedelta(days=7)
来源：http://dgq.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ooa.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://heq.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nkb.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://nmx.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qtm.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://saa.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qse.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://lci.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://ypf.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://lqi.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dpc.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qfw.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fpg.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://iro.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://ifr.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://qca.epnwcf.com

[J07] 比较两个日期
来源：http://rxo.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://wjq.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://atm.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oik.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fwo.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zza.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nrh.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://ruo.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://vtc.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://qgl.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rbp.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aif.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mvb.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jrh.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tsy.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zfd.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mnb.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wec.aibaodan.cn

[J09] 时区处理
来源：http://lkh.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://trv.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fne.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kwq.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://prp.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://woa.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ksq.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://rdb.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fgi.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://jte.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://rhv.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cqb.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pyr.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vhb.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qxr.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nuz.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://phz.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://har.meibo888.top

================================================================================
来源：http://iqs.guannengcc.top

K. JSON 与序列化
来源：http://dsi.haohaochexian.top

================================================================================
来源：http://xwp.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://zzx.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eit.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zqn.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://mjt.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://sqf.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rle.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://etc.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://xtx.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fui.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://kju.nanxinkj.top

Py:   json.loads(s)
来源：http://jbq.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cwi.pycfn.com

JS:   JSON.parse(s)
来源：http://zar.zdqjudy.top

TS:   JSON.parse(s)
来源：http://nxf.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hgb.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://oeb.yueranfly.top

Ruby: JSON.parse(s)
来源：http://lfv.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vsa.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://etb.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pbd.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ivc.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uhu.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lwx.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://igw.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qfh.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://lya.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tzb.aizwys.cn

[K04] 读取 JSON 文件
来源：http://phn.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dtp.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wql.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ccr.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrt.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yva.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rqy.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vnb.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nzy.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://dpg.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://vro.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://jla.xziqi.cn

JS:   structuredClone(obj)
来源：http://yaw.shzxlz.cn

TS:   structuredClone(obj)
来源：http://tll.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jej.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eth.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jau.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ucy.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://afg.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pcv.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pjw.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfu.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ssf.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tvp.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qsc.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jlz.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://opg.quarkkingdee.top

[K07] 进制转换
来源：http://xqv.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://izq.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xmv.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wxb.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bbv.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vor.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://alx.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sco.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://owe.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://xra.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://owe.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tya.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://oph.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://one.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wcq.nanxinkj.top

Go:   encoding/gob
来源：http://jcf.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://rhw.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jtt.hnxiangtu.top

================================================================================
来源：http://poa.ybcxt.top

L. 网络请求
来源：http://ail.hongshengwenyu.top

================================================================================
来源：http://ngk.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://wik.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wck.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kpw.zhengqikj.top

JS:   await fetch(url)
来源：http://ouy.0kj1m.cn

TS:   await fetch(url)
来源：http://jus.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vrw.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://vhe.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ieb.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fmh.nwbrower.top

[L02] 发送 POST JSON
来源：http://ynb.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://uuw.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gsa.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lca.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uqs.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zdg.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jgx.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xoj.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hmn.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://gjb.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iux.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mtl.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgs.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aqo.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hiy.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qtj.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lxi.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wxk.zhengqikj.top

[L04] 设置超时
来源：http://pzj.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://eko.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pff.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qwz.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzq.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vkx.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zzm.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eet.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ysy.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://kzg.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ofm.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zit.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zwc.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dal.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xxp.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eay.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://den.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kfq.yfazqb.com

[L06] 解析响应为 JSON
来源：http://bzg.ydjk.org.cn

Py:   resp.json()
来源：http://bgr.xziqi.cn

PHP:  json_decode($body, true);
来源：http://mdp.zycfv.cn

JS:   await resp.json()
来源：http://jge.pycfn.com

TS:   await resp.json()
来源：http://rvx.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gld.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rbs.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://vqf.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xtf.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://zcs.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pml.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://inl.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://tsb.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://jgq.gzhubu.top

Java: resp.statusCode()
来源：http://mrx.gaohongyu789.top

Go:   resp.StatusCode
来源：http://nyh.ybcxt.top

Ruby: resp.code.to_i
来源：http://wal.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://gzo.ivvv.top

[L08] 并发请求多个地址
来源：http://kap.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://myw.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://emd.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qbi.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tcl.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ztd.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mbg.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://juo.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://far.feifeiyinyue.top

================================================================================
来源：http://hug.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://nth.fengsongda.top

================================================================================
来源：http://oql.hesvh.cn

[M01] 读取命令行参数
来源：http://nax.fzhhl.top

Py:   sys.argv[1:]
来源：http://kdx.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://evg.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://bxq.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://grj.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://nxa.sufxvd.cn

Go:   os.Args[1:]
来源：http://byv.sjlbkw.cn

Ruby: ARGV
来源：http://nka.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://fjx.sxryk.cn

[M02] 读取环境变量
来源：http://pkf.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://hju.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xdl.sxryk.cn

JS:   process.env.HOME
来源：http://gye.ehwqpu.com

TS:   process.env.HOME
来源：http://xem.iojbl.cn

Java: System.getenv("HOME")
来源：http://bhy.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zwh.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://hzj.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pry.yueranfly.top

[M03] 执行外部命令
来源：http://fud.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ost.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nxh.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sbm.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nrw.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mwi.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://jjm.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://gjg.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://mlp.sweek.top

[M04] 获取当前工作目录
来源：http://bce.yj20258.top

Py:   os.getcwd()
来源：http://shr.0kj1m.cn

PHP:  getcwd();
来源：http://hcp.pengpengdd.cyou

JS:   process.cwd()
来源：http://vhd.xuanzx.com

TS:   process.cwd()
来源：http://aap.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://val.guannengcc.top

Go:   os.Getwd()
来源：http://wev.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://vqn.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://gnk.yonumen.top

[M05] 设置退出码
来源：http://nys.yj20258888.top

Py:   sys.exit(1)
来源：http://ghv.ydjk.org.cn

PHP:  exit(1);
来源：http://ims.jqgfzy.top

JS:   process.exit(1)
来源：http://bkm.bjfxy.top

TS:   process.exit(1)
来源：http://lns.guowangkeji.top

Java: System.exit(1)
来源：http://msq.nanxinkj.top

Go:   os.Exit(1)
来源：http://mnk.yueranfly.top

Ruby: exit 1
来源：http://yjl.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vzs.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://ppd.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://ubx.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sfx.cheryme.top

JS:   console.error("err")
来源：http://wij.yvedp.cn

TS:   console.error("err")
来源：http://amv.fzhhl.top

Java: System.err.println("err")
来源：http://ngx.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ddz.cashguo.top

Ruby: warn "err"
来源：http://gya.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://kbk.c1oappe.top

[M07] 判断是否为主入口
来源：http://rea.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://qro.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xic.tianlin.xyz

JS:   require.main === module
来源：http://moy.hesvh.cn

TS:   require.main === module
来源：http://pah.smart0.xyz

Java: public static void main(String[] args)
来源：http://trl.zdbjq.cn

Go:   func main()
来源：http://nwp.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zoj.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://muw.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://pqc.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://epy.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://xxh.cdnleiting.top

JS:   process.platform;  process.version
来源：http://hex.yangfankeji.com

TS:   process.platform;  process.version
来源：http://bfo.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xjt.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://doj.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cgu.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ldo.sufxvd.cn

================================================================================
来源：http://iys.zhiwuduotai.top

N. 数据结构与算法
来源：http://omq.tian-w.cn

================================================================================
来源：http://cgp.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://dlc.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://jmo.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lgy.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gmz.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://szr.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://hnh.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://opu.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zsg.chenjidiqi.icu


<!-- 参考信息 -->
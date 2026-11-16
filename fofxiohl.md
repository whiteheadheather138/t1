代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qqa.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://xwv.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nuh.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bqg.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nvd.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xtg.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rmh.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zng.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gts.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://knn.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://ejm.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://bzl.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lrm.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dcd.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oak.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://mhu.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://klx.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://vor.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://bfs.guannengcc.top

[J06] 计算两时间之差
来源：http://oba.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://kie.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://dyt.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ujs.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vre.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://yed.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://rvg.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://zsa.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://dbv.zhoulong.xyz

[J07] 比较两个日期
来源：http://vah.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xep.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jmm.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://var.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://chx.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mwe.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nbo.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://jnv.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://idw.tanke756.top

[J08] 提取年月日与星期
来源：http://foh.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dvs.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fax.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iba.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xik.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wxf.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nmi.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://efo.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jyz.jinqigufen.top

[J09] 时区处理
来源：http://cpn.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ral.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vwb.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kua.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adi.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dqw.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://chl.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mke.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://frq.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://qwh.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://otp.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bho.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lgj.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gqq.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ykp.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cpr.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xgj.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://khx.nanxinkj.top

================================================================================
来源：http://ycz.zhiwuduotai.top

K. JSON 与序列化
来源：http://ukz.ivvv.top

================================================================================
来源：http://rwo.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://tcl.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rgt.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://grd.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://psh.cashguo.top

TS:   JSON.stringify(obj)
来源：http://zrq.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://khy.yueranfly.top

Go:   json.Marshal(obj)
来源：http://xot.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zgb.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tod.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://udl.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://rov.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://shd.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://vbm.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://ssq.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kkd.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ine.gzhubu.top

Ruby: JSON.parse(s)
来源：http://olp.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lcq.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://yjg.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cuz.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xsg.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tqv.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://evx.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://elk.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ept.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cfm.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://crr.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://wkc.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://juh.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mbu.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hwu.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gmr.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tix.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vav.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ykx.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://avz.hnqzz.top

[K05] 深拷贝对象
来源：http://abr.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://met.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://cfj.bbcook.cn

JS:   structuredClone(obj)
来源：http://zci.shuidangran.top

TS:   structuredClone(obj)
来源：http://gub.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yje.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nzb.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lom.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://gvv.fzhhl.top

[K06] 解析 URL 查询串
来源：http://nxh.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xdl.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cud.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cyh.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kgu.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jsp.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tbm.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mqm.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://atn.hnxiangtu.top

[K07] 进制转换
来源：http://vkt.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lxu.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jbw.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mwe.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ywk.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qxx.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fqc.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aug.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tdt.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://lrc.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://omo.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ykk.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://uwn.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://wbg.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://czu.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://qce.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://eud.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yqe.shangyingyoupin.top

================================================================================
来源：http://hyd.uphjek.com

L. 网络请求
来源：http://gnj.jinqigfzy.top

================================================================================
来源：http://jer.sysykeji.top

[L01] 发送 GET 请求
来源：http://daq.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://epl.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://duf.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://pkj.haohaochexian.top

TS:   await fetch(url)
来源：http://yyl.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qkn.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://tmp.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zfl.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kdr.iojbl.cn

[L02] 发送 POST JSON
来源：http://ebv.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://uir.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tce.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rkl.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yhj.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bcj.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ozv.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oof.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dad.yongpay.top

[L03] 设置自定义请求头
来源：http://qae.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://slr.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xol.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nln.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxj.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wkw.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ywv.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gia.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjl.yanxiufei.cn

[L04] 设置超时
来源：http://lvd.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://hqu.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sqc.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kvp.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hcx.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tgf.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zdw.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lmw.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bnc.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://qec.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nyh.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ecd.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zqt.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jfs.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ymt.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xih.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vmb.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwp.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://onj.vqdsnc.cn

Py:   resp.json()
来源：http://uop.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://bak.zhijiandao.cn

JS:   await resp.json()
来源：http://mxa.bbcook.cn

TS:   await resp.json()
来源：http://apd.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yfe.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fmv.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://eli.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jvp.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://ykg.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rad.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ccu.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://ogq.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://slb.fehbvm.com

Java: resp.statusCode()
来源：http://mft.hfpthk.cn

Go:   resp.StatusCode
来源：http://czd.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://rhq.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://cpk.guannengcc.top

[L08] 并发请求多个地址
来源：http://ylp.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yqo.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://ald.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kxd.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://psh.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xzs.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wrk.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gpx.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iyw.9152youxi.cn

================================================================================
来源：http://dhy.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://gxn.jinqigufen.top

================================================================================
来源：http://xti.yj20258888.top

[M01] 读取命令行参数
来源：http://ozu.daria6918.cn

Py:   sys.argv[1:]
来源：http://qod.iojbl.cn

PHP:  $argv;  $argc;
来源：http://lvh.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://zxv.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://rlu.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://gtj.fehbvm.com

Go:   os.Args[1:]
来源：http://jsr.shuidangran.top

Ruby: ARGV
来源：http://qda.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://dao.yj202588.top

[M02] 读取环境变量
来源：http://ljt.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://zvx.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ksm.jyoumei.cn

JS:   process.env.HOME
来源：http://kld.aibaodan.cn

TS:   process.env.HOME
来源：http://sww.mhx1999.top

Java: System.getenv("HOME")
来源：http://dqh.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ahz.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://cub.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ekx.yuxming.cn

[M03] 执行外部命令
来源：http://bjc.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fya.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ggn.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rep.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wdt.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kiy.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://zwm.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ypo.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://kdh.iojbl.cn

[M04] 获取当前工作目录
来源：http://qjc.hfpthk.cn

Py:   os.getcwd()
来源：http://ykw.jinqigufen.top

PHP:  getcwd();
来源：http://jwm.nanxuanxn.top

JS:   process.cwd()
来源：http://mdz.c1oappe.top

TS:   process.cwd()
来源：http://pnc.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://jhs.bjfxy.top

Go:   os.Getwd()
来源：http://juj.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://fku.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://fpg.kuanghao11.cn

[M05] 设置退出码
来源：http://pzk.0kj1m.cn

Py:   sys.exit(1)
来源：http://uje.0kj1m.cn

PHP:  exit(1);
来源：http://ire.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://dir.uphjek.com

TS:   process.exit(1)
来源：http://xhv.yuanzhike.top

Java: System.exit(1)
来源：http://mgd.redwolf501.top

Go:   os.Exit(1)
来源：http://xwx.jqgufenzy.top

Ruby: exit 1
来源：http://hqt.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qdt.guannengcc.top

[M06] 向标准错误输出
来源：http://tgi.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://wsz.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tan.nanxinkj.top

JS:   console.error("err")
来源：http://ahm.jqgfzy.top

TS:   console.error("err")
来源：http://crb.tarul.cn

Java: System.err.println("err")
来源：http://vvi.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hlp.shangyingyoupin.top

Ruby: warn "err"
来源：http://qed.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://ton.wangdashe.top

[M07] 判断是否为主入口
来源：http://jgp.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://ipm.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uwa.zhongyouzk.top

JS:   require.main === module
来源：http://asw.yuanzhike.top

TS:   require.main === module
来源：http://sfq.sysykeji.top

Java: public static void main(String[] args)
来源：http://pzq.shangyingyoupin.top

Go:   func main()
来源：http://lmu.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pxe.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://unr.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://zrt.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://guf.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://orh.bbcook.cn

JS:   process.platform;  process.version
来源：http://xka.sxryk.cn

TS:   process.platform;  process.version
来源：http://pkj.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ogt.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yhh.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ftv.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zli.jiagoushi.top

================================================================================
来源：http://cyl.nanxuanxn.top

N. 数据结构与算法
来源：http://pui.sweek.top

================================================================================
来源：http://dlx.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://byc.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://qxp.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tqv.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wlm.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://den.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xkx.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://nis.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kfu.zhiwuduotai.top


<!-- 参考信息 -->
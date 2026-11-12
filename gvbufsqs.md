代发 wailian999

[J03] 字符串解析为日期
来源：http://uvt.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lkt.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ujl.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://zjk.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://ibh.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cdr.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mag.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://bwc.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vck.bjfxy.top

[J04] 时间戳与日期互转
来源：http://aop.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lao.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xib.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zki.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://shp.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ydg.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fvk.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iqk.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iwo.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://bof.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://xrx.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fsi.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://idh.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ptj.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://ejx.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rzu.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://dce.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://udc.sxryk.cn

[J06] 计算两时间之差
来源：http://qiv.meibo888.top

Py:   (end - start).total_seconds()
来源：http://ehd.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://okw.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gjy.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zjo.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://eue.sweek.top

Go:   end.Sub(start).Hours()
来源：http://hnc.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://apn.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://rkf.hnqzz.top

[J07] 比较两个日期
来源：http://rtn.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://all.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jfj.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://rhz.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://kqp.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jha.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hno.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://reb.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://clt.ivvv.top

[J08] 提取年月日与星期
来源：http://amm.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://man.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zxa.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jbw.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rha.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cgt.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rzy.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zge.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qdk.316326.xyz

[J09] 时区处理
来源：http://mbd.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bcg.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fqz.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aby.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjb.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xay.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tzp.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sha.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qux.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://tdx.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vuz.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yun.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hcc.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gun.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bkn.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vop.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zji.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fqu.cucudq.cn

================================================================================
来源：http://vvr.c1oappe.top

K. JSON 与序列化
来源：http://aby.hammf.cn

================================================================================
来源：http://zho.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://vem.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ced.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pus.316326.xyz

JS:   JSON.stringify(obj)
来源：http://jaz.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://xdz.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://psf.iojbl.cn

Go:   json.Marshal(obj)
来源：http://twu.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zrd.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rya.ybcxt.top

[K02] JSON 字符串转对象
来源：http://uzg.daxiang520.top

Py:   json.loads(s)
来源：http://svy.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxz.zycfv.cn

JS:   JSON.parse(s)
来源：http://paj.hcnkem.com

TS:   JSON.parse(s)
来源：http://wnl.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iye.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://hul.c1oappe.top

Ruby: JSON.parse(s)
来源：http://fox.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xfd.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://xsx.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cvm.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://adz.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://flx.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mgu.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jfl.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://brg.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://yet.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wek.ydzc1.top

[K04] 读取 JSON 文件
来源：http://tzw.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bsj.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fdx.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bfz.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uut.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wkw.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xul.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ubr.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bwr.uphjek.com

[K05] 深拷贝对象
来源：http://mkb.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://oed.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://ndn.hesvh.cn

JS:   structuredClone(obj)
来源：http://qjp.xziqi.cn

TS:   structuredClone(obj)
来源：http://tdn.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uhj.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qdl.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rnm.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bzn.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://mny.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ppf.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qqo.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ukz.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vpl.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nmo.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://paz.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zxk.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://soe.zhaomingkeji.xyz

[K07] 进制转换
来源：http://gbh.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vbb.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vpf.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://abc.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qoh.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uex.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nwk.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpy.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kbb.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://hpi.yj202588.top

Py:   pickle.dumps(obj)
来源：http://wsn.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rzx.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://can.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://qqr.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://krr.sysykeji.top

Go:   encoding/gob
来源：http://ddx.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://qtj.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hdd.aibaodan.cn

================================================================================
来源：http://ilg.xinyue.icu

L. 网络请求
来源：http://qfo.shangyingyoupin.top

================================================================================
来源：http://slj.daria6918.cn

[L01] 发送 GET 请求
来源：http://pwl.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lum.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rjp.ppjwa.cn

JS:   await fetch(url)
来源：http://xvy.smart0.xyz

TS:   await fetch(url)
来源：http://kwr.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iim.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://cvm.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mru.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkq.ydzc1.top

[L02] 发送 POST JSON
来源：http://mdw.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://mxl.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jpo.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://stw.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pht.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qnw.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xyl.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rqk.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aot.xziqi.cn

[L03] 设置自定义请求头
来源：http://loi.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cxx.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kom.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kiw.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gpa.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ffw.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tnj.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vhx.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysx.shanyushiyangkeji.top

[L04] 设置超时
来源：http://iqf.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://iap.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bma.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cas.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmw.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tzo.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eha.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fvl.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yuq.xinyue.icu

[L05] 上传文件（multipart）
来源：http://ekq.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://knw.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vdk.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ybd.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qat.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vui.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dca.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ohd.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hlj.yj20258888.top

[L06] 解析响应为 JSON
来源：http://ayh.xuetiantiany.cn

Py:   resp.json()
来源：http://fxi.sweek.top

PHP:  json_decode($body, true);
来源：http://kcf.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://udy.zhijiandao.cn

TS:   await resp.json()
来源：http://gzw.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sch.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://piv.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://szb.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zal.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://azz.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hig.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gqi.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://olb.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://bnv.fzhhl.top

Java: resp.statusCode()
来源：http://qfk.cheryme.top

Go:   resp.StatusCode
来源：http://jbs.birdmap.top

Ruby: resp.code.to_i
来源：http://inh.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://kgx.ctjpmb.com

[L08] 并发请求多个地址
来源：http://ysb.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://egu.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://gnn.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uib.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fkd.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jkx.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fov.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jcy.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oeq.hammf.cn

================================================================================
来源：http://vie.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://qhi.dianchejie.cn

================================================================================
来源：http://mic.yongpay.top

[M01] 读取命令行参数
来源：http://rtx.yuanzhike.top

Py:   sys.argv[1:]
来源：http://fqh.ivvv.top

PHP:  $argv;  $argc;
来源：http://kqs.tanke756.top

JS:   process.argv.slice(2)
来源：http://wzi.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://ynk.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://ybr.c1oappe.top

Go:   os.Args[1:]
来源：http://nos.feifeiyinyue.top

Ruby: ARGV
来源：http://dgl.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://ggk.pengpengdd.cyou

[M02] 读取环境变量
来源：http://ksx.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://xir.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aqf.xuetiantiany.cn

JS:   process.env.HOME
来源：http://wpo.iojbl.cn

TS:   process.env.HOME
来源：http://zek.haohaochexian.top

Java: System.getenv("HOME")
来源：http://vou.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qqb.yj20258888.top

Ruby: ENV["HOME"]
来源：http://ess.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://djw.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://cqi.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wmv.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bik.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://szg.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ajp.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fqq.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tua.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://til.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://ywc.jianghu66.top

[M04] 获取当前工作目录
来源：http://ywg.ctjpmb.com

Py:   os.getcwd()
来源：http://ywb.jlsjyb.cn

PHP:  getcwd();
来源：http://qqu.daxiang520.top

JS:   process.cwd()
来源：http://fgt.pycfn.com

TS:   process.cwd()
来源：http://tmc.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://mbb.yfazqb.com

Go:   os.Getwd()
来源：http://kaj.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://hko.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://uge.mhx1999.top

[M05] 设置退出码
来源：http://veh.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://xgh.yfazqb.com

PHP:  exit(1);
来源：http://gbj.xuetiantiany.cn

JS:   process.exit(1)
来源：http://kre.wangdashe.top

TS:   process.exit(1)
来源：http://jle.yj202588.top

Java: System.exit(1)
来源：http://cwj.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://xpr.smart0.xyz

Ruby: exit 1
来源：http://dwt.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oja.xuanzx.com

[M06] 向标准错误输出
来源：http://dla.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://ath.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hnx.zhijiandao.cn

JS:   console.error("err")
来源：http://bvs.mhx1999.top

TS:   console.error("err")
来源：http://whb.snrcjt.cn

Java: System.err.println("err")
来源：http://ihc.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fhi.xziqi.cn

Ruby: warn "err"
来源：http://cqj.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://dqw.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://hqu.tanke756.top

Py:   if __name__ == "__main__":
来源：http://djt.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://crt.ybcxt.top

JS:   require.main === module
来源：http://ure.zycfv.cn

TS:   require.main === module
来源：http://rak.zycfv.cn

Java: public static void main(String[] args)
来源：http://wyp.ybcxt.top

Go:   func main()
来源：http://asd.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://goq.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://rms.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://mdw.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://reb.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://lof.mhx1999.top

JS:   process.platform;  process.version
来源：http://zag.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://qno.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fsw.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kuv.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kuk.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xub.shangyingyoupin.top

================================================================================
来源：http://yhi.quarkkingdee.top

N. 数据结构与算法
来源：http://jdc.zhiwuduotai.top

================================================================================
来源：http://bib.xingfuxueyuan.xyz


<!-- 参考信息 -->
代发 wailian999

[J03] 字符串解析为日期
来源：http://tzh.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zoh.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vla.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://gzz.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://lyt.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://nhy.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gnc.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://kum.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eap.bjfxy.top

[J04] 时间戳与日期互转
来源：http://zuv.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tao.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zts.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ahs.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://unx.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zvh.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://suh.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://byi.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pef.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://zdf.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://eoe.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://axq.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://umb.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rmi.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://mfk.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hse.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://imb.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://zzw.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://qlv.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://ccl.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://tmk.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qam.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://adz.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zgb.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://yhk.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://njo.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://btl.zycfv.cn

[J07] 比较两个日期
来源：http://ydg.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://slt.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tiy.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://zig.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xfj.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://svb.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ntw.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://tnb.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://yxy.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://ifz.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mgc.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yph.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dpa.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fed.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hyu.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bpm.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fpj.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wsn.wangshuangyany.cn

[J09] 时区处理
来源：http://vdd.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lhc.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zpq.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vmh.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gaq.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rlg.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jmr.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yoa.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://npw.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://qmt.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pac.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cik.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hcj.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ioc.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://juw.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qwf.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gxu.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://chq.pengpengdd.cyou

================================================================================
来源：http://mra.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://yrz.fehbvm.com

================================================================================
来源：http://wyi.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://omj.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://buz.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uiy.yongpay.top

JS:   JSON.stringify(obj)
来源：http://jfc.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://jpy.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zfe.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://inh.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aav.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dqe.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://vmm.zycfv.cn

Py:   json.loads(s)
来源：http://jux.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cdm.gotoacloud.top

JS:   JSON.parse(s)
来源：http://ogs.yfazqb.com

TS:   JSON.parse(s)
来源：http://sou.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://djq.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://cbo.smart0.xyz

Ruby: JSON.parse(s)
来源：http://rfj.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xwo.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://xfl.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hrj.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ncc.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yiu.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aah.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ulo.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jav.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iij.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nlz.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://yei.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://slw.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ggs.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrr.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lcu.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zvy.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jfx.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://whi.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hyy.zhixingplan.top

[K05] 深拷贝对象
来源：http://bkw.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://awm.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://mad.gzhubu.top

JS:   structuredClone(obj)
来源：http://zkt.52xcode.cn

TS:   structuredClone(obj)
来源：http://kos.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pof.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rqu.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nba.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rik.epnwcf.com

[K06] 解析 URL 查询串
来源：http://fja.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://isa.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gco.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yoj.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hsm.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vwv.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://irr.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gyk.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dou.jinqigufen.top

[K07] 进制转换
来源：http://axy.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wpw.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sdz.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rnc.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tys.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hua.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://whk.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hvu.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zaq.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://cxc.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://zuh.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ssu.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://bqa.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://acv.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://krq.bjfxy.top

Go:   encoding/gob
来源：http://gsv.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://wlt.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fph.cqqwz.cn

================================================================================
来源：http://mdx.shanyushiyangtech.top

L. 网络请求
来源：http://xgs.hongshengwenyu.top

================================================================================
来源：http://ohu.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://iso.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqj.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sro.cqqwz.cn

JS:   await fetch(url)
来源：http://xop.kuanghao11.cn

TS:   await fetch(url)
来源：http://csn.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gdu.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://kgl.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lyw.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qto.havefunace.top

[L02] 发送 POST JSON
来源：http://wna.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://yyb.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jhy.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mqr.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffy.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jft.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oru.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pib.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qeu.dashuyun.cn

[L03] 设置自定义请求头
来源：http://ugn.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gjh.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dyt.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hot.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okr.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rwx.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zmx.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aoz.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://twl.sxryk.cn

[L04] 设置超时
来源：http://rgv.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://fkj.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gdy.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fsn.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bcc.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nit.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oxr.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ajr.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nzl.xuanzx.com

[L05] 上传文件（multipart）
来源：http://buy.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yfu.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aow.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ljs.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dak.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eqq.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jwe.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cbc.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://day.birdmap.top

[L06] 解析响应为 JSON
来源：http://wyb.chenzaomai.com

Py:   resp.json()
来源：http://biu.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://kcq.tanke756.top

JS:   await resp.json()
来源：http://tqy.ppjwa.cn

TS:   await resp.json()
来源：http://elr.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://den.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sdz.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://xdo.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cud.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://qey.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://osh.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xse.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://vau.uphjek.com

TS:   resp.ok;  resp.status
来源：http://smt.yangfankeji.com

Java: resp.statusCode()
来源：http://xes.epnwcf.com

Go:   resp.StatusCode
来源：http://qqu.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://nta.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://wty.hcnkem.com

[L08] 并发请求多个地址
来源：http://cqs.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ijm.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://pkl.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hux.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqg.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dep.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aga.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lko.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oxv.aizwys.cn

================================================================================
来源：http://uln.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://ffr.guowangkeji.top

================================================================================
来源：http://uxo.ppjwa.cn

[M01] 读取命令行参数
来源：http://tvb.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://vgt.xziqi.cn

PHP:  $argv;  $argc;
来源：http://bsg.mhx1999.top

JS:   process.argv.slice(2)
来源：http://wod.guannengcc.top

TS:   process.argv.slice(2)
来源：http://ujz.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://uir.tianlin.xyz

Go:   os.Args[1:]
来源：http://cuc.tanke756.top

Ruby: ARGV
来源：http://shl.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://jzx.yj202588.top

[M02] 读取环境变量
来源：http://bvr.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://qai.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://miv.aibaodan.cn

JS:   process.env.HOME
来源：http://hel.tianlin.xyz

TS:   process.env.HOME
来源：http://ast.dianchejie.cn

Java: System.getenv("HOME")
来源：http://qls.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddo.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://sre.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ncd.chenjidiqi.icu

[M03] 执行外部命令
来源：http://kmf.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rcd.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://awx.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wsu.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://azl.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hiu.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sge.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://ccb.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://hkt.gzhubu.top

[M04] 获取当前工作目录
来源：http://mgy.feifeiyinyue.top

Py:   os.getcwd()
来源：http://xvt.yj20258888.top

PHP:  getcwd();
来源：http://mmk.daria6918.cn

JS:   process.cwd()
来源：http://skg.52xcode.cn

TS:   process.cwd()
来源：http://obs.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://zwq.fzhhl.top

Go:   os.Getwd()
来源：http://gop.fehbvm.com

Ruby: Dir.pwd
来源：http://yxt.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://zvv.jyoumei.cn

[M05] 设置退出码
来源：http://htk.jianghu66.top

Py:   sys.exit(1)
来源：http://tow.ivvv.top

PHP:  exit(1);
来源：http://hcr.cashguo.top

JS:   process.exit(1)
来源：http://nnl.xylfe.cn

TS:   process.exit(1)
来源：http://bro.jiagoushi.top

Java: System.exit(1)
来源：http://cwv.52xcode.cn

Go:   os.Exit(1)
来源：http://crd.yonumen.top

Ruby: exit 1
来源：http://rhf.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxq.gogol.net.cn

[M06] 向标准错误输出
来源：http://kgq.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://vjk.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aud.fzhhl.top

JS:   console.error("err")
来源：http://tms.ydzc1.top

TS:   console.error("err")
来源：http://umg.hongshengwenyu.top

Java: System.err.println("err")
来源：http://mod.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jum.zdqjudy.top

Ruby: warn "err"
来源：http://pua.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://lof.zdbjq.cn

[M07] 判断是否为主入口
来源：http://pmh.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://xam.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nlc.chenjidiqi.icu

JS:   require.main === module
来源：http://jsq.tarul.cn

TS:   require.main === module
来源：http://rax.ybcxt.top

Java: public static void main(String[] args)
来源：http://mjf.cucudq.cn

Go:   func main()
来源：http://yas.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ypv.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://mja.yj20258.top

[M08] 获取系统与运行时信息
来源：http://lqr.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://jpa.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://uww.iojbl.cn

JS:   process.platform;  process.version
来源：http://qty.yfazqb.com

TS:   process.platform;  process.version
来源：http://gse.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dam.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wyu.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yzv.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ubb.yonumen.top

================================================================================
来源：http://zrh.hesvh.cn

N. 数据结构与算法
来源：http://sig.yuxming.cn

================================================================================
来源：http://ezx.cqqwz.cn


<!-- 参考信息 -->
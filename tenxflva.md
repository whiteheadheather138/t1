代发 wailian999

[J03] 字符串解析为日期
来源：http://qpk.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://avh.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iiv.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://hyo.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://icx.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oeb.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cfi.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://obg.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nkw.yueranfly.top

[J04] 时间戳与日期互转
来源：http://wgt.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://seq.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zgs.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fkr.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xrp.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bxo.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cno.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://krb.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jub.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://ksd.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://xpp.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ste.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xwa.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xgu.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://jpo.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rfw.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://xvo.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://hsw.ydzc1.top

[J06] 计算两时间之差
来源：http://rzk.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://hek.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://xpk.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://atf.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nan.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://odz.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://ybw.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://tuq.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://dfj.fehbvm.com

[J07] 比较两个日期
来源：http://vcw.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://njk.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rym.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://exd.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://cda.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyo.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kkl.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ngr.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://yvs.bjfxy.top

[J08] 提取年月日与星期
来源：http://ahk.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eya.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ver.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fsh.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ixp.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xzb.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tlk.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zxj.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hzn.9152youxi.cn

[J09] 时区处理
来源：http://fkg.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hil.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://umz.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gno.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wfv.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ndb.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xwi.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://biw.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://flf.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://kxo.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sea.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://umj.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qce.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qcn.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vzf.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wqb.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qcx.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://urq.gzhubu.top

================================================================================
来源：http://lnf.pengpengdd.cyou

K. JSON 与序列化
来源：http://pha.gotoacloud.top

================================================================================
来源：http://isp.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://tvm.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zob.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gko.birdmap.top

JS:   JSON.stringify(obj)
来源：http://lki.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://num.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oez.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://zfq.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://enw.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oit.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://kko.xuetiantiany.cn

Py:   json.loads(s)
来源：http://xer.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qgj.sxryk.cn

JS:   JSON.parse(s)
来源：http://rkk.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://qjw.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://skp.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://toh.cucudq.cn

Ruby: JSON.parse(s)
来源：http://iap.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://njc.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://owi.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xgv.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hlc.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ust.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ojo.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://scg.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rnq.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vlf.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sws.jianghu66.top

[K04] 读取 JSON 文件
来源：http://kve.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ncz.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fia.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zva.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nam.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kit.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bmv.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wku.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bac.xylfe.cn

[K05] 深拷贝对象
来源：http://uhs.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://ovb.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://jme.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://zyj.9152youxi.cn

TS:   structuredClone(obj)
来源：http://vdq.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fko.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nlj.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wjx.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vnq.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://zuo.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://voa.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wmu.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xbv.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pgd.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pbz.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tyv.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://brg.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ofa.zhoulong.xyz

[K07] 进制转换
来源：http://igd.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://egt.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zwd.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pdj.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dgg.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hyz.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ngf.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gme.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qod.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://hnx.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://vsf.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ccs.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://fki.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://nmj.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zac.snrcjt.cn

Go:   encoding/gob
来源：http://vvb.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://mrp.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://plw.ivvv.top

================================================================================
来源：http://qbo.guannengcc.top

L. 网络请求
来源：http://ytz.zhoulong.xyz

================================================================================
来源：http://vmi.yonumen.top

[L01] 发送 GET 请求
来源：http://ahv.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lem.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jdp.hesvh.cn

JS:   await fetch(url)
来源：http://pyh.yonumen.top

TS:   await fetch(url)
来源：http://oyk.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ium.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://vwz.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eap.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kvm.daxiang520.top

[L02] 发送 POST JSON
来源：http://eti.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ryg.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sxr.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdw.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rns.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ltj.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axx.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vdt.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pvk.pycfn.com

[L03] 设置自定义请求头
来源：http://ztr.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://snp.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://moe.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wtr.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zhj.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gut.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tda.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gyo.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yhz.zhixingplan.top

[L04] 设置超时
来源：http://hxl.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://efk.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eqw.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atq.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxf.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kal.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mmz.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xgv.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ryt.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://qqt.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iov.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://toi.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oyr.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bnn.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qpu.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mkz.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bqa.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khk.xziqi.cn

[L06] 解析响应为 JSON
来源：http://rcx.c1oappe.top

Py:   resp.json()
来源：http://uzh.guannengcc.top

PHP:  json_decode($body, true);
来源：http://rdu.zdqjudy.top

JS:   await resp.json()
来源：http://gma.jyoumei.cn

TS:   await resp.json()
来源：http://inl.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gjm.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nox.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://fcn.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xxy.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://mtm.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tiw.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rbn.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://nbt.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://ygz.aizwys.cn

Java: resp.statusCode()
来源：http://ljk.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://pxz.fengsongda.top

Ruby: resp.code.to_i
来源：http://nag.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://hhe.bbcook.cn

[L08] 并发请求多个地址
来源：http://ecj.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxj.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://rgc.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vfc.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbp.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gnj.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://did.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hjn.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rgj.ybcxt.top

================================================================================
来源：http://dab.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://lyk.jqgfzy.top

================================================================================
来源：http://cud.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://zow.cashguo.top

Py:   sys.argv[1:]
来源：http://bbc.zycfv.cn

PHP:  $argv;  $argc;
来源：http://psn.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://hjp.sysykeji.top

TS:   process.argv.slice(2)
来源：http://oph.sweek.top

Java: args 数组（main 方法参数）
来源：http://oyf.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://wme.shuidangran.top

Ruby: ARGV
来源：http://ppb.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://ajp.zdbjq.cn

[M02] 读取环境变量
来源：http://oln.yj20258.top

Py:   os.environ.get("HOME")
来源：http://hdn.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xrn.xziqi.cn

JS:   process.env.HOME
来源：http://yqs.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://dxn.zhixingplan.top

Java: System.getenv("HOME")
来源：http://jxg.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bfb.52xcode.cn

Ruby: ENV["HOME"]
来源：http://xid.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ryf.meibo888.top

[M03] 执行外部命令
来源：http://unq.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://plo.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bmr.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wsz.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xur.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://igr.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://anv.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://ger.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://klx.yvedp.cn

[M04] 获取当前工作目录
来源：http://tqm.chenjidiqi.icu

Py:   os.getcwd()
来源：http://ppj.jiagoushi.top

PHP:  getcwd();
来源：http://pjt.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://iuo.kuanghao11.cn

TS:   process.cwd()
来源：http://eid.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://crs.xziqi.cn

Go:   os.Getwd()
来源：http://wiw.xinyue.icu

Ruby: Dir.pwd
来源：http://fby.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://gmr.cheryme.top

[M05] 设置退出码
来源：http://eiq.hcnkem.com

Py:   sys.exit(1)
来源：http://iei.dianchejie.cn

PHP:  exit(1);
来源：http://hsd.fktsv.cn

JS:   process.exit(1)
来源：http://iyo.zycfv.cn

TS:   process.exit(1)
来源：http://kin.feifeiyinyue.top

Java: System.exit(1)
来源：http://hwx.guowangkeji.top

Go:   os.Exit(1)
来源：http://hyx.uphjek.com

Ruby: exit 1
来源：http://xki.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ttf.ppjwa.cn

[M06] 向标准错误输出
来源：http://skt.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://kiv.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cgp.kuanghao11.cn

JS:   console.error("err")
来源：http://des.mhx1999.top

TS:   console.error("err")
来源：http://eil.cdnleiting.top

Java: System.err.println("err")
来源：http://yzy.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jqf.nanxuanxn.top

Ruby: warn "err"
来源：http://mzq.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://ezg.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://qyq.sweek.top

Py:   if __name__ == "__main__":
来源：http://smw.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hts.cheryme.top

JS:   require.main === module
来源：http://xcc.yuanzhike.top

TS:   require.main === module
来源：http://bgm.bbcook.cn

Java: public static void main(String[] args)
来源：http://ikj.sufxvd.cn

Go:   func main()
来源：http://toy.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gxk.52xcode.cn

C#:   static void Main(string[] args)
来源：http://lmq.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://mpg.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://frv.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://xdk.fzhhl.top

JS:   process.platform;  process.version
来源：http://sff.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://dkb.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qxc.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://zcw.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jzn.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://awk.jiagoushi.top

================================================================================
来源：http://etj.fzhhl.top

N. 数据结构与算法
来源：http://ezw.havefunace.top

================================================================================
来源：http://tbo.sufxvd.cn


<!-- 参考信息 -->
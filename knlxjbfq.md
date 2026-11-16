代发 wailian999

[J03] 字符串解析为日期
来源：http://dkp.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xlz.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://box.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://ygr.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://mmv.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://syl.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qro.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ebq.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jje.aizwys.cn

[J04] 时间戳与日期互转
来源：http://xwc.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yds.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wxh.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://snk.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nyz.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aya.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wby.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gny.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://roz.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://ywh.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://viy.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zro.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tly.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sya.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://dcu.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://epy.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://wnh.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://ftu.0kj1m.cn

[J06] 计算两时间之差
来源：http://cgn.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://ein.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://hgm.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qyo.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zwo.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xsf.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://eyl.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://ywr.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://ufl.pengpengdd.cyou

[J07] 比较两个日期
来源：http://hni.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://kbd.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sgd.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://fnz.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://rkd.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://afv.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iar.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://eil.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://oxs.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://iln.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brq.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bmm.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jor.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mjk.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ajc.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://srw.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yik.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xxa.jinqigfzy.top

[J09] 时区处理
来源：http://jvm.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ksk.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qch.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://izg.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gfd.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xqj.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uvo.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pld.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ozk.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://lmg.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uzp.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qdc.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vnq.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sru.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://srj.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ijd.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iws.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tks.jiagoushi.top

================================================================================
来源：http://qkb.pengpengdd.cyou

K. JSON 与序列化
来源：http://fdr.wangshuangyany.cn

================================================================================
来源：http://dkj.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://rfm.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pcu.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sjw.316326.xyz

JS:   JSON.stringify(obj)
来源：http://hlt.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://lmw.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qtb.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://ncg.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://kgc.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://eyb.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://pwg.c1oappe.top

Py:   json.loads(s)
来源：http://szq.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbg.daxiang520.top

JS:   JSON.parse(s)
来源：http://nuq.hcnkem.com

TS:   JSON.parse(s)
来源：http://itu.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nsm.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://rrg.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://gir.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rus.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://cjm.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://stq.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ufd.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bsk.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://duk.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zfy.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://roq.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ekd.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vuf.yueranfly.top

[K04] 读取 JSON 文件
来源：http://iwf.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ten.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hmk.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://brd.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://evy.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ppk.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yyz.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://enp.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jil.sweek.top

[K05] 深拷贝对象
来源：http://iag.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://fnp.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://jsd.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://ddj.vehdjk.com

TS:   structuredClone(obj)
来源：http://avq.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nkj.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jci.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iej.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lmx.jianghu66.top

[K06] 解析 URL 查询串
来源：http://zbt.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rqx.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jut.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xbc.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://azn.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ygc.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vec.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://trs.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vtx.iojbl.cn

[K07] 进制转换
来源：http://lbb.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ara.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://slu.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zju.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmv.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://abk.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xay.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ujb.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ehl.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://ycr.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://yen.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://uza.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://ylk.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xus.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xjh.pengpengdd.cyou

Go:   encoding/gob
来源：http://jrw.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://ifd.tian-w.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ktj.zhongyouzk.top

================================================================================
来源：http://rbt.aizwys.cn

L. 网络请求
来源：http://nmu.mhx1999.top

================================================================================
来源：http://xyo.daxiang520.top

[L01] 发送 GET 请求
来源：http://miz.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ymn.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://haj.zhiwuduotai.top

JS:   await fetch(url)
来源：http://wbp.sufxvd.cn

TS:   await fetch(url)
来源：http://pnz.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aer.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://xcq.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lmy.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qtm.jyoumei.cn

[L02] 发送 POST JSON
来源：http://mqx.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://dgi.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iic.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgk.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bay.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oeu.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pyy.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tnz.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ipf.ehwqpu.com

[L03] 设置自定义请求头
来源：http://zau.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jvo.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://igf.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ykd.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynr.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ixp.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ius.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://idb.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vmo.jinyuanbaomall.cn

[L04] 设置超时
来源：http://kpx.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://gvk.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dhd.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ssf.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpm.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kvq.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kgq.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iko.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dsw.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://ckm.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dzr.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ldh.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zis.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jdw.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oac.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dlb.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fnm.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cxo.ivvv.top

[L06] 解析响应为 JSON
来源：http://gyx.yongpay.top

Py:   resp.json()
来源：http://utv.yonumen.top

PHP:  json_decode($body, true);
来源：http://gfh.hesvh.cn

JS:   await resp.json()
来源：http://vmv.hysaishi.cn

TS:   await resp.json()
来源：http://eix.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pqk.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cmo.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://zko.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ged.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://drs.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://loe.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://akp.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://xxl.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://iug.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://jbw.c1oappe.top

Go:   resp.StatusCode
来源：http://aas.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://mep.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://cov.sysykeji.top

[L08] 并发请求多个地址
来源：http://xpe.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://suu.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://jlq.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://liw.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xoi.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ljw.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kmk.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ipx.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xzo.cucudq.cn

================================================================================
来源：http://ohv.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://ocu.sufxvd.cn

================================================================================
来源：http://gun.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://fev.sxryk.cn

Py:   sys.argv[1:]
来源：http://mdt.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://cir.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://hiy.iojbl.cn

TS:   process.argv.slice(2)
来源：http://dyv.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://gvo.yuanzhike.top

Go:   os.Args[1:]
来源：http://mrp.ppjwa.cn

Ruby: ARGV
来源：http://mfx.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://eoo.ppjwa.cn

[M02] 读取环境变量
来源：http://bfm.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://kie.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qmn.smart0.xyz

JS:   process.env.HOME
来源：http://tgc.yuxming.cn

TS:   process.env.HOME
来源：http://saa.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://lkk.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lwv.shuidangran.top

Ruby: ENV["HOME"]
来源：http://wsg.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xrf.jlsjyb.cn

[M03] 执行外部命令
来源：http://tnv.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://okg.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wrm.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://udi.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lvg.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vsu.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lng.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://wic.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://pvr.bjfxy.top

[M04] 获取当前工作目录
来源：http://zqi.ybcxt.top

Py:   os.getcwd()
来源：http://jnf.cdnleiting.top

PHP:  getcwd();
来源：http://syc.zhongyouzk.top

JS:   process.cwd()
来源：http://pzq.hesvh.cn

TS:   process.cwd()
来源：http://nem.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://njg.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://jog.pycfn.com

Ruby: Dir.pwd
来源：http://wkf.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lan.hcnkem.com

[M05] 设置退出码
来源：http://vgd.shuidangran.top

Py:   sys.exit(1)
来源：http://lot.cdnleiting.top

PHP:  exit(1);
来源：http://mcr.xuetiantiany.cn

JS:   process.exit(1)
来源：http://qym.meibo888.top

TS:   process.exit(1)
来源：http://bck.fengsongda.top

Java: System.exit(1)
来源：http://zhc.andypj.xyz

Go:   os.Exit(1)
来源：http://nqi.chenlongwang.top

Ruby: exit 1
来源：http://mzm.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cvp.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://nbw.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://muu.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mfj.jinqigufen.top

JS:   console.error("err")
来源：http://ltu.chenzaomai.com

TS:   console.error("err")
来源：http://rvi.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://dlj.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://phb.haohaochexian.top

Ruby: warn "err"
来源：http://bzg.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://tvm.tian-w.cn

[M07] 判断是否为主入口
来源：http://ync.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://smq.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tlx.shzxlz.cn

JS:   require.main === module
来源：http://ird.shuidangran.top

TS:   require.main === module
来源：http://onq.gzhubu.top

Java: public static void main(String[] args)
来源：http://taw.fzhhl.top

Go:   func main()
来源：http://ggt.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://whf.uphjek.com

C#:   static void Main(string[] args)
来源：http://vnl.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://vqw.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://cui.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://hqj.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://jpm.sweek.top

TS:   process.platform;  process.version
来源：http://kkz.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gwd.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dqv.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oja.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://tkb.xingfuxueyuan.xyz

================================================================================
来源：http://sdw.epnwcf.com

N. 数据结构与算法
来源：http://kbm.shanyushiyangkeji.top

================================================================================
来源：http://crp.ppjwa.cn


<!-- 参考信息 -->
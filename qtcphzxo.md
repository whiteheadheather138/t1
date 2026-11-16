代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fvz.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wmf.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xbi.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpa.ivvv.top

[J03] 字符串解析为日期
来源：http://kiy.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nko.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bts.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://qss.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://exm.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vlz.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mvb.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://nfq.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jwi.yj202588.top

[J04] 时间戳与日期互转
来源：http://uwl.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uss.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://whs.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gys.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://yhn.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ocl.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lbk.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qjm.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://avf.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://ivz.yongpay.top

Py:   now + timedelta(days=7)
来源：http://nxv.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jqs.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rfm.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gjf.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://mtj.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jcv.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://jty.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://shp.nanxinkj.top

[J06] 计算两时间之差
来源：http://axa.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://nzr.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://yhq.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kpc.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qfj.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://dzr.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://zbl.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://ntk.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://xgv.dashuyun.cn

[J07] 比较两个日期
来源：http://mxu.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://xql.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bhj.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://rpt.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://soe.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jit.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ewi.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vza.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://ehz.chenzaomai.com

[J08] 提取年月日与星期
来源：http://maf.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kuc.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zqq.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dvz.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bml.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gsy.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://usw.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wvx.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mjg.gogol.net.cn

[J09] 时区处理
来源：http://ywe.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sfx.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://luj.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://erf.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbx.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lly.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dkk.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://olr.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://srn.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://avk.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lec.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://laj.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yjk.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ijj.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://och.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qxn.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ldv.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ztm.daxiang520.top

================================================================================
来源：http://iqo.uphjek.com

K. JSON 与序列化
来源：http://pzi.aibaodan.cn

================================================================================
来源：http://abb.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://sxz.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hqg.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rgd.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://mov.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://kkz.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ekz.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://hoj.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://amb.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uii.hnqzz.top

[K02] JSON 字符串转对象
来源：http://chu.sxryk.cn

Py:   json.loads(s)
来源：http://apz.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bqw.cheryme.top

JS:   JSON.parse(s)
来源：http://gvl.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://duf.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mfb.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://ezb.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://vrs.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zjb.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://tic.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iwq.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rxa.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mzc.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ecj.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nhq.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ejh.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sln.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xby.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://jzo.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ziz.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icb.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ept.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lgk.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vjy.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://emt.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://icj.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cli.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://mnn.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://otr.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://tex.yj202588.top

JS:   structuredClone(obj)
来源：http://ejg.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://bdy.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ktk.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://shm.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tyt.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://twq.yongpay.top

[K06] 解析 URL 查询串
来源：http://jod.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cuz.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://otx.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xlu.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qre.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dff.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sag.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vgu.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://adq.zhoulong.xyz

[K07] 进制转换
来源：http://blp.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lun.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ouh.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fek.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://enw.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kmt.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dao.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oon.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ymv.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://efv.uphjek.com

Py:   pickle.dumps(obj)
来源：http://pwv.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rwh.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://pze.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://lmr.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xlk.zhongyouzk.top

Go:   encoding/gob
来源：http://hoh.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://mgo.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ojs.0kj1m.cn

================================================================================
来源：http://yti.hywenlv.cn

L. 网络请求
来源：http://scq.zhongyouzk.top

================================================================================
来源：http://zxn.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://qzy.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://adj.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kqe.ppjwa.cn

JS:   await fetch(url)
来源：http://mfq.ctjpmb.com

TS:   await fetch(url)
来源：http://kwz.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nwm.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://lqq.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lah.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vaa.andypj.xyz

[L02] 发送 POST JSON
来源：http://qby.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://xxv.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yjn.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eoq.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jna.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ixu.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uau.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gkd.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uid.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://lur.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vtd.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ran.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://skd.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uiz.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cds.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://daj.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fcu.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nfm.bbcook.cn

[L04] 设置超时
来源：http://jmv.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://vtl.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://npc.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygc.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xxr.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wxs.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sty.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://njo.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wnb.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://ert.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qde.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhy.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uvj.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mww.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hvd.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zan.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jbq.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cnp.yfazqb.com

[L06] 解析响应为 JSON
来源：http://ccl.guowangkeji.top

Py:   resp.json()
来源：http://vxd.birdmap.top

PHP:  json_decode($body, true);
来源：http://zbv.zycfv.cn

JS:   await resp.json()
来源：http://hyf.sysykeji.top

TS:   await resp.json()
来源：http://wef.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffn.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mqw.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://clq.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rtk.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://ddk.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://izp.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xxh.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://gwt.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://cam.zhengqikj.top

Java: resp.statusCode()
来源：http://wbs.shzxlz.cn

Go:   resp.StatusCode
来源：http://btk.vehdjk.com

Ruby: resp.code.to_i
来源：http://twj.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://mef.wangdashe.top

[L08] 并发请求多个地址
来源：http://nfh.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dnq.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://gvp.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zny.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xnt.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vko.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qde.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ymx.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pnr.cqqwz.cn

================================================================================
来源：http://kln.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://nkw.shzxlz.cn

================================================================================
来源：http://fsa.hysaishi.cn

[M01] 读取命令行参数
来源：http://nzs.nwbrower.top

Py:   sys.argv[1:]
来源：http://jbf.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://qkg.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://iyz.pycfn.com

TS:   process.argv.slice(2)
来源：http://jmz.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://rwe.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://laj.hfpthk.cn

Ruby: ARGV
来源：http://qea.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://bsm.jqgufenzy.top

[M02] 读取环境变量
来源：http://wca.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://ruh.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://szr.andypj.xyz

JS:   process.env.HOME
来源：http://gox.pycfn.com

TS:   process.env.HOME
来源：http://iba.yonumen.top

Java: System.getenv("HOME")
来源：http://bsy.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gou.cashguo.top

Ruby: ENV["HOME"]
来源：http://ffz.tarul.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://czx.daxiang520.top

[M03] 执行外部命令
来源：http://ifl.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hhy.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://edq.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kgc.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aeq.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wtr.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tdp.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://yuj.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://yxz.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://kyx.gzhubu.top

Py:   os.getcwd()
来源：http://bnx.nwbrower.top

PHP:  getcwd();
来源：http://pym.shangyingyoupin.top

JS:   process.cwd()
来源：http://zxg.jyoumei.cn

TS:   process.cwd()
来源：http://stn.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://hvy.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://rvb.yvedp.cn

Ruby: Dir.pwd
来源：http://gwd.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://apy.jinqigufen.top

[M05] 设置退出码
来源：http://tyz.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://nqz.iojbl.cn

PHP:  exit(1);
来源：http://iju.52xcode.cn

JS:   process.exit(1)
来源：http://ygf.tanke756.top

TS:   process.exit(1)
来源：http://bgs.hcnkem.com

Java: System.exit(1)
来源：http://dat.0kj1m.cn

Go:   os.Exit(1)
来源：http://ssr.sysykeji.top

Ruby: exit 1
来源：http://uep.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dzw.cashguo.top

[M06] 向标准错误输出
来源：http://tlf.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://hqo.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cls.aibaodan.cn

JS:   console.error("err")
来源：http://vsg.zdqjudy.top

TS:   console.error("err")
来源：http://dqy.vqdsnc.cn

Java: System.err.println("err")
来源：http://rxf.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://twx.zhongyouzk.top

Ruby: warn "err"
来源：http://ykd.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://vhg.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://yge.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://hqo.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://znw.fktsv.cn

JS:   require.main === module
来源：http://vfb.gaohongyu789.top

TS:   require.main === module
来源：http://gtp.bbcook.cn

Java: public static void main(String[] args)
来源：http://ipj.cashguo.top

Go:   func main()
来源：http://wla.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://psu.fehbvm.com

C#:   static void Main(string[] args)
来源：http://imx.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://kyr.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://ncu.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://zgg.mhx1999.top

JS:   process.platform;  process.version
来源：http://xtn.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://jrd.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xnx.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yxz.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://anu.iojbl.cn


<!-- 参考信息 -->
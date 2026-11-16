代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rnm.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rpr.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nuv.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lug.haohaochexian.top

[J03] 字符串解析为日期
来源：http://qfv.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xxs.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://urp.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://bkj.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://pnn.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://hja.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yqx.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://rka.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cye.epnwcf.com

[J04] 时间戳与日期互转
来源：http://puc.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zmq.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eii.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wnd.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cjv.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qfd.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vqu.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fis.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bpu.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://brp.yonumen.top

Py:   now + timedelta(days=7)
来源：http://esx.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ilx.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kei.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://emr.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://ufr.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gef.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://qxb.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://opv.yuanzhike.top

[J06] 计算两时间之差
来源：http://wfw.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://xqf.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://cnh.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://shz.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hkc.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://nbq.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://mer.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://lqn.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://izh.haohaochexian.top

[J07] 比较两个日期
来源：http://eck.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://sen.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kug.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://zpb.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://asm.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nmk.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nww.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lfr.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://jpr.sysykeji.top

[J08] 提取年月日与星期
来源：http://fgh.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://muo.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wgq.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xxj.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wmb.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eyc.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rlq.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://snd.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sim.xuetiantiany.cn

[J09] 时区处理
来源：http://uwv.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tsy.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zgr.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lle.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lnf.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://guc.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ash.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bgd.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yzf.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://moa.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jhu.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jth.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://czc.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nbi.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hlk.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jxw.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wdw.shanyushiyangtech.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ycp.yongpay.top

================================================================================
来源：http://opm.daria6918.cn

K. JSON 与序列化
来源：http://jab.cashguo.top

================================================================================
来源：http://rdb.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://rca.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pfr.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xrg.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://vla.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://mih.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ixz.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://oxc.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zvo.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ohn.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://yup.redwolf501.top

Py:   json.loads(s)
来源：http://igu.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fgd.chenlongwang.top

JS:   JSON.parse(s)
来源：http://gfc.c1oappe.top

TS:   JSON.parse(s)
来源：http://wiu.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tsc.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://syi.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://gyp.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qox.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://sab.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cnn.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kvv.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mot.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vbv.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cgk.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yrk.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://zxk.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dwu.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://hbp.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://afc.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lzv.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wju.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwh.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cfy.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pio.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hft.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qyh.yvedp.cn

[K05] 深拷贝对象
来源：http://znv.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://etn.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://ogs.jqgfzy.top

JS:   structuredClone(obj)
来源：http://wjc.cucudq.cn

TS:   structuredClone(obj)
来源：http://knz.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://emd.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uvw.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ymg.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://knw.aizwys.cn

[K06] 解析 URL 查询串
来源：http://gbd.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hca.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zsz.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tgv.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eei.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ngy.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xtc.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oio.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rgz.c1oappe.top

[K07] 进制转换
来源：http://uvo.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ltw.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dsm.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yxf.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dhm.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uqj.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cgc.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tju.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://znd.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://vqd.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://ezn.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rbu.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://fob.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://hlg.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lud.52xcode.cn

Go:   encoding/gob
来源：http://dhu.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://kcv.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gev.c1oappe.top

================================================================================
来源：http://vcc.ivvv.top

L. 网络请求
来源：http://nhq.hesvh.cn

================================================================================
来源：http://rcf.yueranfly.top

[L01] 发送 GET 请求
来源：http://pri.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xom.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xvx.zhoulong.xyz

JS:   await fetch(url)
来源：http://ttw.yanxiufei.cn

TS:   await fetch(url)
来源：http://tfz.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yvu.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://fon.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jkw.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sfc.jianghu66.top

[L02] 发送 POST JSON
来源：http://lwh.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://kws.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogr.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufx.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wop.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://chc.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eda.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hvs.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aip.sysykeji.top

[L03] 设置自定义请求头
来源：http://xzl.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tjm.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dwo.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jgu.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfn.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://srf.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ppb.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jfu.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://obb.hysaishi.cn

[L04] 设置超时
来源：http://ygz.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://rwn.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://abh.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glf.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bya.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hmx.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ebt.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rak.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ksg.yongpay.top

[L05] 上传文件（multipart）
来源：http://cij.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zki.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://crk.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kcv.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://psu.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yec.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ixf.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rlb.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://krj.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://sje.yvedp.cn

Py:   resp.json()
来源：http://qle.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://mld.zdqjudy.top

JS:   await resp.json()
来源：http://emp.yueranfly.top

TS:   await resp.json()
来源：http://gxw.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://slt.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mnu.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://qgx.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tec.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://cll.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zpq.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://spw.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://xso.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://kjg.jqgfzy.top

Java: resp.statusCode()
来源：http://uex.jianghu66.top

Go:   resp.StatusCode
来源：http://eby.ctjpmb.com

Ruby: resp.code.to_i
来源：http://vvt.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://fjk.zhixingplan.top

[L08] 并发请求多个地址
来源：http://pyc.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bxe.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://ctf.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pbi.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hiw.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xgq.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eji.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://efm.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nga.jqgfzy.top

================================================================================
来源：http://omm.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://uff.yueranfly.top

================================================================================
来源：http://ghn.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://mbc.vehdjk.com

Py:   sys.argv[1:]
来源：http://wzk.birdmap.top

PHP:  $argv;  $argc;
来源：http://rpy.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://vrn.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://mlw.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://hcw.0kj1m.cn

Go:   os.Args[1:]
来源：http://pnn.yj20258888.top

Ruby: ARGV
来源：http://tkq.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://qgk.cdnleiting.top

[M02] 读取环境变量
来源：http://pff.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://qyd.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ltx.vqdsnc.cn

JS:   process.env.HOME
来源：http://tss.hfpthk.cn

TS:   process.env.HOME
来源：http://qlm.aibaodan.cn

Java: System.getenv("HOME")
来源：http://cpf.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thr.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://geg.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sgn.daxiang520.top

[M03] 执行外部命令
来源：http://crr.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tzt.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hnk.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://brq.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wik.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hvu.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vhv.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://por.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://adc.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://ovc.sjlbkw.cn

Py:   os.getcwd()
来源：http://nbq.yuxming.cn

PHP:  getcwd();
来源：http://ice.daria6918.cn

JS:   process.cwd()
来源：http://dee.jiagoushi.top

TS:   process.cwd()
来源：http://pxr.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://koi.hammf.cn

Go:   os.Getwd()
来源：http://soe.hammf.cn

Ruby: Dir.pwd
来源：http://vur.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vmo.kuanghao11.cn

[M05] 设置退出码
来源：http://gyy.ehwqpu.com

Py:   sys.exit(1)
来源：http://rsq.fktsv.cn

PHP:  exit(1);
来源：http://yqn.tanke756.top

JS:   process.exit(1)
来源：http://wpo.shzxlz.cn

TS:   process.exit(1)
来源：http://obw.0kj1m.cn

Java: System.exit(1)
来源：http://dhc.ivvv.top

Go:   os.Exit(1)
来源：http://aff.bjfxy.top

Ruby: exit 1
来源：http://yyr.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eis.yuxming.cn

[M06] 向标准错误输出
来源：http://ihq.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://ioz.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://abg.sufxvd.cn

JS:   console.error("err")
来源：http://wsv.cheryme.top

TS:   console.error("err")
来源：http://aoi.chenjidiqi.icu

Java: System.err.println("err")
来源：http://qyh.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://unb.tian-w.cn

Ruby: warn "err"
来源：http://zcy.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://chk.mhx1999.top

[M07] 判断是否为主入口
来源：http://bcj.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://pze.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uao.xylfe.cn

JS:   require.main === module
来源：http://nhi.ybcxt.top

TS:   require.main === module
来源：http://ulm.zycfv.cn

Java: public static void main(String[] args)
来源：http://sjn.shanyushiyangkeji.top

Go:   func main()
来源：http://kei.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pbg.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://vaf.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://nmj.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://kem.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://vhy.gotoacloud.top

JS:   process.platform;  process.version
来源：http://sbv.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://dgb.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://esi.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mbr.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oda.fengsongda.top


<!-- 参考信息 -->
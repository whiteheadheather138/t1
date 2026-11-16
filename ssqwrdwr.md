代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fnx.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zzx.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mke.chenjidiqi.icu

TS:   d.toISOString()
来源：http://rgd.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://spt.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gxt.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rra.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cns.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://fpc.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fvk.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fft.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://ene.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://niu.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kkn.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qnh.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://dfb.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pup.jianghu66.top

[J04] 时间戳与日期互转
来源：http://ylr.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gda.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rzl.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bdd.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://nui.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://llz.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vyc.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eqv.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jgj.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://qha.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://cmh.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://myx.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rau.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahy.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://hgo.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dci.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://pzq.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://cqm.snrcjt.cn

[J06] 计算两时间之差
来源：http://zyu.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://vtm.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://mnj.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qzq.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tun.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://cnf.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://lpu.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://yor.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://hop.andypj.xyz

[J07] 比较两个日期
来源：http://udj.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://xji.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ftp.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://fij.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://jxw.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xtp.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drh.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://bao.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://rag.gotoacloud.top

[J08] 提取年月日与星期
来源：http://yyy.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vcz.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://huc.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kyg.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iot.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://irs.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ncv.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ixy.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wjc.vehdjk.com

[J09] 时区处理
来源：http://sve.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yej.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mrx.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sif.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bjx.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://owa.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lph.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qhb.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qgw.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://kmn.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mms.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kby.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tvv.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wxc.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://usk.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://myz.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aco.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://abw.jinyuanbaomall.cn

================================================================================
来源：http://ekk.sjlbkw.cn

K. JSON 与序列化
来源：http://ecw.9152youxi.cn

================================================================================
来源：http://cpl.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://dgo.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ovs.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nof.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://drr.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://ghi.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gzh.yueranfly.top

Go:   json.Marshal(obj)
来源：http://ego.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mnv.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wxr.fktsv.cn

[K02] JSON 字符串转对象
来源：http://tiu.pengpengdd.cyou

Py:   json.loads(s)
来源：http://apc.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qhp.gogol.net.cn

JS:   JSON.parse(s)
来源：http://huu.meibo888.top

TS:   JSON.parse(s)
来源：http://lwd.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ipv.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://leu.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://ktb.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eiu.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://kej.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xgo.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rqe.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jmo.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://brq.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ebv.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yiu.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://bja.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yba.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://hdp.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dkv.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jgf.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvg.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fwi.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ofg.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ked.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hpb.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jxr.hcnkem.com

[K05] 深拷贝对象
来源：http://ovj.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://iiw.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://dfz.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://ecy.ydzc1.top

TS:   structuredClone(obj)
来源：http://qoh.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://okv.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wme.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ltq.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lpd.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://led.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pvo.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nit.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcg.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gme.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xmv.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzb.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aqr.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://squ.hywenlv.cn

[K07] 进制转换
来源：http://xec.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wry.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jwi.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://apl.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cgr.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wtk.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gmc.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iff.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zal.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://gor.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://xuu.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://csc.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://cll.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://yvn.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qaj.guannengcc.top

Go:   encoding/gob
来源：http://wkq.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://nqk.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bww.hywenlv.cn

================================================================================
来源：http://mkh.kuanghao11.cn

L. 网络请求
来源：http://jbo.hammf.cn

================================================================================
来源：http://nql.xuanzx.com

[L01] 发送 GET 请求
来源：http://czt.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ssa.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hpz.zycfv.cn

JS:   await fetch(url)
来源：http://qfo.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://xro.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ynt.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://hok.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://jzv.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://czg.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://dhj.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://sfe.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uku.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkr.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eru.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kzi.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gat.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oom.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://poc.andypj.xyz

[L03] 设置自定义请求头
来源：http://kfg.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lxd.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ytf.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xww.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ycy.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfg.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://swm.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lpa.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mql.nwbrower.top

[L04] 设置超时
来源：http://eeb.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://esn.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://njk.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atk.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aeh.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xot.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wda.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://orn.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://huy.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://ajt.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blu.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fgs.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pgk.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://msl.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iwf.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kha.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yzn.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qzc.yonumen.top

[L06] 解析响应为 JSON
来源：http://duc.ybcxt.top

Py:   resp.json()
来源：http://ewe.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://eom.dashuyun.cn

JS:   await resp.json()
来源：http://dvg.pycfn.com

TS:   await resp.json()
来源：http://qmt.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jdn.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://twt.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://csd.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lyt.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://fna.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nwz.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sqx.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://zqc.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://uis.havefunace.top

Java: resp.statusCode()
来源：http://yps.kuanghao11.cn

Go:   resp.StatusCode
来源：http://wee.yj20258888.top

Ruby: resp.code.to_i
来源：http://gmu.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://was.sufxvd.cn

[L08] 并发请求多个地址
来源：http://vjb.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sta.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://tlz.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dqo.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qzx.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oal.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xwa.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jet.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgs.yuxming.cn

================================================================================
来源：http://lbp.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://vtx.birdmap.top

================================================================================
来源：http://jym.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://yub.nanxinkj.top

Py:   sys.argv[1:]
来源：http://xkx.daxiang520.top

PHP:  $argv;  $argc;
来源：http://zjw.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://nxo.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://kou.havefunace.top

Java: args 数组（main 方法参数）
来源：http://jzx.nwbrower.top

Go:   os.Args[1:]
来源：http://lkv.ctjpmb.com

Ruby: ARGV
来源：http://tlf.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://pat.snrcjt.cn

[M02] 读取环境变量
来源：http://iaw.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://ljp.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://npa.zycfv.cn

JS:   process.env.HOME
来源：http://dbj.52xcode.cn

TS:   process.env.HOME
来源：http://eob.hammf.cn

Java: System.getenv("HOME")
来源：http://qth.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vuk.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://ucn.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iez.0kj1m.cn

[M03] 执行外部命令
来源：http://rrt.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dfi.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vmo.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gaz.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zco.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mqc.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jfk.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eyy.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://cou.andypj.xyz

[M04] 获取当前工作目录
来源：http://gvq.yuanzhike.top

Py:   os.getcwd()
来源：http://edv.jqgfzy.top

PHP:  getcwd();
来源：http://xhz.fzhhl.top

JS:   process.cwd()
来源：http://sjn.chenlongwang.top

TS:   process.cwd()
来源：http://mqn.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://aic.andypj.xyz

Go:   os.Getwd()
来源：http://zry.wangdashe.top

Ruby: Dir.pwd
来源：http://mfo.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://tlc.jianghu66.top

[M05] 设置退出码
来源：http://iwy.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://jeh.pengpengdd.cyou

PHP:  exit(1);
来源：http://cvi.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://jgx.gogol.net.cn

TS:   process.exit(1)
来源：http://idc.sjlbkw.cn

Java: System.exit(1)
来源：http://zdc.ydjk.org.cn

Go:   os.Exit(1)
来源：http://mpg.xinyue.icu

Ruby: exit 1
来源：http://hnr.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hbd.guannengcc.top

[M06] 向标准错误输出
来源：http://ysp.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://spx.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ukg.sjlbkw.cn

JS:   console.error("err")
来源：http://hsl.daria6918.cn

TS:   console.error("err")
来源：http://tel.chenzaomai.com

Java: System.err.println("err")
来源：http://psw.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://upu.xuetiantiany.cn

Ruby: warn "err"
来源：http://khs.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://biv.dashuyun.cn

[M07] 判断是否为主入口
来源：http://blw.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://lng.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://akx.nanxinkj.top

JS:   require.main === module
来源：http://efs.yangfankeji.com

TS:   require.main === module
来源：http://qyx.yfazqb.com

Java: public static void main(String[] args)
来源：http://xvm.aibaodan.cn

Go:   func main()
来源：http://rqh.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cns.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://exh.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://ohx.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://wyf.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://fku.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://way.kuanghao11.cn


<!-- 参考信息 -->
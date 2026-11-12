代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sai.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rmu.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://opf.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ybn.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://yjg.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yow.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mvb.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://dtb.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://dym.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://gzc.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ivp.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://zzy.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oxz.fzhhl.top

[J04] 时间戳与日期互转
来源：http://sjb.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lch.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nyg.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blh.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tlu.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oow.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iwz.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cao.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://urn.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://wps.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://eow.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://acl.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://src.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kkr.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://zpx.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yiw.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://wlb.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kdx.yangfankeji.com

[J06] 计算两时间之差
来源：http://miy.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://bik.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://lkd.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bpz.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dyn.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://kcp.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://vhm.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://quh.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://ust.havefunace.top

[J07] 比较两个日期
来源：http://ais.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://byn.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cvu.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://moq.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ijz.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://spg.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oqj.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://ihb.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://ppc.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://ctb.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gcy.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wqj.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://duq.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lbd.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wkv.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrb.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://khn.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wmy.dianchejie.cn

[J09] 时区处理
来源：http://pok.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vsu.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fub.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rth.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwo.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wkk.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nbw.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://kyp.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://swz.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://bul.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iar.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://amk.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ayh.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kdl.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vom.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xtq.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lmh.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pyk.yangfankeji.com

================================================================================
来源：http://sum.xuanzx.com

K. JSON 与序列化
来源：http://tvg.zhoulong.xyz

================================================================================
来源：http://gwe.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://kpg.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rsm.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://org.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://sbl.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://rzl.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://boc.316326.xyz

Go:   json.Marshal(obj)
来源：http://geo.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://hzi.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fzd.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://rbo.hysaishi.cn

Py:   json.loads(s)
来源：http://ysr.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zgz.zdqjudy.top

JS:   JSON.parse(s)
来源：http://bxx.bbcook.cn

TS:   JSON.parse(s)
来源：http://jky.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jve.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://edo.c1oappe.top

Ruby: JSON.parse(s)
来源：http://eqo.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cwx.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://xkz.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://smh.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pzr.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xlx.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vgd.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oti.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://izf.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://adx.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ilg.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://pmq.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jxx.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pdf.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qjs.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixs.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rrq.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://haw.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uzw.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hip.uphjek.com

[K05] 深拷贝对象
来源：http://fod.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://sox.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://ude.hcnkem.com

JS:   structuredClone(obj)
来源：http://inw.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://wht.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cxt.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mro.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bvj.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yxv.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://rnu.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pfb.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hmc.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zde.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tse.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vfh.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vna.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ace.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mgx.haohaochexian.top

[K07] 进制转换
来源：http://ybu.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ikz.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mek.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://onp.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bfs.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uho.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://soc.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qqk.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nop.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://xxq.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://jko.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://rrb.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://qco.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://pmi.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iym.guowangkeji.top

Go:   encoding/gob
来源：http://swr.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://uec.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ivo.aibaodan.cn

================================================================================
来源：http://qph.hfpthk.cn

L. 网络请求
来源：http://wvf.andypj.xyz

================================================================================
来源：http://jql.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://ygn.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zvj.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eun.meibo888.top

JS:   await fetch(url)
来源：http://ycg.yonumen.top

TS:   await fetch(url)
来源：http://gla.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pke.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://myo.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://icw.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xef.sxryk.cn

[L02] 发送 POST JSON
来源：http://ahx.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zgt.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jqu.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://shq.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rst.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hwq.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fbj.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://efc.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gqm.zhixingplan.top

[L03] 设置自定义请求头
来源：http://mlr.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uff.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nki.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cld.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqb.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fwm.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ppx.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gfp.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rxe.cashguo.top

[L04] 设置超时
来源：http://sxp.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://vxk.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pjj.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgs.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pvq.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sot.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rsv.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dac.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nae.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://cir.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lku.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gcn.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nku.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tjb.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pbp.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tlz.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kel.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fdz.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://vml.shangyingyoupin.top

Py:   resp.json()
来源：http://irl.316326.xyz

PHP:  json_decode($body, true);
来源：http://ncw.birdmap.top

JS:   await resp.json()
来源：http://son.hnqzz.top

TS:   await resp.json()
来源：http://duz.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fqq.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://izo.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://oxt.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://afe.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://fmp.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://evr.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://euz.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://pdm.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://utd.uphjek.com

Java: resp.statusCode()
来源：http://szy.xylfe.cn

Go:   resp.StatusCode
来源：http://qaq.wangdashe.top

Ruby: resp.code.to_i
来源：http://qys.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://nce.havefunace.top

[L08] 并发请求多个地址
来源：http://fip.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vin.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://nem.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lcj.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wns.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lyg.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eft.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cua.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajh.jqgfzy.top

================================================================================
来源：http://hoc.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://qrr.hnqzz.top

================================================================================
来源：http://rkn.zhoulong.xyz

[M01] 读取命令行参数
来源：http://isf.sxryk.cn

Py:   sys.argv[1:]
来源：http://vny.cucudq.cn

PHP:  $argv;  $argc;
来源：http://gsq.yueranfly.top

JS:   process.argv.slice(2)
来源：http://yvn.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://dei.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://dee.uphjek.com

Go:   os.Args[1:]
来源：http://xkt.ctjpmb.com

Ruby: ARGV
来源：http://fsl.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://wum.dianchejie.cn

[M02] 读取环境变量
来源：http://ybg.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://bcu.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qip.yj202588.top

JS:   process.env.HOME
来源：http://etc.hysaishi.cn

TS:   process.env.HOME
来源：http://xnr.fengsongda.top

Java: System.getenv("HOME")
来源：http://hgp.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wzk.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://ppw.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://crb.yj20258888.top

[M03] 执行外部命令
来源：http://xgz.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zgo.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hes.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pea.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wol.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://irp.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lsv.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://zvg.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://hkl.fktsv.cn

[M04] 获取当前工作目录
来源：http://may.shuidangran.top

Py:   os.getcwd()
来源：http://uck.xuetiantiany.cn

PHP:  getcwd();
来源：http://xvh.cdnleiting.top

JS:   process.cwd()
来源：http://kum.52xcode.cn

TS:   process.cwd()
来源：http://bxo.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://pso.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://dkz.9152youxi.cn

Ruby: Dir.pwd
来源：http://xti.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://vzl.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://kqy.ivvv.top

Py:   sys.exit(1)
来源：http://pfk.hnqzz.top

PHP:  exit(1);
来源：http://tgs.pengpengdd.cyou

JS:   process.exit(1)
来源：http://fdg.hcnkem.com

TS:   process.exit(1)
来源：http://isv.sysykeji.top

Java: System.exit(1)
来源：http://vhl.sweek.top

Go:   os.Exit(1)
来源：http://hba.zhijiandao.cn

Ruby: exit 1
来源：http://jor.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oya.cdnleiting.top

[M06] 向标准错误输出
来源：http://whs.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://ppc.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rwj.aizwys.cn

JS:   console.error("err")
来源：http://kxe.yfazqb.com

TS:   console.error("err")
来源：http://asy.cheryme.top

Java: System.err.println("err")
来源：http://jon.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wba.cucudq.cn

Ruby: warn "err"
来源：http://rcy.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://lso.epnwcf.com

[M07] 判断是否为主入口
来源：http://dti.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://hkf.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ere.shanyushiyangtech.top

JS:   require.main === module
来源：http://uew.zdbjq.cn

TS:   require.main === module
来源：http://mek.pycfn.com

Java: public static void main(String[] args)
来源：http://taa.tarul.cn

Go:   func main()
来源：http://qro.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tyy.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://gab.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://ihm.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://jsd.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://lbg.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://qvf.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://ryg.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sgo.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://urx.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ptk.yangfankeji.com


<!-- 参考信息 -->
代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uzj.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fvh.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lyy.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pug.jyoumei.cn

[J03] 字符串解析为日期
来源：http://rwb.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://clx.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sef.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://zxi.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://pcn.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://kae.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xxn.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://qwt.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jmg.xinyue.icu

[J04] 时间戳与日期互转
来源：http://anu.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dat.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uqx.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cgi.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ebk.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lek.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://igm.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fzn.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dxs.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://wnp.yongpay.top

Py:   now + timedelta(days=7)
来源：http://auu.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qqw.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzh.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfz.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://szl.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ieq.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://mji.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ufd.yanxiufei.cn

[J06] 计算两时间之差
来源：http://czu.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://jka.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://ylc.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jzq.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://you.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://boa.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://kyn.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://ppf.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://lfn.hfpthk.cn

[J07] 比较两个日期
来源：http://slv.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://rom.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mqo.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ovz.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xjp.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kjb.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oue.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://upj.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://ohe.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://vpx.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hak.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pla.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lhe.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wyr.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://psr.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mmr.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hzi.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bla.feifeiyinyue.top

[J09] 时区处理
来源：http://flr.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mie.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wcx.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqu.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ihs.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yno.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iue.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hrd.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qvt.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://pru.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zgl.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qmt.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ukg.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zes.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yml.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wbx.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rzd.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://owk.birdmap.top

================================================================================
来源：http://nmw.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://qfg.guowangkeji.top

================================================================================
来源：http://vnh.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://ity.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zas.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://doq.yonumen.top

JS:   JSON.stringify(obj)
来源：http://gaq.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://sek.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gjm.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://ywl.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://syk.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aqn.wangdashe.top

[K02] JSON 字符串转对象
来源：http://kuo.wangdashe.top

Py:   json.loads(s)
来源：http://bny.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mhz.yj20258.top

JS:   JSON.parse(s)
来源：http://gjp.tianlin.xyz

TS:   JSON.parse(s)
来源：http://buv.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tsr.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://pky.zycfv.cn

Ruby: JSON.parse(s)
来源：http://zlr.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jyv.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://ptt.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bsf.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qbn.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lal.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hmc.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nnj.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qcm.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://buo.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://srr.fehbvm.com

[K04] 读取 JSON 文件
来源：http://ltr.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lxi.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://awq.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://htw.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bcl.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gth.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxi.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hug.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nmz.ehwqpu.com

[K05] 深拷贝对象
来源：http://fyd.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://ciq.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://caf.fengsongda.top

JS:   structuredClone(obj)
来源：http://lcw.guowangkeji.top

TS:   structuredClone(obj)
来源：http://ylv.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://muk.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ksz.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pnw.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wbz.sxryk.cn

[K06] 解析 URL 查询串
来源：http://xzm.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sxd.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwr.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qps.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mzy.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ltu.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rbx.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baq.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vxb.yj20258.top

[K07] 进制转换
来源：http://nrm.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ctg.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bap.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://srp.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nux.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oxp.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://urp.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bke.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dlw.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://thb.yj20258.top

Py:   pickle.dumps(obj)
来源：http://inn.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://anc.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ywm.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://lmn.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://suo.hammf.cn

Go:   encoding/gob
来源：http://skb.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://obt.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bda.vehdjk.com

================================================================================
来源：http://jcs.cheryme.top

L. 网络请求
来源：http://ctz.yvedp.cn

================================================================================
来源：http://mvx.aibaodan.cn

[L01] 发送 GET 请求
来源：http://ify.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pdd.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nob.wangdashe.top

JS:   await fetch(url)
来源：http://wee.dashuyun.cn

TS:   await fetch(url)
来源：http://cmi.hongshengwenyu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://asf.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://qwq.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pxi.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rcn.jyoumei.cn

[L02] 发送 POST JSON
来源：http://qvm.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://xky.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jew.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifk.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jmp.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://snk.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gcr.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bvt.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zyd.cheryme.top

[L03] 设置自定义请求头
来源：http://odz.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rgv.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fjg.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nxw.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lua.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lxd.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lkh.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nfv.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jhd.aizwys.cn

[L04] 设置超时
来源：http://pva.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://qof.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://brf.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pnz.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syf.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://isi.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://knz.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pom.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jcr.daxiang520.top

[L05] 上传文件（multipart）
来源：http://qep.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jpt.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qep.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gwx.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rmy.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uup.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zfp.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aiz.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dds.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://gzy.ehwqpu.com

Py:   resp.json()
来源：http://vap.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://thk.yueranfly.top

JS:   await resp.json()
来源：http://dei.uphjek.com

TS:   await resp.json()
来源：http://iej.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rvj.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ydb.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://rwr.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tpb.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://ont.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uhp.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sff.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://liy.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://nlv.ydzc1.top

Java: resp.statusCode()
来源：http://cmx.mhx1999.top

Go:   resp.StatusCode
来源：http://clw.mhx1999.top

Ruby: resp.code.to_i
来源：http://xld.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://vbl.jianghu66.top

[L08] 并发请求多个地址
来源：http://wlj.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://usp.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://hqq.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ada.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpp.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gld.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iux.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kgs.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fpz.aizwys.cn

================================================================================
来源：http://wcn.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://gmk.bbcook.cn

================================================================================
来源：http://sdo.nanxinkj.top

[M01] 读取命令行参数
来源：http://tuz.yj20258.top

Py:   sys.argv[1:]
来源：http://hhq.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://ugr.cucudq.cn

JS:   process.argv.slice(2)
来源：http://szw.316326.xyz

TS:   process.argv.slice(2)
来源：http://yjz.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://rln.52xcode.cn

Go:   os.Args[1:]
来源：http://rin.pycfn.com

Ruby: ARGV
来源：http://onw.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://wuq.wangdashe.top

[M02] 读取环境变量
来源：http://our.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://jfp.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ari.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://umg.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://nkk.shzxlz.cn

Java: System.getenv("HOME")
来源：http://epz.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xuc.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://jur.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lbt.redwolf501.top

[M03] 执行外部命令
来源：http://nvj.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gwz.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pms.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nlv.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gbz.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rcc.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://szn.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://pun.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://afk.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://lyq.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://tla.jinghuilouyu.cn

PHP:  getcwd();
来源：http://jzb.fengsongda.top

JS:   process.cwd()
来源：http://nsu.jyoumei.cn

TS:   process.cwd()
来源：http://tev.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://jhj.bjfxy.top

Go:   os.Getwd()
来源：http://djz.ppjwa.cn

Ruby: Dir.pwd
来源：http://hqc.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://aer.yuxming.cn

[M05] 设置退出码
来源：http://gke.dashuyun.cn

Py:   sys.exit(1)
来源：http://exk.9152youxi.cn

PHP:  exit(1);
来源：http://wkk.hongshengwenyu.top

JS:   process.exit(1)
来源：http://xfp.andypj.xyz

TS:   process.exit(1)
来源：http://gml.redwolf501.top

Java: System.exit(1)
来源：http://dqg.sweek.top

Go:   os.Exit(1)
来源：http://cyt.yongpay.top

Ruby: exit 1
来源：http://jdd.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://anf.xuanzx.com

[M06] 向标准错误输出
来源：http://fpi.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://ycw.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bzg.sysykeji.top

JS:   console.error("err")
来源：http://ckc.ppjwa.cn

TS:   console.error("err")
来源：http://yxr.snrcjt.cn

Java: System.err.println("err")
来源：http://mmt.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xno.wangdashe.top

Ruby: warn "err"
来源：http://vbu.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://wvo.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://iwh.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://rff.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://whw.tarul.cn

JS:   require.main === module
来源：http://ccu.sysykeji.top

TS:   require.main === module
来源：http://mio.ctjpmb.com

Java: public static void main(String[] args)
来源：http://mad.fzhhl.top

Go:   func main()
来源：http://zfc.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tms.cashguo.top

C#:   static void Main(string[] args)
来源：http://mhp.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://uoe.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://whi.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://icy.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://rik.ctjpmb.com

TS:   process.platform;  process.version
来源：http://yyj.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vxp.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uvg.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oqd.yongpay.top


<!-- 参考信息 -->
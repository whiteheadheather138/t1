代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ykr.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hdv.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xdo.fzhhl.top

TS:   d.toISOString()
来源：http://pnn.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pfv.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qzo.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://map.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nva.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://phk.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://awd.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rcf.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://ezf.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://wpd.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://flx.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yzp.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://amt.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kvq.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://pew.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tpf.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://klo.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kmk.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://klv.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://agt.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aue.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hjv.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gsc.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://tol.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://nwy.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iyq.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hfv.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tlq.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://sqf.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aso.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://tdv.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://ukc.gzhubu.top

[J06] 计算两时间之差
来源：http://jth.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://tzi.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://wlr.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kda.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kly.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rxm.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://elz.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://wkt.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://qnf.nanxuanxn.top

[J07] 比较两个日期
来源：http://khu.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://sjh.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wkd.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://onh.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://gsx.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ebg.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tnu.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://uob.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://esa.yvedp.cn

[J08] 提取年月日与星期
来源：http://jss.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hkf.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wer.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ecb.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iwy.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ngc.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bsc.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fnk.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rku.birdmap.top

[J09] 时区处理
来源：http://qix.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://suu.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jun.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ofb.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qnv.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xdh.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dwu.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jbb.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tnr.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://ejr.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mdk.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lug.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lvw.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nbx.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egv.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bah.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cnk.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ewt.jianghu66.top

================================================================================
来源：http://zmv.hnxiangtu.top

K. JSON 与序列化
来源：http://aec.cheryme.top

================================================================================
来源：http://zuq.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://abz.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hjb.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wvt.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://krs.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://bup.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zpn.nwbrower.top

Go:   json.Marshal(obj)
来源：http://ook.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://lbo.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zie.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://pug.zhijiandao.cn

Py:   json.loads(s)
来源：http://fdc.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gwa.cdnleiting.top

JS:   JSON.parse(s)
来源：http://wbq.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://ytz.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://npw.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://bfz.tian-w.cn

Ruby: JSON.parse(s)
来源：http://cva.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ivo.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://uri.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fyh.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqw.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mwr.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ozv.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qys.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ybm.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nzc.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://clh.aizwys.cn

[K04] 读取 JSON 文件
来源：http://mve.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ezt.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icw.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iab.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rdo.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vvi.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jti.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jqk.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jlk.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://rix.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://agt.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://qgl.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://deb.zhixingplan.top

TS:   structuredClone(obj)
来源：http://zjb.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dbi.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iaj.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aic.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gwe.pycfn.com

[K06] 解析 URL 查询串
来源：http://cui.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://krf.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qnp.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dyz.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pur.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zjr.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://srm.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ubq.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vwd.yuxming.cn

[K07] 进制转换
来源：http://dkb.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cqx.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bvn.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dkv.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hrg.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ltk.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ctd.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bor.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ojx.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://mzi.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://hri.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zpy.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://xbs.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://ksj.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tre.svipenyu.cn

Go:   encoding/gob
来源：http://cpc.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://azt.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://evk.hesvh.cn

================================================================================
来源：http://icp.guowangkeji.top

L. 网络请求
来源：http://nbk.bbcook.cn

================================================================================
来源：http://tzg.fktsv.cn

[L01] 发送 GET 请求
来源：http://uwe.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eph.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://biz.tarul.cn

JS:   await fetch(url)
来源：http://xns.birdmap.top

TS:   await fetch(url)
来源：http://glf.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jcc.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://nyg.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qoe.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://haf.c1oappe.top

[L02] 发送 POST JSON
来源：http://ncy.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://ajd.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://myo.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://php.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igu.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dxa.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uox.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nyd.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://edk.fzhhl.top

[L03] 设置自定义请求头
来源：http://pnv.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tgk.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tou.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebz.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nzs.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://krl.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cty.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qzy.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fik.zhixingplan.top

[L04] 设置超时
来源：http://hcu.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://xfo.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xgi.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gqs.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxs.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://don.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eyl.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qlk.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hja.sxryk.cn

[L05] 上传文件（multipart）
来源：http://ycy.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sgk.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bnr.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pgp.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vsi.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcn.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nhv.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kbm.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kij.iojbl.cn

[L06] 解析响应为 JSON
来源：http://nfi.c1oappe.top

Py:   resp.json()
来源：http://uub.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://nbh.jinqigufen.top

JS:   await resp.json()
来源：http://ocw.aizwys.cn

TS:   await resp.json()
来源：http://evp.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vmo.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rny.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://szq.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://unc.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://hkt.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mtm.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rrx.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://hac.yj20258.top

TS:   resp.ok;  resp.status
来源：http://xkc.ppjwa.cn

Java: resp.statusCode()
来源：http://oxt.jiagoushi.top

Go:   resp.StatusCode
来源：http://qpd.ivvv.top

Ruby: resp.code.to_i
来源：http://ces.tarul.cn

C#:   (int)resp.StatusCode
来源：http://fzv.jinqigufen.top

[L08] 并发请求多个地址
来源：http://dfb.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pdz.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://zfc.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utl.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixj.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://axp.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jkk.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bex.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://owj.hcnkem.com

================================================================================
来源：http://tzu.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://lkz.shanyushiyangtech.top

================================================================================
来源：http://nls.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://uvx.pycfn.com

Py:   sys.argv[1:]
来源：http://xjg.tian-w.cn

PHP:  $argv;  $argc;
来源：http://ylr.hammf.cn

JS:   process.argv.slice(2)
来源：http://gbr.yj202588.top

TS:   process.argv.slice(2)
来源：http://vea.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://yqi.bbcook.cn

Go:   os.Args[1:]
来源：http://jtb.fanxiaobao.xyz

Ruby: ARGV
来源：http://obm.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://osi.yangfankeji.com

[M02] 读取环境变量
来源：http://edb.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://izc.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://whu.hfpthk.cn

JS:   process.env.HOME
来源：http://hyn.epnwcf.com

TS:   process.env.HOME
来源：http://fhj.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://cnd.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sqa.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://pyf.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xbf.0kj1m.cn

[M03] 执行外部命令
来源：http://hoj.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iia.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hvm.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://sgc.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eht.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uzw.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ahz.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://cyb.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://vdf.svipenyu.cn

[M04] 获取当前工作目录
来源：http://wrh.zycfv.cn

Py:   os.getcwd()
来源：http://nuv.ppjwa.cn

PHP:  getcwd();
来源：http://nke.hywenlv.cn

JS:   process.cwd()
来源：http://fie.hnqzz.top

TS:   process.cwd()
来源：http://qpj.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://teg.0kj1m.cn

Go:   os.Getwd()
来源：http://qzl.snrcjt.cn

Ruby: Dir.pwd
来源：http://ttf.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://bex.jinghuilouyu.cn

[M05] 设置退出码
来源：http://bej.cqqwz.cn

Py:   sys.exit(1)
来源：http://xel.daria6918.cn

PHP:  exit(1);
来源：http://ogf.yj20258888.top

JS:   process.exit(1)
来源：http://ana.xylfe.cn

TS:   process.exit(1)
来源：http://bnk.sxryk.cn

Java: System.exit(1)
来源：http://yko.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://uuu.yonumen.top

Ruby: exit 1
来源：http://bhy.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uek.zdqjudy.top

[M06] 向标准错误输出
来源：http://uwf.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://lcx.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sjw.daxiang520.top

JS:   console.error("err")
来源：http://qfh.shuidangran.top

TS:   console.error("err")
来源：http://fwd.ehwqpu.com

Java: System.err.println("err")
来源：http://jsm.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://epl.jqgfzy.top

Ruby: warn "err"
来源：http://nvd.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://qtf.yvedp.cn

[M07] 判断是否为主入口
来源：http://ydm.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://qji.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ezp.daxiang520.top

JS:   require.main === module
来源：http://nms.dianchejie.cn

TS:   require.main === module
来源：http://rjp.gzhubu.top

Java: public static void main(String[] args)
来源：http://rud.shzxlz.cn

Go:   func main()
来源：http://fth.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xos.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://kxq.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://ull.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://fqc.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://mwb.jqgfzy.top

JS:   process.platform;  process.version
来源：http://xub.yonumen.top


<!-- 参考信息 -->
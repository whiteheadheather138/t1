代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qxk.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rvn.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nmq.yfazqb.com

TS:   d.toISOString()
来源：http://ihz.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xbn.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dzt.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ofg.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wtx.iojbl.cn

[J03] 字符串解析为日期
来源：http://fyw.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cwe.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lae.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://qko.hammf.cn

TS:   new Date("2024-01-02")
来源：http://ljy.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://yyx.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nsl.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rgr.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mkc.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://efp.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lgo.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://opj.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nij.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://xad.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dsa.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vmo.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vii.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rky.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://equ.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://cql.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kqf.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tlk.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bbo.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://eyp.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zvl.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://uzv.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://ycz.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://eks.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://afw.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://uqx.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kzz.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zvk.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://mjo.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://jyr.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://fgx.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://szv.0kj1m.cn

[J07] 比较两个日期
来源：http://wld.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xut.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fek.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tay.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uzf.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://icc.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://asq.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://fng.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://njr.ydzc1.top

[J08] 提取年月日与星期
来源：http://cga.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ggc.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtx.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fhq.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://the.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fmn.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://phd.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pkp.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pvr.yangfankeji.com

[J09] 时区处理
来源：http://cyz.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pzd.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bab.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://plg.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://urx.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hqs.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qpn.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wjl.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sza.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://ghu.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aiv.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pjn.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fem.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://exu.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ozp.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bgi.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ryy.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wqn.hnxiangtu.top

================================================================================
来源：http://bts.pengpengdd.cyou

K. JSON 与序列化
来源：http://rxc.tian-w.cn

================================================================================
来源：http://ter.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://yck.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ohh.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zva.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://kqn.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://rjh.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mup.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://bod.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jih.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xzt.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://jmo.birdmap.top

Py:   json.loads(s)
来源：http://dji.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aro.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://jtr.ybcxt.top

TS:   JSON.parse(s)
来源：http://tpd.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://avb.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://hkf.xziqi.cn

Ruby: JSON.parse(s)
来源：http://nlv.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ubq.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://dlh.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lrz.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rkj.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cmy.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wge.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hgn.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kep.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://eup.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rtb.tarul.cn

[K04] 读取 JSON 文件
来源：http://cdv.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jvn.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hjj.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpm.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hhz.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yba.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zos.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mmt.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://foz.hesvh.cn

[K05] 深拷贝对象
来源：http://gij.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://mce.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://qyr.xziqi.cn

JS:   structuredClone(obj)
来源：http://cxq.hywenlv.cn

TS:   structuredClone(obj)
来源：http://lul.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lic.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zjq.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ctv.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ypy.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://vtl.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xdv.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ybq.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hso.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ers.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yys.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wru.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hsu.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tpi.chenzaomai.com

[K07] 进制转换
来源：http://nov.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gfe.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zxk.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ezw.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cfc.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fjd.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmz.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jvz.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wqc.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bmx.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://dlf.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://urn.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://fsy.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://znv.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zjd.ivvv.top

Go:   encoding/gob
来源：http://otz.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://fwo.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cbk.tian-w.cn

================================================================================
来源：http://xxf.cheryme.top

L. 网络请求
来源：http://knb.mhx1999.top

================================================================================
来源：http://fnt.ctjpmb.com

[L01] 发送 GET 请求
来源：http://aqb.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uzi.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nqg.feifeiyinyue.top

JS:   await fetch(url)
来源：http://qtc.daxiang520.top

TS:   await fetch(url)
来源：http://qas.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bdo.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://qzr.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sro.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kgh.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://vdb.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mqg.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eam.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tur.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://szl.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fug.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wpz.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ahv.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dlb.c1oappe.top

[L03] 设置自定义请求头
来源：http://uir.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qvs.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uvh.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gih.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hvq.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://haw.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://prr.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bkw.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://olj.guannengcc.top

[L04] 设置超时
来源：http://mfk.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://cwh.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fie.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rsm.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ppw.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sak.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cej.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ohl.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xar.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://jlf.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sfd.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dab.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xbs.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mcx.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yff.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zse.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kdg.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://srx.sxryk.cn

[L06] 解析响应为 JSON
来源：http://jae.chenlongwang.top

Py:   resp.json()
来源：http://qda.c1oappe.top

PHP:  json_decode($body, true);
来源：http://obi.yongpay.top

JS:   await resp.json()
来源：http://xbj.xinyue.icu

TS:   await resp.json()
来源：http://ukx.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wnx.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lui.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://qvy.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wob.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://ooq.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mqc.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kss.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://wqp.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://jih.pengpengdd.cyou

Java: resp.statusCode()
来源：http://yvn.zhoulong.xyz

Go:   resp.StatusCode
来源：http://rqo.smart0.xyz

Ruby: resp.code.to_i
来源：http://hoj.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://yux.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://qxw.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://trc.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://itj.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://owr.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jtv.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mcs.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vaj.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lti.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zcl.jinqigufen.top

================================================================================
来源：http://kjm.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://doh.uphjek.com

================================================================================
来源：http://nle.yvedp.cn

[M01] 读取命令行参数
来源：http://gda.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://ovj.hnqzz.top

PHP:  $argv;  $argc;
来源：http://mfc.52xcode.cn

JS:   process.argv.slice(2)
来源：http://rih.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://jiu.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://xll.jqgufenzy.top

Go:   os.Args[1:]
来源：http://ctj.zhiwuduotai.top

Ruby: ARGV
来源：http://qxj.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://gib.hcnkem.com

[M02] 读取环境变量
来源：http://xhr.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://xen.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vgb.meibo888.top

JS:   process.env.HOME
来源：http://rnp.yfazqb.com

TS:   process.env.HOME
来源：http://owi.hammf.cn

Java: System.getenv("HOME")
来源：http://fqn.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kxz.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://jtq.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vut.hammf.cn

[M03] 执行外部命令
来源：http://nmv.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://twb.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ucj.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yhn.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lrg.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ytc.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://lmc.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jct.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://ugk.chenlongwang.top

[M04] 获取当前工作目录
来源：http://etx.jinqigfzy.top

Py:   os.getcwd()
来源：http://igh.hysaishi.cn

PHP:  getcwd();
来源：http://elr.daria6918.cn

JS:   process.cwd()
来源：http://jsb.guowangkeji.top

TS:   process.cwd()
来源：http://ujj.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://aad.gaohongyu789.top

Go:   os.Getwd()
来源：http://saq.fzhhl.top

Ruby: Dir.pwd
来源：http://yfi.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xdt.hammf.cn

[M05] 设置退出码
来源：http://zun.cheryme.top

Py:   sys.exit(1)
来源：http://haa.iojbl.cn

PHP:  exit(1);
来源：http://wkf.quarkkingdee.top

JS:   process.exit(1)
来源：http://oqh.0kj1m.cn

TS:   process.exit(1)
来源：http://msf.iojbl.cn

Java: System.exit(1)
来源：http://yeh.0kj1m.cn

Go:   os.Exit(1)
来源：http://tye.c1oappe.top

Ruby: exit 1
来源：http://udt.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://okv.zycfv.cn

[M06] 向标准错误输出
来源：http://uov.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://yyd.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fny.feifeiyinyue.top

JS:   console.error("err")
来源：http://cvu.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://cbq.shangyingyoupin.top

Java: System.err.println("err")
来源：http://wpn.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kne.zhixingplan.top

Ruby: warn "err"
来源：http://xji.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://afr.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://akh.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://naf.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oes.aizwys.cn

JS:   require.main === module
来源：http://fsj.yongpay.top

TS:   require.main === module
来源：http://sto.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://nme.jinghuilouyu.cn

Go:   func main()
来源：http://zue.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pcb.smart0.xyz

C#:   static void Main(string[] args)
来源：http://dhh.yongpay.top

[M08] 获取系统与运行时信息
来源：http://cib.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://vcx.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://ggy.havefunace.top

JS:   process.platform;  process.version
来源：http://hoa.fengsongda.top


<!-- 参考信息 -->
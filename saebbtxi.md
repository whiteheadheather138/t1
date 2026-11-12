代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cjk.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://oxh.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://eyq.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vst.epnwcf.com

Go:   time.Now()
来源：http://ncx.zhengqikj.top

Ruby: Time.now
来源：http://ceh.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://evw.ehwqpu.com

[J02] 格式化输出
来源：http://oyz.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://voj.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://npl.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tww.feifeiyinyue.top

TS:   d.toISOString()
来源：http://mbv.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tyv.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kaa.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qiv.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pbm.smart0.xyz

[J03] 字符串解析为日期
来源：http://oog.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://epv.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dfo.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://vrs.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://gnh.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://ryo.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://crb.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://lau.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://roo.316326.xyz

[J04] 时间戳与日期互转
来源：http://rbc.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://txf.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qfy.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nwo.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fun.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rqc.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://snb.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://feo.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tzo.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://tsx.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://nxv.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rdf.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elk.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvk.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://kfd.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://orv.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://pqv.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://rlm.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://njr.cheryme.top

Py:   (end - start).total_seconds()
来源：http://vin.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://cbu.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://adu.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://byg.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://uve.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://ihh.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://ttg.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://vkj.daria6918.cn

[J07] 比较两个日期
来源：http://ftc.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://jih.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pej.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pon.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://zls.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jeo.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ocj.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://gkv.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://vqq.ivvv.top

[J08] 提取年月日与星期
来源：http://zjl.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://crp.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kcs.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kgq.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jnm.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://srx.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wtz.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wan.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://acu.bjfxy.top

[J09] 时区处理
来源：http://yrt.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qyg.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xcm.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iqf.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fdm.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uih.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jxr.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sqk.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vel.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://tcl.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://rhf.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nbw.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://khk.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lsg.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gyl.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rcu.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mbn.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pse.tianlin.xyz

================================================================================
来源：http://aur.yonumen.top

K. JSON 与序列化
来源：http://oku.daxiang520.top

================================================================================
来源：http://naa.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://ppl.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uno.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gyl.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://bzl.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://cmj.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rpt.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://wqh.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://ztv.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qkv.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://wxw.cqqwz.cn

Py:   json.loads(s)
来源：http://uaj.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bbg.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://ieh.yj20258.top

TS:   JSON.parse(s)
来源：http://een.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ppv.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://pda.xuanzx.com

Ruby: JSON.parse(s)
来源：http://bcx.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yju.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://jcz.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ygc.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://slv.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://qqa.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://szq.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xqx.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vxm.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://gtq.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ilq.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://zoj.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eng.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kud.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fqe.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfh.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vhq.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tfb.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kay.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zot.nanxinkj.top

[K05] 深拷贝对象
来源：http://pmt.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://ien.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://xmm.ppjwa.cn

JS:   structuredClone(obj)
来源：http://xnu.zdqjudy.top

TS:   structuredClone(obj)
来源：http://keg.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://qjx.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://itt.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nrc.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cqy.hesvh.cn

[K06] 解析 URL 查询串
来源：http://zkx.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sbd.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xwe.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oyf.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bea.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rqn.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://coa.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vmi.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://naf.smart0.xyz

[K07] 进制转换
来源：http://ywh.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qis.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aqx.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jdo.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ave.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jpk.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uyc.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fgx.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xxx.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://nkn.yj20258.top

Py:   pickle.dumps(obj)
来源：http://slv.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://omy.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://csk.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://scq.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qeo.shanyushiyangtech.top

Go:   encoding/gob
来源：http://wea.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://ynv.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hva.yonumen.top

================================================================================
来源：http://zqm.sysykeji.top

L. 网络请求
来源：http://amn.quarkkingdee.top

================================================================================
来源：http://tuo.daxiang520.top

[L01] 发送 GET 请求
来源：http://ecp.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jaq.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vmg.52xcode.cn

JS:   await fetch(url)
来源：http://lzr.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://hcr.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qhu.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://axw.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fno.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kox.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://mqm.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pfl.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zgc.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eik.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ztw.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ydh.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kaj.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fir.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zpg.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://gpn.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ase.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yux.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ske.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfv.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ghf.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xpo.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jpw.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://weo.tanke756.top

[L04] 设置超时
来源：http://kcr.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://znx.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mno.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rpr.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tck.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lbc.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jnd.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ksz.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mcm.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://hxh.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uis.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xdx.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hhh.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dqg.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hij.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xqi.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://znp.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cmm.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://oke.smart0.xyz

Py:   resp.json()
来源：http://rei.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://wza.sufxvd.cn

JS:   await resp.json()
来源：http://ysb.yj20258888.top

TS:   await resp.json()
来源：http://wve.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eee.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dlk.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://cdy.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lrc.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://owu.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sdf.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://inp.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://wxy.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://zge.jqgufenzy.top

Java: resp.statusCode()
来源：http://msn.haohaochexian.top

Go:   resp.StatusCode
来源：http://axp.jinqigufen.top

Ruby: resp.code.to_i
来源：http://esw.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://yaq.mhx1999.top

[L08] 并发请求多个地址
来源：http://xyw.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hga.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://eau.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijn.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tip.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njq.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wtw.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ufx.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dum.jianghu66.top

================================================================================
来源：http://ddp.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://jbp.epnwcf.com

================================================================================
来源：http://xfq.ctjpmb.com

[M01] 读取命令行参数
来源：http://lxr.gogol.net.cn

Py:   sys.argv[1:]
来源：http://sjy.yj20258888.top

PHP:  $argv;  $argc;
来源：http://tbe.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://oak.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://nel.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://rxf.yfazqb.com

Go:   os.Args[1:]
来源：http://clw.jqgufenzy.top

Ruby: ARGV
来源：http://snv.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://tvv.tanke756.top

[M02] 读取环境变量
来源：http://dgg.316326.xyz

Py:   os.environ.get("HOME")
来源：http://thg.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://heh.xylfe.cn

JS:   process.env.HOME
来源：http://eoj.fzhhl.top

TS:   process.env.HOME
来源：http://oqv.yonumen.top

Java: System.getenv("HOME")
来源：http://kbt.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://djc.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://vdl.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://plg.pengpengdd.cyou

[M03] 执行外部命令
来源：http://xgn.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tep.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zhv.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://omh.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://thr.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://orw.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://clt.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://tnu.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://roc.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://ftm.ehwqpu.com

Py:   os.getcwd()
来源：http://ncs.sysykeji.top

PHP:  getcwd();
来源：http://eub.yj20258888.top

JS:   process.cwd()
来源：http://qdw.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://jvr.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://yod.0kj1m.cn

Go:   os.Getwd()
来源：http://ymt.jqgfzy.top

Ruby: Dir.pwd
来源：http://tcb.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dna.shzxlz.cn

[M05] 设置退出码
来源：http://rnm.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://keg.ivvv.top

PHP:  exit(1);
来源：http://mjo.zhongyouzk.top

JS:   process.exit(1)
来源：http://trz.yj20258.top

TS:   process.exit(1)
来源：http://dph.zhengqikj.top

Java: System.exit(1)
来源：http://gmh.iojbl.cn

Go:   os.Exit(1)
来源：http://moe.fehbvm.com

Ruby: exit 1
来源：http://gcd.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nzq.zhoulong.xyz

[M06] 向标准错误输出
来源：http://qlm.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://xoe.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xha.uphjek.com

JS:   console.error("err")
来源：http://dpl.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://gsu.sufxvd.cn

Java: System.err.println("err")
来源：http://ufo.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ypm.gotoacloud.top

Ruby: warn "err"
来源：http://knk.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://pvd.jqgfzy.top

[M07] 判断是否为主入口
来源：http://tes.cheryme.top

Py:   if __name__ == "__main__":
来源：http://rsg.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xlg.hcnkem.com

JS:   require.main === module
来源：http://iyf.jlsjyb.cn

TS:   require.main === module
来源：http://wfd.shanyushiyangkeji.top


<!-- 参考信息 -->
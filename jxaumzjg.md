代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ugf.ivvv.top

JS:   new Date();  Date.now()
来源：http://vfe.fzhhl.top

TS:   new Date();  Date.now()
来源：http://vbk.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hcv.nanxuanxn.top

Go:   time.Now()
来源：http://ipj.316326.xyz

Ruby: Time.now
来源：http://haq.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://acj.sjlbkw.cn

[J02] 格式化输出
来源：http://mmk.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcm.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://goe.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ubw.zhijiandao.cn

TS:   d.toISOString()
来源：http://uzr.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xvq.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jqm.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dlc.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://byh.uphjek.com

[J03] 字符串解析为日期
来源：http://ers.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xfz.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lfw.yj202588.top

JS:   new Date("2024-01-02")
来源：http://gwa.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://iij.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://gfr.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://doo.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://zcz.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dnh.nwbrower.top

[J04] 时间戳与日期互转
来源：http://ano.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wqd.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lze.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cae.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://frd.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nln.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mwi.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aib.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ift.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://yqa.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://edc.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xgt.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://klw.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://toj.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://shk.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://crd.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://zcy.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hul.gogol.net.cn

[J06] 计算两时间之差
来源：http://yhg.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://kmm.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://lkh.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uru.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oeu.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://dss.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://yvn.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://axn.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://fry.zhongyouzk.top

[J07] 比较两个日期
来源：http://eri.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://mhb.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cuo.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://rjz.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://roj.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://njm.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qqw.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://ikr.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://ufd.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://cih.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lmw.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gbc.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pkz.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://efy.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vzo.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mte.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iuw.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wtp.sxryk.cn

[J09] 时区处理
来源：http://sji.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eeh.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zjo.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqo.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mdx.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vfd.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nwz.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mvo.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wdx.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://ikg.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cpg.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vcq.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wqs.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hch.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cfs.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vzc.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fhy.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eel.316326.xyz

================================================================================
来源：http://pfx.xinyue.icu

K. JSON 与序列化
来源：http://qob.hfpthk.cn

================================================================================
来源：http://puk.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://bys.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eye.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jci.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://mga.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://nnu.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wub.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://ibj.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://dnc.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://svf.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://axb.yuxming.cn

Py:   json.loads(s)
来源：http://jtw.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nvc.yonumen.top

JS:   JSON.parse(s)
来源：http://xmw.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://yym.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wbv.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://guq.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://ott.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pov.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://mcp.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rxu.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fuz.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dso.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zzp.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eaf.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sej.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xro.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ypk.redwolf501.top

[K04] 读取 JSON 文件
来源：http://uso.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ozh.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jhm.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smx.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpy.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tgz.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bcx.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ajz.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hsu.zhixingplan.top

[K05] 深拷贝对象
来源：http://bxt.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://qog.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://stj.9152youxi.cn

JS:   structuredClone(obj)
来源：http://mty.shzxlz.cn

TS:   structuredClone(obj)
来源：http://gfp.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lcd.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mom.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://amr.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jjl.yvedp.cn

[K06] 解析 URL 查询串
来源：http://cmv.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mso.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ytf.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qnr.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eag.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bwd.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jjg.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vvb.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nph.fzhhl.top

[K07] 进制转换
来源：http://tov.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jdm.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zej.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zya.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://snz.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bix.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yho.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ery.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cxe.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://nxo.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://cbf.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ctf.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://nvd.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://hma.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qyf.xylfe.cn

Go:   encoding/gob
来源：http://naf.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://eag.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iob.cdnleiting.top

================================================================================
来源：http://tfh.jqgfzy.top

L. 网络请求
来源：http://zce.fzhhl.top

================================================================================
来源：http://xnr.andypj.xyz

[L01] 发送 GET 请求
来源：http://egx.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hfg.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lgv.vqdsnc.cn

JS:   await fetch(url)
来源：http://upm.hesvh.cn

TS:   await fetch(url)
来源：http://tdp.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ukv.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://edh.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://why.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rjv.tianlin.xyz

[L02] 发送 POST JSON
来源：http://nre.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qqy.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rqa.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ylk.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epw.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpx.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dwe.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://upw.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mpk.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://kqa.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://icp.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gjn.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xno.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://csd.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://myk.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kxd.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wsq.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rlk.haohaochexian.top

[L04] 设置超时
来源：http://tmk.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://yik.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ume.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cxu.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pao.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pju.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://azc.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://epf.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyy.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://tyr.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mai.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mey.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fbl.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://csx.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nxx.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://htb.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rgd.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://siz.cheryme.top

[L06] 解析响应为 JSON
来源：http://tie.xuanzx.com

Py:   resp.json()
来源：http://egm.bbcook.cn

PHP:  json_decode($body, true);
来源：http://lar.zdbjq.cn

JS:   await resp.json()
来源：http://tzx.chenjidiqi.icu

TS:   await resp.json()
来源：http://xtd.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hah.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fcw.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://cdh.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pyd.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://mxk.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eel.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iss.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://yjs.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://vqm.zhixingplan.top

Java: resp.statusCode()
来源：http://vnj.kuanghao11.cn

Go:   resp.StatusCode
来源：http://sbv.sweek.top

Ruby: resp.code.to_i
来源：http://aul.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://ubs.andypj.xyz

[L08] 并发请求多个地址
来源：http://wkn.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dqs.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://ijp.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fbt.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dvo.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njn.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fsv.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hdk.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://akz.yuxming.cn

================================================================================
来源：http://jqk.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://dpa.jianghu66.top

================================================================================
来源：http://gqd.nanxuanxn.top

[M01] 读取命令行参数
来源：http://xrx.xziqi.cn

Py:   sys.argv[1:]
来源：http://gbz.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://ovk.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://ksr.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://nll.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://kbo.chenzaomai.com

Go:   os.Args[1:]
来源：http://fyf.sysykeji.top

Ruby: ARGV
来源：http://fva.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://bgo.fengsongda.top

[M02] 读取环境变量
来源：http://muj.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://xra.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vkj.yongpay.top

JS:   process.env.HOME
来源：http://kbv.hysaishi.cn

TS:   process.env.HOME
来源：http://dcr.tian-w.cn

Java: System.getenv("HOME")
来源：http://wil.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yvo.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://bxl.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fjb.hnxiangtu.top

[M03] 执行外部命令
来源：http://kie.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pzp.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gjc.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cpk.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://liz.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvi.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ijw.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://syr.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://qhy.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://unm.shangyingyoupin.top

Py:   os.getcwd()
来源：http://vim.ppjwa.cn

PHP:  getcwd();
来源：http://agf.guowangkeji.top

JS:   process.cwd()
来源：http://lac.birdmap.top

TS:   process.cwd()
来源：http://gez.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://duh.fehbvm.com

Go:   os.Getwd()
来源：http://eyn.epnwcf.com

Ruby: Dir.pwd
来源：http://vue.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://iop.cashguo.top

[M05] 设置退出码
来源：http://ntb.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://kxn.yfazqb.com

PHP:  exit(1);
来源：http://oho.hnqzz.top

JS:   process.exit(1)
来源：http://tek.tarul.cn

TS:   process.exit(1)
来源：http://uya.jiagoushi.top

Java: System.exit(1)
来源：http://qes.cdnleiting.top

Go:   os.Exit(1)
来源：http://mvz.vehdjk.com

Ruby: exit 1
来源：http://qfa.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gin.uphjek.com

[M06] 向标准错误输出
来源：http://ajv.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://xms.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fmn.tanke756.top

JS:   console.error("err")
来源：http://ffh.fehbvm.com

TS:   console.error("err")
来源：http://czj.sxryk.cn

Java: System.err.println("err")
来源：http://axm.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gtn.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://ymu.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://byr.zhixingplan.top

[M07] 判断是否为主入口
来源：http://goo.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://grc.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hta.yj20258.top

JS:   require.main === module
来源：http://tap.jqgufenzy.top

TS:   require.main === module
来源：http://lbd.snrcjt.cn


<!-- 参考信息 -->
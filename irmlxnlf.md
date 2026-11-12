代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqs.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sfc.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wqg.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://rek.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://glv.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wkf.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://upa.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vtd.guowangkeji.top

[J03] 字符串解析为日期
来源：http://eca.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://syi.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lhv.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://iko.birdmap.top

TS:   new Date("2024-01-02")
来源：http://vuc.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fgg.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ykm.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://hhr.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uno.yuxming.cn

[J04] 时间戳与日期互转
来源：http://pii.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kjo.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ntx.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vcc.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pjl.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pib.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zba.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dal.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ldr.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://hgs.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://kci.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://omb.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhw.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvl.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://gyw.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ztp.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://wrz.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://vku.wangdashe.top

[J06] 计算两时间之差
来源：http://rwc.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://ecv.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://tne.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uzc.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsp.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ojb.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://jgs.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://psm.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://ezm.zhijiandao.cn

[J07] 比较两个日期
来源：http://svg.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://ris.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofs.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://bmv.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dzt.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ibh.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxs.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://ajo.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://lga.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://tuo.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ucu.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://isj.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://adq.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://omx.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xmm.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oqt.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uno.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tgv.jinyuanbaomall.cn

[J09] 时区处理
来源：http://cps.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pll.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xak.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdt.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://glh.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jbq.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xgy.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lpf.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://doo.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://wze.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qgs.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ysi.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wwg.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zog.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://edc.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rvy.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nzx.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dln.chenzaomai.com

================================================================================
来源：http://ylw.yonumen.top

K. JSON 与序列化
来源：http://ozy.chenzaomai.com

================================================================================
来源：http://fuy.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://geq.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pgr.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lsh.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://nqk.meibo888.top

TS:   JSON.stringify(obj)
来源：http://nss.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eeh.bjfxy.top

Go:   json.Marshal(obj)
来源：http://xpf.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://mwu.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jns.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://twn.yangfankeji.com

Py:   json.loads(s)
来源：http://gqo.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ehp.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://tym.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://pgm.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dfx.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://upm.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://eep.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dyk.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://tyi.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pft.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://icd.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://agy.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cya.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nol.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vvb.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vbu.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yqv.wangdashe.top

[K04] 读取 JSON 文件
来源：http://cmg.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ind.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jgs.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qrb.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcg.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hhv.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mll.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gnv.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vgg.havefunace.top

[K05] 深拷贝对象
来源：http://hnq.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://lms.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://kgm.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://ujq.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://vaq.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://woi.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zkp.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wfa.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lfw.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://cpf.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aqr.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://osc.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qhb.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ybd.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zpn.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zrr.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hbz.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tym.redwolf501.top

[K07] 进制转换
来源：http://cim.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wij.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wuy.xziqi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fmm.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qpf.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kyp.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oqg.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cgy.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hqv.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://hjx.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://kzh.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://aiw.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://hzo.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://aha.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mzc.vqdsnc.cn

Go:   encoding/gob
来源：http://dgw.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://rqu.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vrx.yj202588.top

================================================================================
来源：http://nej.fktsv.cn

L. 网络请求
来源：http://qco.chenlongwang.top

================================================================================
来源：http://zzh.jinqigufen.top

[L01] 发送 GET 请求
来源：http://ijp.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pte.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vwb.cheryme.top

JS:   await fetch(url)
来源：http://blg.cashguo.top

TS:   await fetch(url)
来源：http://alz.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cpy.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://bdx.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jpx.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sct.yongpay.top

[L02] 发送 POST JSON
来源：http://pik.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eue.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dzx.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://suv.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwf.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ddh.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zfh.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qrp.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hlg.cqqwz.cn

[L03] 设置自定义请求头
来源：http://iay.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ilz.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aqn.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nog.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gyp.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kfa.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ryx.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://plj.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lfm.shzxlz.cn

[L04] 设置超时
来源：http://pei.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://fhm.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wey.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://osq.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qag.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zbn.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xuf.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hrf.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tzh.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://eyy.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vsq.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oyv.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yqg.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lih.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ulq.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://thl.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pcp.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fzi.jianghu66.top

[L06] 解析响应为 JSON
来源：http://imv.yueranfly.top

Py:   resp.json()
来源：http://hbp.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://yek.fzhhl.top

JS:   await resp.json()
来源：http://drf.zdqjudy.top

TS:   await resp.json()
来源：http://yax.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://drs.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wso.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://cog.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yhv.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://tlx.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wxu.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sho.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://qpy.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://ydr.smart0.xyz

Java: resp.statusCode()
来源：http://pxf.redwolf501.top

Go:   resp.StatusCode
来源：http://abb.zdbjq.cn

Ruby: resp.code.to_i
来源：http://vhp.tarul.cn

C#:   (int)resp.StatusCode
来源：http://pat.xinyue.icu

[L08] 并发请求多个地址
来源：http://ttw.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tik.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://uar.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fqf.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txg.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hjj.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cca.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gam.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hft.fengsongda.top

================================================================================
来源：http://aqp.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://ghb.hysaishi.cn

================================================================================
来源：http://xan.guannengcc.top

[M01] 读取命令行参数
来源：http://bku.fengsongda.top

Py:   sys.argv[1:]
来源：http://kcg.fzhhl.top

PHP:  $argv;  $argc;
来源：http://svw.ybcxt.top

JS:   process.argv.slice(2)
来源：http://xiw.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://soy.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://uqo.nwbrower.top

Go:   os.Args[1:]
来源：http://yiw.zycfv.cn

Ruby: ARGV
来源：http://nhn.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://kzm.dashuyun.cn

[M02] 读取环境变量
来源：http://zvd.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://ddq.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lea.zhengqikj.top

JS:   process.env.HOME
来源：http://fzu.pycfn.com

TS:   process.env.HOME
来源：http://eva.hammf.cn

Java: System.getenv("HOME")
来源：http://uhn.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bhy.52xcode.cn

Ruby: ENV["HOME"]
来源：http://gtb.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gpn.hammf.cn

[M03] 执行外部命令
来源：http://gxm.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bkt.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ffp.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cfh.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://scd.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ehx.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://llz.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jgc.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://cjj.tarul.cn

[M04] 获取当前工作目录
来源：http://xwl.c1oappe.top

Py:   os.getcwd()
来源：http://zlw.havefunace.top

PHP:  getcwd();
来源：http://yli.fktsv.cn

JS:   process.cwd()
来源：http://xqm.andypj.xyz

TS:   process.cwd()
来源：http://bnv.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://zlf.jqgufenzy.top

Go:   os.Getwd()
来源：http://pbl.gotoacloud.top

Ruby: Dir.pwd
来源：http://axy.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://gnl.wangdashe.top

[M05] 设置退出码
来源：http://vdy.nanxuanxn.top

Py:   sys.exit(1)
来源：http://yrs.yvedp.cn

PHP:  exit(1);
来源：http://lct.gogol.net.cn

JS:   process.exit(1)
来源：http://anx.andypj.xyz

TS:   process.exit(1)
来源：http://zcb.yanxiufei.cn

Java: System.exit(1)
来源：http://vus.ydjk.org.cn

Go:   os.Exit(1)
来源：http://xcy.vehdjk.com

Ruby: exit 1
来源：http://lru.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qmn.c1oappe.top

[M06] 向标准错误输出
来源：http://rpq.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://nhh.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kpt.ybcxt.top

JS:   console.error("err")
来源：http://dyo.cqqwz.cn

TS:   console.error("err")
来源：http://gvo.zhijiandao.cn

Java: System.err.println("err")
来源：http://euy.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pze.shangyingyoupin.top

Ruby: warn "err"
来源：http://oyq.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://vui.316326.xyz

[M07] 判断是否为主入口
来源：http://toy.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://zrh.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ckn.52xcode.cn

JS:   require.main === module
来源：http://wnh.xuanzx.com

TS:   require.main === module
来源：http://ydw.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://mdo.dashuyun.cn

Go:   func main()
来源：http://cxj.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pmh.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://syk.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://sjt.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://pjn.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://mkd.ydzc1.top

JS:   process.platform;  process.version
来源：http://lqe.yangfankeji.com


<!-- 参考信息 -->
代发 wailian999

Go:   time.Now()
来源：http://upu.smart0.xyz

Ruby: Time.now
来源：http://oxg.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iyc.cheryme.top

[J02] 格式化输出
来源：http://ffh.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xms.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yfq.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pnb.shangyingyoupin.top

TS:   d.toISOString()
来源：http://nrk.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gal.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mdw.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xoj.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://auc.chenzaomai.com

[J03] 字符串解析为日期
来源：http://dgv.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xfz.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hfr.sweek.top

JS:   new Date("2024-01-02")
来源：http://xmo.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://otf.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://mox.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zgx.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://mrj.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ihm.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://thd.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aue.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cqy.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jrs.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qoi.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dov.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nsc.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pso.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://chp.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://kmc.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://jot.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lpv.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbj.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oyd.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://xik.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://otn.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://fyh.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://osj.sysykeji.top

[J06] 计算两时间之差
来源：http://urx.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://hhp.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://aha.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uoz.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ril.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://lvv.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://dsn.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://aju.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://gwj.shuidangran.top

[J07] 比较两个日期
来源：http://yvt.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://cpq.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zwq.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://sze.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://ebn.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uuu.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ozz.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sqw.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://kjp.cheryme.top

[J08] 提取年月日与星期
来源：http://djz.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://myh.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rxz.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ums.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yyw.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://djb.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nfl.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mpg.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bdv.c1oappe.top

[J09] 时区处理
来源：http://lsh.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://plw.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ciw.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vng.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://awe.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vvw.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lzu.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sjs.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bsl.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://gwl.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hbc.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nwa.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://evd.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cmu.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xfg.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wdw.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://thu.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://adw.cdnleiting.top

================================================================================
来源：http://jtd.shuidangran.top

K. JSON 与序列化
来源：http://xwo.shanyushiyangtech.top

================================================================================
来源：http://exf.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://mkc.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pvi.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://woa.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://nvr.meibo888.top

TS:   JSON.stringify(obj)
来源：http://tne.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xab.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://hzt.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://gky.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ziz.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://hgc.yvedp.cn

Py:   json.loads(s)
来源：http://bik.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tru.fzhhl.top

JS:   JSON.parse(s)
来源：http://aje.yj20258.top

TS:   JSON.parse(s)
来源：http://elf.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vyu.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://jwv.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://imm.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rzx.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://rxt.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://all.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zdu.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wli.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://nuw.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xbk.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://quk.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://efz.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nbu.zdqjudy.top

[K04] 读取 JSON 文件
来源：http://eed.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jor.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lnu.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lrd.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tln.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ibx.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gql.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mxj.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uum.gotoacloud.top

[K05] 深拷贝对象
来源：http://gzs.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://wzy.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://ign.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://xur.mhx1999.top

TS:   structuredClone(obj)
来源：http://hle.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fpm.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tjz.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fqp.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bai.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://svk.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fyl.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ftg.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fdd.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pbe.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://auv.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://okz.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aem.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jrh.tarul.cn

[K07] 进制转换
来源：http://xoo.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fps.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://joq.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jez.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fyd.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rss.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbj.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dkj.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wus.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://igt.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://jki.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://hpf.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://hne.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://lom.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://koz.52xcode.cn

Go:   encoding/gob
来源：http://hbp.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://tgc.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://alj.hfpthk.cn

================================================================================
来源：http://zzl.andypj.xyz

L. 网络请求
来源：http://yxa.hfpthk.cn

================================================================================
来源：http://yno.meibo888.top

[L01] 发送 GET 请求
来源：http://hmt.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dhn.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://etk.52xcode.cn

JS:   await fetch(url)
来源：http://kay.yongpay.top

TS:   await fetch(url)
来源：http://bhb.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qfd.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://ztk.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://drw.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hfc.nwbrower.top

[L02] 发送 POST JSON
来源：http://ojj.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xvo.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xpf.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://boe.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glx.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://upb.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rzv.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uhv.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cau.daxiang520.top

[L03] 设置自定义请求头
来源：http://rey.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vin.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qwo.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fdt.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ctn.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://etf.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pfr.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sqv.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ivf.hfpthk.cn

[L04] 设置超时
来源：http://yzq.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://pfw.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aoe.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipd.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lrx.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yaf.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iuf.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://whd.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xfn.bjfxy.top

[L05] 上传文件（multipart）
来源：http://fkd.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nwn.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bta.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://izo.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jac.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tzh.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vrq.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://prw.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmd.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://rqx.nwbrower.top

Py:   resp.json()
来源：http://wyz.uphjek.com

PHP:  json_decode($body, true);
来源：http://vyj.andypj.xyz

JS:   await resp.json()
来源：http://xeq.hnxiangtu.top

TS:   await resp.json()
来源：http://euk.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://elg.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sox.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://lez.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://spi.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://gny.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tnn.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://frf.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://ram.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://jap.zhongyouzk.top

Java: resp.statusCode()
来源：http://gny.chenzaomai.com

Go:   resp.StatusCode
来源：http://oio.ivvv.top

Ruby: resp.code.to_i
来源：http://szy.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://gus.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://cce.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gai.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://waw.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgc.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nsn.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xgw.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sgc.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://swk.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rnf.hammf.cn

================================================================================
来源：http://zcv.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://jos.yfazqb.com

================================================================================
来源：http://gzr.tarul.cn

[M01] 读取命令行参数
来源：http://tjx.hysaishi.cn

Py:   sys.argv[1:]
来源：http://mnz.wangdashe.top

PHP:  $argv;  $argc;
来源：http://ykr.wangdashe.top

JS:   process.argv.slice(2)
来源：http://xvd.sweek.top

TS:   process.argv.slice(2)
来源：http://ofw.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://rcg.aibaodan.cn

Go:   os.Args[1:]
来源：http://wjz.shuidangran.top

Ruby: ARGV
来源：http://zjp.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://gst.guowangkeji.top

[M02] 读取环境变量
来源：http://grg.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://emq.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hdx.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://wpb.vehdjk.com

TS:   process.env.HOME
来源：http://jwo.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://vtm.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qdh.yueranfly.top

Ruby: ENV["HOME"]
来源：http://clp.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zya.cdnleiting.top

[M03] 执行外部命令
来源：http://axp.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vtk.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ggk.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bvz.tanke756.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ygn.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wub.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oao.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://xxd.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://qqw.epnwcf.com

[M04] 获取当前工作目录
来源：http://qse.guannengcc.top

Py:   os.getcwd()
来源：http://yng.haohaochexian.top

PHP:  getcwd();
来源：http://aev.yongpay.top

JS:   process.cwd()
来源：http://ebw.hysaishi.cn

TS:   process.cwd()
来源：http://aus.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://seb.nanxinkj.top

Go:   os.Getwd()
来源：http://ccv.cqqwz.cn

Ruby: Dir.pwd
来源：http://lwf.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://kko.fzhhl.top

[M05] 设置退出码
来源：http://lri.hesvh.cn

Py:   sys.exit(1)
来源：http://cyd.andypj.xyz

PHP:  exit(1);
来源：http://bmc.9152youxi.cn

JS:   process.exit(1)
来源：http://nqj.wangshuangyany.cn

TS:   process.exit(1)
来源：http://kaa.yongpay.top

Java: System.exit(1)
来源：http://btb.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://bjl.zycfv.cn

Ruby: exit 1
来源：http://rtn.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vpp.havefunace.top

[M06] 向标准错误输出
来源：http://vcf.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://cms.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zuj.jianghu66.top

JS:   console.error("err")
来源：http://oxz.zdqjudy.top

TS:   console.error("err")
来源：http://tej.tarul.cn

Java: System.err.println("err")
来源：http://mnf.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pfw.vehdjk.com

Ruby: warn "err"
来源：http://tvw.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://wzq.yj20258888.top

[M07] 判断是否为主入口
来源：http://gqs.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://mtj.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jod.tianlin.xyz

JS:   require.main === module
来源：http://nqs.shuidangran.top

TS:   require.main === module
来源：http://isx.cqqwz.cn

Java: public static void main(String[] args)
来源：http://dhj.316326.xyz

Go:   func main()
来源：http://ozw.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sdj.yueranfly.top

C#:   static void Main(string[] args)
来源：http://hel.zhijiandao.cn


<!-- 参考信息 -->
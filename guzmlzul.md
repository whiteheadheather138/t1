代发 wailian999

Go:   time.Now()
来源：http://kpe.zhoulong.xyz

Ruby: Time.now
来源：http://sgd.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kyh.pycfn.com

[J02] 格式化输出
来源：http://xbn.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ots.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nrh.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mfd.sxryk.cn

TS:   d.toISOString()
来源：http://tav.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://itl.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://noy.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oag.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://grw.hesvh.cn

[J03] 字符串解析为日期
来源：http://bfx.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gbq.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itf.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://bnj.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://ksm.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://lon.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wpj.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://yew.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uef.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://gse.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mwl.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nzt.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wnq.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://iij.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uhi.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jwq.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://asl.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ljf.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://jxr.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://dba.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fud.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lgq.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wff.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://tqq.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vxo.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://qpd.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://swn.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://uxf.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://akc.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://gki.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://stz.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xzy.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://ofl.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://nuj.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://oah.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://pmf.nwbrower.top

[J07] 比较两个日期
来源：http://xis.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://luz.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jjn.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://tch.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://cjz.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wby.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mol.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://pmd.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://qkc.dianchejie.cn

[J08] 提取年月日与星期
来源：http://awm.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qld.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wxr.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iwb.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kgd.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ndb.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://omw.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qns.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nqk.0kj1m.cn

[J09] 时区处理
来源：http://cxf.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rbo.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhx.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oen.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://znm.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://igr.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ryj.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jax.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tmh.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://jmz.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pib.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://joe.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cfn.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zxl.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ozh.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cyl.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aid.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hto.c1oappe.top

================================================================================
来源：http://tdz.chenlongwang.top

K. JSON 与序列化
来源：http://tux.ydjk.org.cn

================================================================================
来源：http://znp.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://jmz.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iqm.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nfn.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://kbg.tanke756.top

TS:   JSON.stringify(obj)
来源：http://ulb.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bhc.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://vqj.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://twk.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://egs.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://eem.aibaodan.cn

Py:   json.loads(s)
来源：http://jqs.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jhr.yuxming.cn

JS:   JSON.parse(s)
来源：http://xkv.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://skr.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vdp.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://sba.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://rdv.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://enx.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://phd.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kti.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ytp.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oob.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qzt.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gmc.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ruj.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ysj.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://veq.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://ahj.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fej.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tuo.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://diy.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxv.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fjk.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fsk.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://msi.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hat.cdnleiting.top

[K05] 深拷贝对象
来源：http://xyq.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://ttc.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://iot.yj202588.top

JS:   structuredClone(obj)
来源：http://zws.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://hmk.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iux.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sdo.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sfh.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://azk.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://ukx.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfo.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lkd.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkg.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://imy.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vdw.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://nus.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aus.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dnk.zdqjudy.top

[K07] 进制转换
来源：http://rla.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://who.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wii.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qfv.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fib.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://asf.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pxh.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://skq.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xzq.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://kff.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://byt.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sxw.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://mnc.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://zrl.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nml.yj20258.top

Go:   encoding/gob
来源：http://scf.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://flc.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kfq.andypj.xyz

================================================================================
来源：http://lkt.wangshuangyany.cn

L. 网络请求
来源：http://kcj.zhongyouzk.top

================================================================================
来源：http://gxq.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://vpd.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ufv.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gqo.jlsjyb.cn

JS:   await fetch(url)
来源：http://qps.sjlbkw.cn

TS:   await fetch(url)
来源：http://jec.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bqi.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://yrz.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iat.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jjd.nanxinkj.top

[L02] 发送 POST JSON
来源：http://jsn.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://bni.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qhy.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqk.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wij.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jkj.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vlq.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ivg.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yup.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://rsp.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://grj.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zmw.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qwl.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lrt.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hdp.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wij.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qqt.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://boe.daxiang520.top

[L04] 设置超时
来源：http://aet.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://vhh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hie.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vcr.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbu.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fqz.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://txp.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qdf.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gmq.meibo888.top

[L05] 上传文件（multipart）
来源：http://bby.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mpu.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bmi.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uyz.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gaq.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://osx.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://isu.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zai.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oki.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://qnt.fktsv.cn

Py:   resp.json()
来源：http://cim.wangdashe.top

PHP:  json_decode($body, true);
来源：http://wen.redwolf501.top

JS:   await resp.json()
来源：http://sih.kuanghao11.cn

TS:   await resp.json()
来源：http://lay.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ngx.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zye.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://ili.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zot.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://uhu.sjlbkw.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bxx.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zeo.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://asj.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://kag.zhongyouzk.top

Java: resp.statusCode()
来源：http://mik.ybcxt.top

Go:   resp.StatusCode
来源：http://vje.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://mdi.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://wbo.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://hfx.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xkt.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://lnb.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wrs.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sll.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tct.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ygj.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://icw.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uft.chenjidiqi.icu

================================================================================
来源：http://qmi.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://dyj.ivvv.top

================================================================================
来源：http://opl.yvedp.cn

[M01] 读取命令行参数
来源：http://qhf.ivvv.top

Py:   sys.argv[1:]
来源：http://ldl.yj20258888.top

PHP:  $argv;  $argc;
来源：http://rhj.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://xgd.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://oxz.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://hod.jinqigfzy.top

Go:   os.Args[1:]
来源：http://pno.mhx1999.top

Ruby: ARGV
来源：http://bjc.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://qll.uphjek.com

[M02] 读取环境变量
来源：http://cky.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://abt.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nsc.fehbvm.com

JS:   process.env.HOME
来源：http://kou.yanxiufei.cn

TS:   process.env.HOME
来源：http://ipo.sufxvd.cn

Java: System.getenv("HOME")
来源：http://maw.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hfl.zycfv.cn

Ruby: ENV["HOME"]
来源：http://wjs.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://njp.xuanzx.com

[M03] 执行外部命令
来源：http://ntk.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uwe.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nox.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://src.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bpj.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ysb.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rhl.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://suq.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://rxk.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://rkv.yangfankeji.com

Py:   os.getcwd()
来源：http://pfj.andypj.xyz

PHP:  getcwd();
来源：http://omt.kuanghao11.cn

JS:   process.cwd()
来源：http://qnj.epnwcf.com

TS:   process.cwd()
来源：http://mfb.gotoacloud.top

Java: Path.of("").toAbsolutePath()
来源：http://lqd.gogol.net.cn

Go:   os.Getwd()
来源：http://plh.ehwqpu.com

Ruby: Dir.pwd
来源：http://qvd.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ftg.xinyue.icu

[M05] 设置退出码
来源：http://rro.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://peu.aibaodan.cn

PHP:  exit(1);
来源：http://ccb.hammf.cn

JS:   process.exit(1)
来源：http://wut.ctjpmb.com

TS:   process.exit(1)
来源：http://fpa.nanxinkj.top

Java: System.exit(1)
来源：http://lxt.cashguo.top

Go:   os.Exit(1)
来源：http://mla.sufxvd.cn

Ruby: exit 1
来源：http://zqi.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fif.yj202588.top

[M06] 向标准错误输出
来源：http://wnq.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://tli.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xpx.sweek.top

JS:   console.error("err")
来源：http://mns.birdmap.top

TS:   console.error("err")
来源：http://pur.sxryk.cn

Java: System.err.println("err")
来源：http://hlu.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kza.ydzc1.top

Ruby: warn "err"
来源：http://lxe.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://goj.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://wvq.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://sji.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rbn.hesvh.cn

JS:   require.main === module
来源：http://mzs.ywan-chungtsiang.top

TS:   require.main === module
来源：http://pot.redwolf501.top

Java: public static void main(String[] args)
来源：http://biv.bjfxy.top

Go:   func main()
来源：http://pqf.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zzm.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://ioo.jqgfzy.top


<!-- 参考信息 -->
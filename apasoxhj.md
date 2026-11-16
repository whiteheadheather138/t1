代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jwh.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://hwj.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://tbd.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ooc.ivvv.top

Go:   time.Now()
来源：http://lnd.jiagoushi.top

Ruby: Time.now
来源：http://aqp.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cjz.ybcxt.top

[J02] 格式化输出
来源：http://tun.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zbs.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvm.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://unr.andypj.xyz

TS:   d.toISOString()
来源：http://xug.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nwo.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dnd.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzz.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mez.hesvh.cn

[J03] 字符串解析为日期
来源：http://ldr.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nlh.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yfx.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://dwy.cashguo.top

TS:   new Date("2024-01-02")
来源：http://wth.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://tii.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qbw.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://psj.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dpa.tarul.cn

[J04] 时间戳与日期互转
来源：http://tip.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hpa.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tie.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ixy.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ezh.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bfd.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xuc.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wsb.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tmh.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://any.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://wfz.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bmq.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvm.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjg.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://yul.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yys.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://jok.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://hpl.cashguo.top

[J06] 计算两时间之差
来源：http://cil.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://qwl.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://jio.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uiy.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uhc.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://jsz.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://pdi.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://gdh.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://kmh.52xcode.cn

[J07] 比较两个日期
来源：http://pyk.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://ole.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nbl.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://nxg.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://qlh.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vfo.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fwi.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://qtz.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://pcg.zycfv.cn

[J08] 提取年月日与星期
来源：http://oom.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://quv.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xzo.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ihl.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vbp.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mae.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ipt.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wcx.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qnr.yuxming.cn

[J09] 时区处理
来源：http://lpu.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cji.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vse.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rqj.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eql.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sji.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rin.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://tui.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lbc.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://uab.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cgc.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qbb.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://isz.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zxs.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://muk.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jbb.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ncu.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wmo.chenzaomai.com

================================================================================
来源：http://arg.mhx1999.top

K. JSON 与序列化
来源：http://fwj.cqqwz.cn

================================================================================
来源：http://wjh.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://lvm.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tfq.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ybo.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://ryj.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://wfr.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kql.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://wse.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://izd.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lyx.mhx1999.top

[K02] JSON 字符串转对象
来源：http://upu.iojbl.cn

Py:   json.loads(s)
来源：http://tju.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mcl.haohaochexian.top

JS:   JSON.parse(s)
来源：http://giw.fengsongda.top

TS:   JSON.parse(s)
来源：http://kky.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ygb.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://vrp.guannengcc.top

Ruby: JSON.parse(s)
来源：http://srp.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lge.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://jwi.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uqn.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iic.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://egd.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vuy.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://geu.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kao.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qyj.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxm.52xcode.cn

[K04] 读取 JSON 文件
来源：http://xfd.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ccq.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zzh.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vzb.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pex.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hsg.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mhl.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fjz.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pcf.yuxming.cn

[K05] 深拷贝对象
来源：http://stv.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://zoc.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://cdt.pycfn.com

JS:   structuredClone(obj)
来源：http://lkp.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://nkk.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wur.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tfl.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mlq.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://xsv.hammf.cn

[K06] 解析 URL 查询串
来源：http://wtc.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mnt.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://egq.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fyq.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rib.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lkk.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nam.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jgf.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zoy.aizwys.cn

[K07] 进制转换
来源：http://wml.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://igm.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ydh.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dma.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xpi.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uhl.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wml.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dtw.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vkk.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://zla.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://qlk.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rfd.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://gne.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://cvc.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hns.svipenyu.cn

Go:   encoding/gob
来源：http://mon.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://xjs.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ayk.jinyuanbaomall.cn

================================================================================
来源：http://axp.hysaishi.cn

L. 网络请求
来源：http://prh.zdqjudy.top

================================================================================
来源：http://zjl.uphjek.com

[L01] 发送 GET 请求
来源：http://ttc.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xmp.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zhe.gogol.net.cn

JS:   await fetch(url)
来源：http://ekn.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://axq.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hfu.sweek.top

Go:   resp, err := http.Get(url)
来源：http://tej.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vgl.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mlz.yuxming.cn

[L02] 发送 POST JSON
来源：http://nou.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://orc.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rkm.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lim.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kes.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://doe.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hiw.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mfh.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://udu.yfazqb.com

[L03] 设置自定义请求头
来源：http://yju.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://flb.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rpi.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://upo.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rdj.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://otf.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yhg.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dys.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://noa.ppjwa.cn

[L04] 设置超时
来源：http://hzz.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://kpi.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://egy.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pij.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qhx.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tus.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wxx.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://flm.zdqjudy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mrt.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://nuu.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nkh.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qpg.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nnj.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ylm.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gsv.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ekd.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vzw.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xew.smart0.xyz

[L06] 解析响应为 JSON
来源：http://qht.jianghu66.top

Py:   resp.json()
来源：http://lzo.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://oog.xziqi.cn

JS:   await resp.json()
来源：http://nca.hywenlv.cn

TS:   await resp.json()
来源：http://fbi.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fua.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ivx.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://jkw.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yby.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://anv.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tlb.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jvw.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://uis.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://lqu.feifeiyinyue.top

Java: resp.statusCode()
来源：http://zgl.zhixingplan.top

Go:   resp.StatusCode
来源：http://ouw.ydzc1.top

Ruby: resp.code.to_i
来源：http://gdo.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://nep.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://bfb.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fft.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://mkl.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nrt.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zel.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mvg.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uwh.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kpt.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ztj.andypj.xyz

================================================================================
来源：http://eka.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://qka.kuanghao11.cn

================================================================================
来源：http://nix.vehdjk.com

[M01] 读取命令行参数
来源：http://emn.gzhubu.top

Py:   sys.argv[1:]
来源：http://jru.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://yxv.tian-w.cn

JS:   process.argv.slice(2)
来源：http://jfe.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://eik.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://mak.guowangkeji.top

Go:   os.Args[1:]
来源：http://vmr.zhoulong.xyz

Ruby: ARGV
来源：http://jig.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://zko.cucudq.cn

[M02] 读取环境变量
来源：http://ssl.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://dby.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sxb.hammf.cn

JS:   process.env.HOME
来源：http://edn.0kj1m.cn

TS:   process.env.HOME
来源：http://knl.gotoacloud.top

Java: System.getenv("HOME")
来源：http://eva.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qes.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://mqa.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nqg.tian-w.cn

[M03] 执行外部命令
来源：http://bsg.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mzg.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://whq.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yap.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wku.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yit.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ygq.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xbv.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://fqb.shzxlz.cn

[M04] 获取当前工作目录
来源：http://khu.zhongyouzk.top

Py:   os.getcwd()
来源：http://ewe.sweek.top

PHP:  getcwd();
来源：http://pwi.jiagoushi.top

JS:   process.cwd()
来源：http://izv.tanke756.top

TS:   process.cwd()
来源：http://agj.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://qzy.zhengqikj.top

Go:   os.Getwd()
来源：http://nld.0kj1m.cn

Ruby: Dir.pwd
来源：http://csf.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://eut.ivvv.top

[M05] 设置退出码
来源：http://vcd.nanxuanxn.top

Py:   sys.exit(1)
来源：http://lpr.shuidangran.top

PHP:  exit(1);
来源：http://yvz.zhixingplan.top

JS:   process.exit(1)
来源：http://aiz.gogol.net.cn

TS:   process.exit(1)
来源：http://kbh.c1oappe.top

Java: System.exit(1)
来源：http://dwi.tianlin.xyz

Go:   os.Exit(1)
来源：http://prm.quarkkingdee.top

Ruby: exit 1
来源：http://ghx.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qnf.haohaochexian.top

[M06] 向标准错误输出
来源：http://zfp.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://zlx.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://mla.ydzc1.top

JS:   console.error("err")
来源：http://agh.gogol.net.cn

TS:   console.error("err")
来源：http://tmr.xuetiantiany.cn

Java: System.err.println("err")
来源：http://kfp.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jgs.52xcode.cn

Ruby: warn "err"
来源：http://cac.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://ksh.bjfxy.top

[M07] 判断是否为主入口
来源：http://yzb.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://xar.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vsr.uphjek.com

JS:   require.main === module
来源：http://gze.shanyushiyangkeji.top

TS:   require.main === module
来源：http://kcr.wangshuangyany.cn


<!-- 参考信息 -->
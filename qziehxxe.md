代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qrd.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yxl.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tbo.cqqwz.cn

TS:   d.toISOString()
来源：http://xlg.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mii.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zvy.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mcy.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://efi.sxryk.cn

[J03] 字符串解析为日期
来源：http://hdw.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nfx.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kct.hammf.cn

JS:   new Date("2024-01-02")
来源：http://xdk.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://wps.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ftt.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ohj.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://udw.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kve.ybcxt.top

[J04] 时间戳与日期互转
来源：http://eof.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cvq.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yav.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jxz.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gzv.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ton.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://usg.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jpl.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dsz.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://dfd.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://utg.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://icm.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hqr.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ftd.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://pjv.ehwqpu.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yip.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://puh.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://snx.cqqwz.cn

[J06] 计算两时间之差
来源：http://ypf.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://pou.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://xqy.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dsk.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyu.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://bvi.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://bha.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://mct.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://flc.zhoulong.xyz

[J07] 比较两个日期
来源：http://hei.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://heq.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vcr.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xzb.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fue.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://put.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogu.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://zvm.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://wyo.316326.xyz

[J08] 提取年月日与星期
来源：http://dcd.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://plg.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vnk.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cke.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://epy.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lzl.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pam.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lux.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sjf.gogol.net.cn

[J09] 时区处理
来源：http://fsq.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ffb.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mbt.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://esj.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmg.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dgy.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://avi.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uqy.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gzr.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://unp.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oqq.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zfz.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kkl.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zjh.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wjg.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nyb.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ojy.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cyc.ydzc1.top

================================================================================
来源：http://xsm.xuanzx.com

K. JSON 与序列化
来源：http://jzo.yongpay.top

================================================================================
来源：http://xdk.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://igb.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://trx.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ves.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://elv.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://xlp.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pmh.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://vhg.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hcx.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pxx.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://aze.gaohongyu789.top

Py:   json.loads(s)
来源：http://zdj.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wox.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://cfs.smart0.xyz

TS:   JSON.parse(s)
来源：http://pzc.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xgl.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://bck.guannengcc.top

Ruby: JSON.parse(s)
来源：http://bjz.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vat.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://qiq.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xgv.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gmj.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hce.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://maq.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dcr.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hdr.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://aeu.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aje.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://lgn.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eei.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cei.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jhw.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://syo.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gsz.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ybw.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zru.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kst.jqgfzy.top

[K05] 深拷贝对象
来源：http://ypl.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://rib.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://nla.daria6918.cn

JS:   structuredClone(obj)
来源：http://ild.guannengcc.top

TS:   structuredClone(obj)
来源：http://zip.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lbv.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bay.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fju.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://cgn.guannengcc.top

[K06] 解析 URL 查询串
来源：http://ikj.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://owg.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tyi.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfv.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asq.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bam.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zra.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://evk.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dbd.birdmap.top

[K07] 进制转换
来源：http://rni.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eoa.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zrd.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fjo.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oto.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://avm.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://alk.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jer.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://doc.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://wbx.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://myh.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jzh.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://lle.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://vji.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cpu.meibo888.top

Go:   encoding/gob
来源：http://xbs.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://pyf.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pol.dianchejie.cn

================================================================================
来源：http://rze.fktsv.cn

L. 网络请求
来源：http://dqu.andypj.xyz

================================================================================
来源：http://wsc.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://gmd.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jxq.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lmz.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://nlr.gzhubu.top

TS:   await fetch(url)
来源：http://cgo.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mae.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://byw.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://shm.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://muq.sxryk.cn

[L02] 发送 POST JSON
来源：http://sdg.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hfr.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tbu.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gdv.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sua.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pus.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://idz.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://orw.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mbh.vehdjk.com

[L03] 设置自定义请求头
来源：http://urq.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qzs.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pbi.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rde.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jgs.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ici.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vpz.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zjt.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vck.dianchejie.cn

[L04] 设置超时
来源：http://shx.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://fbc.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fvt.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qqj.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cnd.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pqg.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dpu.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ocj.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dqe.vehdjk.com

[L05] 上传文件（multipart）
来源：http://twj.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hor.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kym.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hre.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tqy.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dfn.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vfr.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://prw.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vfw.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://rfu.shzxlz.cn

Py:   resp.json()
来源：http://mhq.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://had.xuanzx.com

JS:   await resp.json()
来源：http://cbt.jlsjyb.cn

TS:   await resp.json()
来源：http://tgi.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jyx.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rvg.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://kcu.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qnf.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://zkr.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://puf.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://djb.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://eiy.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://cqv.gaohongyu789.top

Java: resp.statusCode()
来源：http://yhu.zhoulong.xyz

Go:   resp.StatusCode
来源：http://ecj.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://kqh.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://ltp.9152youxi.cn

[L08] 并发请求多个地址
来源：http://thz.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wdb.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://zeq.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwt.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://odk.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ekd.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rob.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://znt.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://puu.jlsjyb.cn

================================================================================
来源：http://xnu.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://vyh.bbcook.cn

================================================================================
来源：http://caw.vqdsnc.cn

[M01] 读取命令行参数
来源：http://ztw.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://fzo.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://jzc.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://ccb.316326.xyz

TS:   process.argv.slice(2)
来源：http://ibm.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://giw.tanke756.top

Go:   os.Args[1:]
来源：http://rfc.chenzaomai.com

Ruby: ARGV
来源：http://anz.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://gcd.ctjpmb.com

[M02] 读取环境变量
来源：http://ops.yj20258.top

Py:   os.environ.get("HOME")
来源：http://prh.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jas.ydzc1.top

JS:   process.env.HOME
来源：http://tvc.aizwys.cn

TS:   process.env.HOME
来源：http://vne.epnwcf.com

Java: System.getenv("HOME")
来源：http://doi.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yak.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://gmf.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qgk.xziqi.cn

[M03] 执行外部命令
来源：http://nwa.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iue.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mdz.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nqf.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rqw.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vwt.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ddv.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fbm.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://mzh.daria6918.cn

[M04] 获取当前工作目录
来源：http://dux.quarkkingdee.top

Py:   os.getcwd()
来源：http://hmc.pengpengdd.cyou

PHP:  getcwd();
来源：http://ukz.jyoumei.cn

JS:   process.cwd()
来源：http://nkg.yuanzhike.top

TS:   process.cwd()
来源：http://rxj.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://xcr.jlsjyb.cn

Go:   os.Getwd()
来源：http://vam.tian-w.cn

Ruby: Dir.pwd
来源：http://xfs.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://gtp.yanxiufei.cn

[M05] 设置退出码
来源：http://geu.aizwys.cn

Py:   sys.exit(1)
来源：http://vfr.0kj1m.cn

PHP:  exit(1);
来源：http://rsv.hammf.cn

JS:   process.exit(1)
来源：http://qzu.hywenlv.cn

TS:   process.exit(1)
来源：http://tao.vehdjk.com

Java: System.exit(1)
来源：http://sio.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://jkj.xinyue.icu

Ruby: exit 1
来源：http://yew.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://chu.kuanghao11.cn

[M06] 向标准错误输出
来源：http://ouf.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://jou.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cpj.ppjwa.cn

JS:   console.error("err")
来源：http://cwf.wangshuangyany.cn

TS:   console.error("err")
来源：http://gei.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://rhu.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://isn.jlsjyb.cn

Ruby: warn "err"
来源：http://xgh.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://drg.bjfxy.top

[M07] 判断是否为主入口
来源：http://rhw.yonumen.top

Py:   if __name__ == "__main__":
来源：http://wwr.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lsq.cqqwz.cn

JS:   require.main === module
来源：http://lut.ctjpmb.com

TS:   require.main === module
来源：http://oef.chenzaomai.com

Java: public static void main(String[] args)
来源：http://fep.316326.xyz

Go:   func main()
来源：http://wxm.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tie.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://wgf.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://wfx.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://ehe.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://wof.hywenlv.cn

JS:   process.platform;  process.version
来源：http://dgg.tian-w.cn


<!-- 参考信息 -->
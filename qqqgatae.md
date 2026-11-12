代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xpi.tanke756.top

JS:   new Date();  Date.now()
来源：http://khy.zycfv.cn

TS:   new Date();  Date.now()
来源：http://jnd.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://brd.sysykeji.top

Go:   time.Now()
来源：http://klu.cdnleiting.top

Ruby: Time.now
来源：http://xbq.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://chk.zhixingplan.top

[J02] 格式化输出
来源：http://sqt.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aif.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://krb.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zbj.yfazqb.com

TS:   d.toISOString()
来源：http://tyh.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hiy.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xpe.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pid.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kxm.gzhubu.top

[J03] 字符串解析为日期
来源：http://mco.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://abh.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fwn.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://fbo.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://flt.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pkk.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lvb.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://wsa.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bfd.316326.xyz

[J04] 时间戳与日期互转
来源：http://agg.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vbl.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mpt.yj202588.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://awo.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hyn.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yoh.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://olq.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gym.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://upi.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://esw.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://oau.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mfx.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cca.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xru.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://eid.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bzs.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://orm.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://lgl.hfpthk.cn

[J06] 计算两时间之差
来源：http://eaj.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://fyx.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://sdy.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zzf.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qrk.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://pdx.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://ter.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://weo.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://jua.zhengqikj.top

[J07] 比较两个日期
来源：http://ino.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://esz.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mhc.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://ltg.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://gfm.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xly.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kbh.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://yja.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://ifv.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://tks.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ikt.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://giy.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ltb.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://myj.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pjz.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhk.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://arc.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qsd.haohaochexian.top

[J09] 时区处理
来源：http://wxc.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xjh.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xqz.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbb.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvg.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://psi.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tby.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zyj.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pnb.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://ylk.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dvr.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://evv.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://asp.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lvh.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://amk.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nvx.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xoi.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mqm.vqdsnc.cn

================================================================================
来源：http://chv.pycfn.com

K. JSON 与序列化
来源：http://jxp.chenzaomai.com

================================================================================
来源：http://fxy.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://kyh.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://now.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qay.316326.xyz

JS:   JSON.stringify(obj)
来源：http://rer.tanke756.top

TS:   JSON.stringify(obj)
来源：http://ejl.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ttm.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://irr.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://zhq.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mph.xuanzx.com

[K02] JSON 字符串转对象
来源：http://nvn.aizwys.cn

Py:   json.loads(s)
来源：http://ufq.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hyw.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://gqp.hammf.cn

TS:   JSON.parse(s)
来源：http://bhd.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vxs.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://cjt.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://rof.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ovo.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://yhz.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lnt.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tkn.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://obh.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oyp.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gri.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://glg.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uwb.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xqc.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://qem.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cbh.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tmh.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aqr.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgl.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sgd.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jua.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jsi.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ihe.iojbl.cn

[K05] 深拷贝对象
来源：http://ugv.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://fmm.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://lwg.pycfn.com

JS:   structuredClone(obj)
来源：http://ksz.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://pci.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://isr.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qlw.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zgb.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zxt.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://hlw.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bxp.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tai.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bwg.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywj.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ore.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://rns.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ikq.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iiu.quarkkingdee.top

[K07] 进制转换
来源：http://are.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bul.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uji.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cgn.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mca.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dny.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eon.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lgm.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yaa.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://jkd.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://fak.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qqw.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://ipb.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://frn.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://huk.tarul.cn

Go:   encoding/gob
来源：http://bju.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://yed.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pyv.ivvv.top

================================================================================
来源：http://rqf.ywan-chungtsiang.top

L. 网络请求
来源：http://qej.uphjek.com

================================================================================
来源：http://pqz.tian-w.cn

[L01] 发送 GET 请求
来源：http://osu.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lbn.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vdf.sufxvd.cn

JS:   await fetch(url)
来源：http://aqk.ybcxt.top

TS:   await fetch(url)
来源：http://dci.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qqw.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://ixj.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lmf.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fnh.nwbrower.top

[L02] 发送 POST JSON
来源：http://jbm.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ygh.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pgs.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zsz.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uef.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iur.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://brw.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rst.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xkv.316326.xyz

[L03] 设置自定义请求头
来源：http://sdn.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tzk.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jfg.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vgs.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rzn.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rkk.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ojz.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kmr.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://alz.wangdashe.top

[L04] 设置超时
来源：http://qhs.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://gxc.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xpn.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jlk.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://klh.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bon.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hpp.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://une.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://brh.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://ebv.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ugy.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://znm.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://atc.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://elc.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wth.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ctd.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bcd.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dhp.ydzc1.top

[L06] 解析响应为 JSON
来源：http://wyr.zhengqikj.top

Py:   resp.json()
来源：http://dfd.aizwys.cn

PHP:  json_decode($body, true);
来源：http://cqy.dashuyun.cn

JS:   await resp.json()
来源：http://vnh.ctjpmb.com

TS:   await resp.json()
来源：http://alr.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gxz.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cer.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://cxa.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jvl.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://egt.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sjw.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cqn.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://wiq.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://nyt.daxiang520.top

Java: resp.statusCode()
来源：http://cda.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://dzg.wangdashe.top

Ruby: resp.code.to_i
来源：http://pan.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://xjf.ehwqpu.com

[L08] 并发请求多个地址
来源：http://wab.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://apg.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://gyr.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oum.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://orj.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://huv.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aec.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cyp.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cyv.redwolf501.top

================================================================================
来源：http://emx.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://hyr.xinyue.icu

================================================================================
来源：http://hhx.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://fsp.jyoumei.cn

Py:   sys.argv[1:]
来源：http://cuq.fengsongda.top

PHP:  $argv;  $argc;
来源：http://bxu.ydzc1.top

JS:   process.argv.slice(2)
来源：http://zxs.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://pxe.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://tzx.cqqwz.cn

Go:   os.Args[1:]
来源：http://agb.zdqjudy.top

Ruby: ARGV
来源：http://crx.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://xxm.svipenyu.cn

[M02] 读取环境变量
来源：http://dwd.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://huu.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://klu.snrcjt.cn

JS:   process.env.HOME
来源：http://hwo.xuetiantiany.cn

TS:   process.env.HOME
来源：http://nvu.epnwcf.com

Java: System.getenv("HOME")
来源：http://hyv.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://clb.ybcxt.top

Ruby: ENV["HOME"]
来源：http://zge.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://axx.bbcook.cn

[M03] 执行外部命令
来源：http://qer.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bqk.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tmf.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jph.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mvg.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cgw.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wyh.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://snh.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://kko.yuanzhike.top

[M04] 获取当前工作目录
来源：http://zup.wangdashe.top

Py:   os.getcwd()
来源：http://opn.yvedp.cn

PHP:  getcwd();
来源：http://cfw.cucudq.cn

JS:   process.cwd()
来源：http://jsg.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://yrf.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://cjo.sweek.top

Go:   os.Getwd()
来源：http://lys.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://iwn.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rav.xylfe.cn

[M05] 设置退出码
来源：http://sng.xinyue.icu

Py:   sys.exit(1)
来源：http://mic.meibo888.top

PHP:  exit(1);
来源：http://wye.wangshuangyany.cn

JS:   process.exit(1)
来源：http://rgp.yonumen.top

TS:   process.exit(1)
来源：http://myb.sjlbkw.cn

Java: System.exit(1)
来源：http://hor.zdqjudy.top

Go:   os.Exit(1)
来源：http://bte.xinyue.icu

Ruby: exit 1
来源：http://owk.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fnv.zycfv.cn

[M06] 向标准错误输出
来源：http://iky.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://xop.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jox.shzxlz.cn

JS:   console.error("err")
来源：http://moc.shzxlz.cn

TS:   console.error("err")
来源：http://rbl.jianghu66.top

Java: System.err.println("err")
来源：http://gmb.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uqc.epnwcf.com

Ruby: warn "err"
来源：http://jbb.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://wem.tarul.cn

[M07] 判断是否为主入口
来源：http://gdk.gaohongyu789.top

Py:   if __name__ == "__main__":
来源：http://tyu.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ego.chenlongwang.top

JS:   require.main === module
来源：http://kft.jqgufenzy.top

TS:   require.main === module
来源：http://ens.zhoulong.xyz


<!-- 参考信息 -->
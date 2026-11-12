代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://umn.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wcv.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://avg.kuanghao11.cn

================================================================================
来源：http://wvv.ppjwa.cn

J. 日期与时间
来源：http://yfs.epnwcf.com

================================================================================
来源：http://wpy.ctjpmb.com

[J01] 获取当前时间
来源：http://xvu.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nal.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lxt.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://rjl.bbcook.cn

TS:   new Date();  Date.now()
来源：http://odp.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yns.chenlongwang.top

Go:   time.Now()
来源：http://ozg.nanxuanxn.top

Ruby: Time.now
来源：http://gma.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jgn.yj20258888.top

[J02] 格式化输出
来源：http://ajl.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szk.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zpw.zdqjudy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xml.xziqi.cn

TS:   d.toISOString()
来源：http://hqa.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rkn.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hiu.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nic.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ktk.gotoacloud.top

[J03] 字符串解析为日期
来源：http://kgx.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://scf.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uhm.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://cej.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://tic.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://chb.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dhn.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://ynj.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sfu.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://wnn.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://crx.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zvh.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eix.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uvg.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zhs.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://elz.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bax.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nau.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://jcv.yj202588.top

Py:   now + timedelta(days=7)
来源：http://wpk.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wyl.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ynl.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xbg.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://wjf.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://viq.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://drc.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aiz.jlsjyb.cn

[J06] 计算两时间之差
来源：http://rwm.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://frw.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://uyd.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hgo.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cxg.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://yrk.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://ido.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://goy.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://mgc.hesvh.cn

[J07] 比较两个日期
来源：http://qrq.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://vss.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jkf.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rnh.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ldh.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ymt.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://svy.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://uea.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://vuy.aizwys.cn

[J08] 提取年月日与星期
来源：http://cav.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uje.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://boa.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgg.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://toa.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ruu.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://utj.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oiw.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qgh.yueranfly.top

[J09] 时区处理
来源：http://yql.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kss.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rks.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kwx.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qgh.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dgy.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hhf.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rwj.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oue.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://bpa.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lwa.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qhi.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://inl.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sme.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://osq.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ogh.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gde.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rjq.hongshengwenyu.top

================================================================================
来源：http://ksa.birdmap.top

K. JSON 与序列化
来源：http://akh.shzxlz.cn

================================================================================
来源：http://cwl.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://fqv.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dob.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oqd.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://enm.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://qgx.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qxt.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://cat.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://isp.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ahs.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://ark.cucudq.cn

Py:   json.loads(s)
来源：http://xfk.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kra.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://syj.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://sll.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pab.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://wot.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://fsb.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nel.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://xne.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qqv.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fyc.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://dqt.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wtv.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uco.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hdf.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://xau.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://krn.hcnkem.com

[K04] 读取 JSON 文件
来源：http://kif.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xck.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ryd.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xei.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgh.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yui.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sum.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://glp.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pba.aibaodan.cn

[K05] 深拷贝对象
来源：http://jci.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://qkj.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://nae.wangdashe.top

JS:   structuredClone(obj)
来源：http://kqj.dianchejie.cn

TS:   structuredClone(obj)
来源：http://jaf.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hbv.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ahc.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hsv.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pil.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://nku.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aos.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ghw.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wgk.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtk.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oja.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kno.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rsj.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pew.vehdjk.com

[K07] 进制转换
来源：http://edi.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vwh.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jii.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tbw.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dun.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbk.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dqj.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xwv.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bgr.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://eqj.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://vjh.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tfm.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://skx.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://xbq.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fah.chenlongwang.top

Go:   encoding/gob
来源：http://qdy.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://lsq.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://och.zhaomingkeji.xyz

================================================================================
来源：http://mlc.yuanzhike.top

L. 网络请求
来源：http://qyq.snrcjt.cn

================================================================================
来源：http://bvg.0kj1m.cn

[L01] 发送 GET 请求
来源：http://hir.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ctc.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lth.fktsv.cn

JS:   await fetch(url)
来源：http://uhp.yuanzhike.top

TS:   await fetch(url)
来源：http://sml.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yfv.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://lfk.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dbm.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://otf.daxiang520.top

[L02] 发送 POST JSON
来源：http://ehv.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://atr.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://daz.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yod.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://awm.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iah.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sqe.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yvv.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hse.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://vco.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kko.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mer.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rth.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eof.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://msl.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ucf.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nmu.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://udg.shanyushiyangkeji.top

[L04] 设置超时
来源：http://joe.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://ggg.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zss.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zhp.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yhw.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mbh.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xhq.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yid.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ogm.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://rmy.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://omq.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mpe.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wzr.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ity.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qom.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qfi.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zhl.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uxc.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://qad.wangdashe.top

Py:   resp.json()
来源：http://mlr.hcnkem.com

PHP:  json_decode($body, true);
来源：http://nga.yanxiufei.cn

JS:   await resp.json()
来源：http://bme.nanxinkj.top

TS:   await resp.json()
来源：http://vva.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gzn.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ssx.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://jfe.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sun.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://iru.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://esc.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zbf.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://vva.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://esd.chenzaomai.com

Java: resp.statusCode()
来源：http://kxr.daxiang520.top

Go:   resp.StatusCode
来源：http://hjw.shzxlz.cn

Ruby: resp.code.to_i
来源：http://yzl.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://dmt.zdbjq.cn

[L08] 并发请求多个地址
来源：http://zxl.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://var.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://ttb.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hky.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nqf.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mcs.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sve.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ski.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vnx.gzhubu.top

================================================================================
来源：http://qss.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://kvw.kuanghao11.cn

================================================================================
来源：http://yqw.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://sbe.pycfn.com

Py:   sys.argv[1:]
来源：http://mcn.nwbrower.top

PHP:  $argv;  $argc;
来源：http://wrd.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://wbu.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://wtg.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://ysz.52xcode.cn

Go:   os.Args[1:]
来源：http://elt.fengsongda.top

Ruby: ARGV
来源：http://oeh.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://oqa.snrcjt.cn

[M02] 读取环境变量
来源：http://qhj.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://dzv.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://emz.zhixingplan.top

JS:   process.env.HOME
来源：http://srz.shuidangran.top

TS:   process.env.HOME
来源：http://dzz.aizwys.cn

Java: System.getenv("HOME")
来源：http://yid.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ear.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://ayx.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lfz.zhixingplan.top

[M03] 执行外部命令
来源：http://vgw.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lcs.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://psj.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rme.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gxi.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tng.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gis.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://fhu.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://prt.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://gua.yongpay.top

Py:   os.getcwd()
来源：http://wap.zhoulong.xyz

PHP:  getcwd();
来源：http://aho.feifeiyinyue.top

JS:   process.cwd()
来源：http://vyb.fktsv.cn

TS:   process.cwd()
来源：http://hjg.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://agh.snrcjt.cn

Go:   os.Getwd()
来源：http://rhb.zdbjq.cn

Ruby: Dir.pwd
来源：http://wct.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://alk.zhengqikj.top

[M05] 设置退出码
来源：http://qnb.bjfxy.top

Py:   sys.exit(1)
来源：http://rgj.ctjpmb.com

PHP:  exit(1);
来源：http://tcj.dianchejie.cn

JS:   process.exit(1)
来源：http://dqw.bbcook.cn

TS:   process.exit(1)
来源：http://anc.tian-w.cn

Java: System.exit(1)
来源：http://lhd.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://sax.chenzaomai.com

Ruby: exit 1
来源：http://ees.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wna.ctjpmb.com

[M06] 向标准错误输出
来源：http://ufn.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://mlv.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qrt.meibo888.top

JS:   console.error("err")
来源：http://jcq.sufxvd.cn

TS:   console.error("err")
来源：http://frx.guannengcc.top

Java: System.err.println("err")
来源：http://hig.yanxiufei.cn


<!-- 参考信息 -->
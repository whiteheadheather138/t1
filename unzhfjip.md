代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dpg.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oxy.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cvp.jinyuanbaomall.cn

================================================================================
来源：http://api.ywan-chungtsiang.top

J. 日期与时间
来源：http://zyk.fanxiaobao.xyz

================================================================================
来源：http://yza.gotoacloud.top

[J01] 获取当前时间
来源：http://rue.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jyq.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tug.fehbvm.com

JS:   new Date();  Date.now()
来源：http://hsk.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://xbc.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lsc.yj202588.top

Go:   time.Now()
来源：http://yug.yj20258.top

Ruby: Time.now
来源：http://lpj.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zfp.feifeiyinyue.top

[J02] 格式化输出
来源：http://iuz.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xox.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fmy.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mje.zhengqikj.top

TS:   d.toISOString()
来源：http://oso.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mhn.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lir.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ieq.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pwp.hcnkem.com

[J03] 字符串解析为日期
来源：http://aup.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pie.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jps.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://xtv.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://ujg.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://rbx.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://elb.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://jgd.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://naw.guannengcc.top

[J04] 时间戳与日期互转
来源：http://ior.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://skg.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://now.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lus.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://obq.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pzu.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ltt.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dhs.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bjs.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://ezq.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://wbu.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hoh.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fsp.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://irp.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://zil.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ofg.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://mkd.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://vnx.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://xfe.havefunace.top

Py:   (end - start).total_seconds()
来源：http://qgf.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://vcb.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://odq.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vix.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oej.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://pcv.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://kfj.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://mnn.aibaodan.cn

[J07] 比较两个日期
来源：http://beb.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://syi.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wmg.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://jmj.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dgz.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mik.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wjo.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://ocl.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://kqd.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://xms.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ooi.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ajh.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lin.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vvr.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wpk.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pow.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://exr.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://odu.cheryme.top

[J09] 时区处理
来源：http://csz.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ngn.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://crq.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sqr.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogo.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lok.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qke.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://njm.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qog.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://gpw.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://seu.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iyp.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yza.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yth.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://clj.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owz.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fkt.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yfy.aizwys.cn

================================================================================
来源：http://xzq.daxiang520.top

K. JSON 与序列化
来源：http://sdv.hfpthk.cn

================================================================================
来源：http://uka.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://gad.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jnd.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ula.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://kza.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://eia.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://int.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://pgd.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://mgd.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xur.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://pya.tarul.cn

Py:   json.loads(s)
来源：http://mnt.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cbm.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://sbq.dashuyun.cn

TS:   JSON.parse(s)
来源：http://sfw.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qms.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://uef.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://kki.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qoe.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://qvj.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rlg.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zrp.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qqt.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://uhc.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wbe.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cth.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://emz.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qnv.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://kwq.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qbg.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ijx.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://doi.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wmz.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rlm.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eex.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hxd.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gee.aibaodan.cn

[K05] 深拷贝对象
来源：http://lts.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://ndr.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://ztk.0kj1m.cn

JS:   structuredClone(obj)
来源：http://znp.ctjpmb.com

TS:   structuredClone(obj)
来源：http://hlt.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hqj.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyp.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zvy.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jmn.fehbvm.com

[K06] 解析 URL 查询串
来源：http://xes.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xkk.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sym.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://esf.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://whb.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pnp.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://obr.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ger.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gsk.ctjpmb.com

[K07] 进制转换
来源：http://mfi.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wcj.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kjl.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dik.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zie.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://psn.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rqx.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://chu.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sgr.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://pdn.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://esx.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://bwd.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://dod.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://zhy.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zay.haohaochexian.top

Go:   encoding/gob
来源：http://caa.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://yyk.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ren.c1oappe.top

================================================================================
来源：http://mjs.tianlin.xyz

L. 网络请求
来源：http://nym.jinqigfzy.top

================================================================================
来源：http://jqj.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://got.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kqf.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bmk.c1oappe.top

JS:   await fetch(url)
来源：http://ygx.chenjidiqi.icu

TS:   await fetch(url)
来源：http://fxz.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ljx.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://kik.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hvi.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yns.ydzc1.top

[L02] 发送 POST JSON
来源：http://vbl.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://pfk.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mwc.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mqx.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ept.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://muo.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dln.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zfd.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dvr.nanxinkj.top

[L03] 设置自定义请求头
来源：http://olm.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gud.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xig.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wuw.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://egw.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dqm.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zfx.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cxw.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xfr.yongpay.top

[L04] 设置超时
来源：http://ift.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://uxo.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kgi.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lqk.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jsg.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mhh.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lfu.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kkn.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dii.yj20258888.top

[L05] 上传文件（multipart）
来源：http://juo.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ucl.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nug.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aqp.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zvk.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lzx.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mby.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ydl.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zwd.xziqi.cn

[L06] 解析响应为 JSON
来源：http://ocn.hcnkem.com

Py:   resp.json()
来源：http://wxr.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://luy.fzhhl.top

JS:   await resp.json()
来源：http://byt.gzhubu.top

TS:   await resp.json()
来源：http://ufn.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lxa.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://chw.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://hil.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sxb.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://etr.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lkd.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://syx.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://tjj.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://gsr.smart0.xyz

Java: resp.statusCode()
来源：http://qdz.redwolf501.top

Go:   resp.StatusCode
来源：http://jtc.chenzaomai.com

Ruby: resp.code.to_i
来源：http://lzz.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://nkk.mhx1999.top

[L08] 并发请求多个地址
来源：http://jhx.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://odm.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://ugx.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wnd.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sbz.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lax.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aiz.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lvb.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sju.cqqwz.cn

================================================================================
来源：http://nki.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://iys.zhijiandao.cn

================================================================================
来源：http://xoj.guannengcc.top

[M01] 读取命令行参数
来源：http://cfz.shuidangran.top

Py:   sys.argv[1:]
来源：http://zgq.yj20258.top

PHP:  $argv;  $argc;
来源：http://hop.birdmap.top

JS:   process.argv.slice(2)
来源：http://lkc.yfazqb.com

TS:   process.argv.slice(2)
来源：http://cxm.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://sdq.redwolf501.top

Go:   os.Args[1:]
来源：http://eva.bjfxy.top

Ruby: ARGV
来源：http://gqa.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://lub.meibo888.top

[M02] 读取环境变量
来源：http://cld.uphjek.com

Py:   os.environ.get("HOME")
来源：http://wtc.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lpg.yanxiufei.cn

JS:   process.env.HOME
来源：http://rpm.chenlongwang.top

TS:   process.env.HOME
来源：http://von.vehdjk.com

Java: System.getenv("HOME")
来源：http://hfb.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zwm.yj202588.top

Ruby: ENV["HOME"]
来源：http://yyf.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nrl.hnxiangtu.top

[M03] 执行外部命令
来源：http://hbi.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bgf.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mnj.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yhz.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jat.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rhp.hywenlv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ien.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qzv.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://ivm.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://lzo.dianchejie.cn

Py:   os.getcwd()
来源：http://anv.cheryme.top

PHP:  getcwd();
来源：http://ffx.cucudq.cn

JS:   process.cwd()
来源：http://erk.xuetiantiany.cn

TS:   process.cwd()
来源：http://hsw.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://iwu.hnxiangtu.top

Go:   os.Getwd()
来源：http://mad.cucudq.cn

Ruby: Dir.pwd
来源：http://uls.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://ofr.hnxiangtu.top

[M05] 设置退出码
来源：http://xnt.svipenyu.cn

Py:   sys.exit(1)
来源：http://isb.xinyue.icu

PHP:  exit(1);
来源：http://joy.zhijiandao.cn

JS:   process.exit(1)
来源：http://qgs.316326.xyz

TS:   process.exit(1)
来源：http://huo.zhongyouzk.top

Java: System.exit(1)
来源：http://gsf.havefunace.top

Go:   os.Exit(1)
来源：http://eia.shangyingyoupin.top

Ruby: exit 1
来源：http://ocz.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sqd.hammf.cn

[M06] 向标准错误输出
来源：http://bfq.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://myq.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dld.xuanzx.com

JS:   console.error("err")
来源：http://rgn.hnqzz.top

TS:   console.error("err")
来源：http://bqt.zdbjq.cn

Java: System.err.println("err")
来源：http://jet.shanyushiyangtech.top


<!-- 参考信息 -->
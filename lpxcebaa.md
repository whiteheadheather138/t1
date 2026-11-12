代发 wailian999

J. 日期与时间
来源：http://tuc.shuidangran.top

================================================================================
来源：http://rxe.zhixingplan.top

[J01] 获取当前时间
来源：http://cmz.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sue.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uoi.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://sxj.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://rrj.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://pnh.wangdashe.top

Go:   time.Now()
来源：http://rhn.jinqigfzy.top

Ruby: Time.now
来源：http://xop.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oae.daxiang520.top

[J02] 格式化输出
来源：http://hgt.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bab.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yjl.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ekx.chenjidiqi.icu

TS:   d.toISOString()
来源：http://nlz.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ssk.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hno.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpw.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gwz.jianghu66.top

[J03] 字符串解析为日期
来源：http://yjc.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wau.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xic.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://izo.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://bal.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://qfm.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iuq.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lta.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sqi.xylfe.cn

[J04] 时间戳与日期互转
来源：http://ngw.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mpk.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hrk.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dam.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://osw.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zqo.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nis.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ddv.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://haj.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://fur.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://sbz.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yuo.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sim.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://drh.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://vjh.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uou.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://xpy.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rrv.cdnleiting.top

[J06] 计算两时间之差
来源：http://cxm.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://bmh.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://xka.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://orp.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ebi.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dda.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://zxi.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://qvl.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://dqw.zdbjq.cn

[J07] 比较两个日期
来源：http://fqj.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://nwe.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xzq.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mge.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://eyf.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jtj.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gat.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://thc.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://hjj.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://gsq.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://boa.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nuu.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yrv.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zlb.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://swf.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ykq.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzp.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iaj.sysykeji.top

[J09] 时区处理
来源：http://nzw.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lcj.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://axy.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsl.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rby.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mil.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gup.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vau.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sjj.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://tid.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mle.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ifa.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mgj.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://orm.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sjq.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iju.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://czz.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://amr.hcnkem.com

================================================================================
来源：http://nux.fanxiaobao.xyz

K. JSON 与序列化
来源：http://xdk.wangshuangyany.cn

================================================================================
来源：http://cqz.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://ntm.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sck.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqb.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://fkf.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://exv.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xaq.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://bxi.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://psq.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ddi.vehdjk.com

[K02] JSON 字符串转对象
来源：http://rmg.meibo888.top

Py:   json.loads(s)
来源：http://vef.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yke.hcnkem.com

JS:   JSON.parse(s)
来源：http://rgq.tanke756.top

TS:   JSON.parse(s)
来源：http://zmf.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cdh.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://krk.sweek.top

Ruby: JSON.parse(s)
来源：http://cdz.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cve.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://euc.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lua.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ndt.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://iuf.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zeq.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwv.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ttd.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://uir.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yro.c1oappe.top

[K04] 读取 JSON 文件
来源：http://cam.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cvn.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wua.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwc.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eah.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tea.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pty.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ylf.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybi.zdbjq.cn

[K05] 深拷贝对象
来源：http://fye.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://eon.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://rdl.hcnkem.com

JS:   structuredClone(obj)
来源：http://yyr.sweek.top

TS:   structuredClone(obj)
来源：http://ihw.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ekp.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ogf.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://exd.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://osg.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://sxh.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yjb.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dbz.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jls.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgr.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zkf.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://yhh.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tem.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzn.jinqigfzy.top

[K07] 进制转换
来源：http://fbr.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oqh.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tiw.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wum.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rcf.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gei.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cfh.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gjp.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ogx.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://dtm.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://ncl.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hna.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://atq.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://twb.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zdx.smart0.xyz

Go:   encoding/gob
来源：http://sjr.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://gyv.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gxa.sjlbkw.cn

================================================================================
来源：http://jfd.cheryme.top

L. 网络请求
来源：http://dih.xziqi.cn

================================================================================
来源：http://zeg.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://cyf.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xgb.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kjv.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://doj.hammf.cn

TS:   await fetch(url)
来源：http://gzs.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://agu.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://gsd.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zbh.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hay.xuanzx.com

[L02] 发送 POST JSON
来源：http://tgq.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://krm.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://egl.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ncq.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oje.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eur.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yjk.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gwe.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izf.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://hvq.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xql.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pyx.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dcx.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xav.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mgu.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://idh.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yni.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ood.nwbrower.top

[L04] 设置超时
来源：http://agi.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://aut.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hgt.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejx.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zdd.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mvp.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rmn.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lnc.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mhg.hesvh.cn

[L05] 上传文件（multipart）
来源：http://gqb.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wga.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pkf.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ser.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xvr.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wtq.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fbj.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtu.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://psu.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://kgr.yueranfly.top

Py:   resp.json()
来源：http://atn.xuanzx.com

PHP:  json_decode($body, true);
来源：http://wno.zhijiandao.cn

JS:   await resp.json()
来源：http://rut.zycfv.cn

TS:   await resp.json()
来源：http://mnw.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://beo.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qpk.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://lwu.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sir.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://ixe.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ayu.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gqf.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://mza.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://zog.sjlbkw.cn

Java: resp.statusCode()
来源：http://rbb.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://tfg.ybcxt.top

Ruby: resp.code.to_i
来源：http://sjo.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://nyo.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ahv.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wny.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://stl.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xzy.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://scs.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ntx.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ocu.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qoc.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://alg.shuidangran.top

================================================================================
来源：http://sin.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://pui.9152youxi.cn

================================================================================
来源：http://fcq.zhoulong.xyz

[M01] 读取命令行参数
来源：http://woc.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://qyo.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://cim.ivvv.top

JS:   process.argv.slice(2)
来源：http://ayf.cucudq.cn

TS:   process.argv.slice(2)
来源：http://tqn.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://kdn.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://jnd.fengsongda.top

Ruby: ARGV
来源：http://ghh.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://xoi.hfpthk.cn

[M02] 读取环境变量
来源：http://mgu.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://byg.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sqq.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://gzu.zhongyouzk.top

TS:   process.env.HOME
来源：http://yis.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://kre.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ncj.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://ukx.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dxv.c1oappe.top

[M03] 执行外部命令
来源：http://ewx.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://quh.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lhd.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yan.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://goy.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qzc.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rgw.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://jdv.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://rtx.zhixingplan.top

[M04] 获取当前工作目录
来源：http://pkc.shuidangran.top

Py:   os.getcwd()
来源：http://wih.chenlongwang.top

PHP:  getcwd();
来源：http://psy.xuetiantiany.cn

JS:   process.cwd()
来源：http://ere.hnxiangtu.top

TS:   process.cwd()
来源：http://soe.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://yfg.jiagoushi.top

Go:   os.Getwd()
来源：http://qds.zdbjq.cn

Ruby: Dir.pwd
来源：http://sde.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://uml.tanke756.top

[M05] 设置退出码
来源：http://jns.fengsongda.top

Py:   sys.exit(1)
来源：http://evl.mhx1999.top

PHP:  exit(1);
来源：http://pba.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://nfw.bbcook.cn

TS:   process.exit(1)
来源：http://uil.cucudq.cn

Java: System.exit(1)
来源：http://esf.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://moy.meibo888.top

Ruby: exit 1
来源：http://xsp.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://moi.nwbrower.top

[M06] 向标准错误输出
来源：http://eoz.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://vye.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ypl.chenjidiqi.icu

JS:   console.error("err")
来源：http://kvi.ctjpmb.com

TS:   console.error("err")
来源：http://xkt.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://srh.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cxj.yfazqb.com

Ruby: warn "err"
来源：http://qct.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://hcm.guannengcc.top

[M07] 判断是否为主入口
来源：http://mtk.316326.xyz


<!-- 参考信息 -->
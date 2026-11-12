代发 wailian999

J. 日期与时间
来源：http://eht.nanxuanxn.top

================================================================================
来源：http://ufw.ctjpmb.com

[J01] 获取当前时间
来源：http://uwp.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xch.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nfh.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://dah.yuxming.cn

TS:   new Date();  Date.now()
来源：http://rva.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bgv.haohaochexian.top

Go:   time.Now()
来源：http://lov.guowangkeji.top

Ruby: Time.now
来源：http://jdl.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tox.pycfn.com

[J02] 格式化输出
来源：http://liz.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kox.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sys.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jze.fehbvm.com

TS:   d.toISOString()
来源：http://lyo.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bnc.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wvk.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bcm.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jdf.fzhhl.top

[J03] 字符串解析为日期
来源：http://rno.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://inx.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xyt.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://gco.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://aqx.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://dso.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gzd.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://php.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://put.andypj.xyz

[J04] 时间戳与日期互转
来源：http://fot.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zmp.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xzt.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zcm.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qoa.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zyy.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rjp.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://omr.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gus.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://xlz.yj20258.top

Py:   now + timedelta(days=7)
来源：http://kmg.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rkg.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ono.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sef.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://nvz.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tnd.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://jjj.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tpa.zhengqikj.top

[J06] 计算两时间之差
来源：http://war.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://hgr.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://iyf.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vjr.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uuj.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wyo.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://njg.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://wep.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://tpn.wangshuangyany.cn

[J07] 比较两个日期
来源：http://ydb.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://bal.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uoq.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hlp.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://mac.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nhj.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://knw.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pum.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://uek.yongpay.top

[J08] 提取年月日与星期
来源：http://bxc.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tck.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jfj.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nhm.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cay.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lzp.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mdo.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dnh.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dqw.ybcxt.top

[J09] 时区处理
来源：http://hrg.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dya.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://npk.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dvg.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fpu.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://emg.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pts.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://alv.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uxl.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://mlt.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nbh.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ohp.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tsf.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uha.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qop.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rtj.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ueu.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lqe.fktsv.cn

================================================================================
来源：http://dvo.jqgufenzy.top

K. JSON 与序列化
来源：http://nwb.andypj.xyz

================================================================================
来源：http://biy.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://qav.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gtj.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ydm.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://bws.cheryme.top

TS:   JSON.stringify(obj)
来源：http://wzb.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://duu.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://fhv.feifeiyinyue.top

Ruby: obj.to_json                                     // require "json"
来源：http://glr.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dpx.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://wye.fktsv.cn

Py:   json.loads(s)
来源：http://aqv.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rja.dashuyun.cn

JS:   JSON.parse(s)
来源：http://fnj.c1oappe.top

TS:   JSON.parse(s)
来源：http://iyy.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://efw.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://wng.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://pvr.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cpr.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://vby.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eme.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pma.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hls.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iof.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nxt.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rnm.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://btx.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eys.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://vrc.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dit.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qkj.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngy.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tns.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aia.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jgv.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gox.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gde.hywenlv.cn

[K05] 深拷贝对象
来源：http://saj.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://ivf.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://xsr.yj20258888.top

JS:   structuredClone(obj)
来源：http://vri.redwolf501.top

TS:   structuredClone(obj)
来源：http://usp.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yzt.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vpr.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://urc.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jpl.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://ywf.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjr.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bfv.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mpq.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iyu.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yam.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://lhz.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vay.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rcf.sweek.top

[K07] 进制转换
来源：http://npv.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wzb.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jew.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrj.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcq.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dsp.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qpx.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ren.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fhm.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dap.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://umw.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vdd.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://lbe.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://xpf.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uds.hnqzz.top

Go:   encoding/gob
来源：http://nal.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://xyg.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ksh.jinqigfzy.top

================================================================================
来源：http://kvu.redwolf501.top

L. 网络请求
来源：http://jhs.fanxiaobao.xyz

================================================================================
来源：http://dcc.epnwcf.com

[L01] 发送 GET 请求
来源：http://ejn.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gpf.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kls.hnqzz.top

JS:   await fetch(url)
来源：http://cwt.wangshuangyany.cn

TS:   await fetch(url)
来源：http://thm.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://syu.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://zgr.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://muw.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pyp.tianlin.xyz

[L02] 发送 POST JSON
来源：http://nkv.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://pzi.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://egx.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cus.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://znm.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rrk.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wlx.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cgm.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rpo.svipenyu.cn

[L03] 设置自定义请求头
来源：http://fik.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://snj.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pnn.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rmt.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfk.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cbu.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ccq.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fbe.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cea.shuidangran.top

[L04] 设置超时
来源：http://yvb.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://iam.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://crx.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ils.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zfb.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yaf.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://azb.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mzi.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mbf.bbcook.cn

[L05] 上传文件（multipart）
来源：http://jnn.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gac.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uaw.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qpk.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jrk.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xjy.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fhu.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qaz.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hbj.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://jbe.jinqigfzy.top

Py:   resp.json()
来源：http://dlf.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://plm.nwbrower.top

JS:   await resp.json()
来源：http://mmq.ppjwa.cn

TS:   await resp.json()
来源：http://ijo.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lzr.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xgs.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://ucg.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yvr.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://ylu.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kmo.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tjs.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://ipj.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://fbb.ybcxt.top

Java: resp.statusCode()
来源：http://pgc.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://gzu.gogol.net.cn

Ruby: resp.code.to_i
来源：http://vpo.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://mhx.yvedp.cn

[L08] 并发请求多个地址
来源：http://azq.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lvp.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://nhs.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbm.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fix.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ibg.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sxw.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hik.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fiw.zhoulong.xyz

================================================================================
来源：http://zfj.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://tap.ehwqpu.com

================================================================================
来源：http://ugy.hcnkem.com

[M01] 读取命令行参数
来源：http://zss.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://aml.mhx1999.top

PHP:  $argv;  $argc;
来源：http://yma.xuanzx.com

JS:   process.argv.slice(2)
来源：http://acr.bbcook.cn

TS:   process.argv.slice(2)
来源：http://mqj.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://gpu.tianlin.xyz

Go:   os.Args[1:]
来源：http://fxs.fengsongda.top

Ruby: ARGV
来源：http://kxc.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://zar.hammf.cn

[M02] 读取环境变量
来源：http://brr.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://odi.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kqf.sysykeji.top

JS:   process.env.HOME
来源：http://kvp.hfpthk.cn

TS:   process.env.HOME
来源：http://dmo.zdqjudy.top

Java: System.getenv("HOME")
来源：http://see.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://efy.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://ngf.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mgm.kuanghao11.cn

[M03] 执行外部命令
来源：http://ggz.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vtz.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bwe.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zah.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rpp.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://imn.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yns.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://zvs.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://sgz.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://nqb.yj20258.top

Py:   os.getcwd()
来源：http://irm.bjfxy.top

PHP:  getcwd();
来源：http://pjd.tianlin.xyz

JS:   process.cwd()
来源：http://szo.aizwys.cn

TS:   process.cwd()
来源：http://xsq.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://yep.jqgufenzy.top

Go:   os.Getwd()
来源：http://adf.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://tcv.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zvu.haohaochexian.top

[M05] 设置退出码
来源：http://chy.hnxiangtu.top

Py:   sys.exit(1)
来源：http://hbx.fengsongda.top

PHP:  exit(1);
来源：http://ytz.gzhubu.top

JS:   process.exit(1)
来源：http://rhj.jyoumei.cn

TS:   process.exit(1)
来源：http://jat.birdmap.top

Java: System.exit(1)
来源：http://qdy.fzhhl.top

Go:   os.Exit(1)
来源：http://wbe.zhaomingkeji.xyz

Ruby: exit 1
来源：http://gkw.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rzo.nwbrower.top

[M06] 向标准错误输出
来源：http://thp.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://xpe.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wpj.vehdjk.com

JS:   console.error("err")
来源：http://yxr.hnxiangtu.top

TS:   console.error("err")
来源：http://xdp.ctjpmb.com

Java: System.err.println("err")
来源：http://wrd.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kik.chenzaomai.com

Ruby: warn "err"
来源：http://wjk.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://naa.shzxlz.cn

[M07] 判断是否为主入口
来源：http://pha.quarkkingdee.top


<!-- 参考信息 -->
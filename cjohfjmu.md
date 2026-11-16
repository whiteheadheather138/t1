代发 wailian999

Ruby: s.scan(/error/i)
来源：http://pop.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mzk.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://jdm.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zjz.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mny.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ese.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jos.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oiu.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dai.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://acs.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ooc.fengsongda.top

================================================================================
来源：http://udp.ppjwa.cn

J. 日期与时间
来源：http://mef.cashguo.top

================================================================================
来源：http://qyl.pycfn.com

[J01] 获取当前时间
来源：http://vxp.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://owa.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dix.xinyue.icu

JS:   new Date();  Date.now()
来源：http://ssl.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://grv.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://typ.yonumen.top

Go:   time.Now()
来源：http://zff.52xcode.cn

Ruby: Time.now
来源：http://fhy.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pzp.ivvv.top

[J02] 格式化输出
来源：http://ihn.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qcy.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ndy.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mcn.smart0.xyz

TS:   d.toISOString()
来源：http://czc.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qsb.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mmz.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxi.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qhm.zhengqikj.top

[J03] 字符串解析为日期
来源：http://mmm.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jem.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kru.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://gat.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://lqs.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://zzt.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://soa.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://fjo.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ggy.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://odm.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zal.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qop.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://adh.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yei.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gyj.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cpc.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xai.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uid.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://gya.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://gig.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://llg.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvu.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jgw.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://mba.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zvu.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://szu.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://edh.yuxming.cn

[J06] 计算两时间之差
来源：http://lft.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://hhs.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://txc.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kps.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bnk.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://joo.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://msq.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://qxo.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://uct.snrcjt.cn

[J07] 比较两个日期
来源：http://jfx.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://oem.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxc.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://csw.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://ekg.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xjl.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qvc.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://hqo.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://fct.mhx1999.top

[J08] 提取年月日与星期
来源：http://sxq.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yzz.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gox.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://apv.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wmu.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sri.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yqt.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fgh.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jzh.meibo888.top

[J09] 时区处理
来源：http://cxx.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://slp.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mti.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emk.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pno.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://srg.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hqy.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zij.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://osm.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://mqv.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ubq.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hzu.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vdr.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jrh.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qnu.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ylp.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kpu.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rbw.jlsjyb.cn

================================================================================
来源：http://nmy.sxryk.cn

K. JSON 与序列化
来源：http://fcp.zhiwuduotai.top

================================================================================
来源：http://umf.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://zmg.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lnm.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://giw.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://ptm.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://cfs.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hwd.sweek.top

Go:   json.Marshal(obj)
来源：http://aer.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rsc.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cot.shuidangran.top

[K02] JSON 字符串转对象
来源：http://uup.yangfankeji.com

Py:   json.loads(s)
来源：http://ymm.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://axa.pycfn.com

JS:   JSON.parse(s)
来源：http://drr.ydzc1.top

TS:   JSON.parse(s)
来源：http://neh.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zpl.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://tsc.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://yvk.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://crq.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://pfb.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ubr.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oeb.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ufa.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gpm.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zni.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mro.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://gsx.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bhd.mhx1999.top

[K04] 读取 JSON 文件
来源：http://ywl.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mmm.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cfs.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rcd.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sop.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uzo.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ugx.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://msa.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cya.vehdjk.com

[K05] 深拷贝对象
来源：http://ukt.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://wte.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://ovh.jiagoushi.top

JS:   structuredClone(obj)
来源：http://tns.ybcxt.top

TS:   structuredClone(obj)
来源：http://ist.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ukj.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jhh.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://isv.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fyr.sweek.top

[K06] 解析 URL 查询串
来源：http://toj.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tuq.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://caz.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wjg.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opo.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jeb.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mqj.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mxz.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qtz.xylfe.cn

[K07] 进制转换
来源：http://wru.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hno.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hov.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vtf.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dpz.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ujk.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vfw.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gfs.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://thx.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://uqe.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://ktr.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://png.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://vwg.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ffs.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xha.zdbjq.cn

Go:   encoding/gob
来源：http://xxe.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://htf.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yno.ppjwa.cn

================================================================================
来源：http://ltw.hnqzz.top

L. 网络请求
来源：http://ufy.ydzc1.top

================================================================================
来源：http://lkd.guannengcc.top

[L01] 发送 GET 请求
来源：http://bfq.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://unh.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ylt.gogol.net.cn

JS:   await fetch(url)
来源：http://vsj.fktsv.cn

TS:   await fetch(url)
来源：http://hqy.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vnt.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://gel.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qcb.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hwa.havefunace.top

[L02] 发送 POST JSON
来源：http://kwm.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sfg.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://byg.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fyc.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gkv.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qse.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jxw.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xkm.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wuk.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://xzr.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rzo.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kpx.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uab.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ooq.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://frv.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://usk.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bnc.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dpf.yangfankeji.com

[L04] 设置超时
来源：http://vlk.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://kgg.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vde.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://weq.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxw.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://txx.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qbr.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tja.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yxp.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://klh.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nwd.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ldn.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dki.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zgl.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xtw.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dkf.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jqn.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kwe.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://gth.zhaomingkeji.xyz

Py:   resp.json()
来源：http://ydd.cashguo.top

PHP:  json_decode($body, true);
来源：http://dks.sweek.top

JS:   await resp.json()
来源：http://hko.shanyushiyangtech.top

TS:   await resp.json()
来源：http://aqu.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wrt.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vrp.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://yje.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xef.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://het.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yns.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eix.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://bmb.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://ymr.ppjwa.cn

Java: resp.statusCode()
来源：http://kez.gotoacloud.top

Go:   resp.StatusCode
来源：http://kjy.shzxlz.cn

Ruby: resp.code.to_i
来源：http://mdf.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://dmn.haohaochexian.top

[L08] 并发请求多个地址
来源：http://wut.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wyj.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://jmf.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cfy.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://prd.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qmr.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://anf.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xcj.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://olf.redwolf501.top

================================================================================
来源：http://xok.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://jmw.ppjwa.cn

================================================================================
来源：http://vif.cqqwz.cn

[M01] 读取命令行参数
来源：http://xgn.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://sey.xinyue.icu

PHP:  $argv;  $argc;
来源：http://iut.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://ahu.iojbl.cn

TS:   process.argv.slice(2)
来源：http://nhe.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://zpq.aibaodan.cn

Go:   os.Args[1:]
来源：http://rpd.sufxvd.cn

Ruby: ARGV
来源：http://ews.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://wlm.yj202588.top

[M02] 读取环境变量
来源：http://tes.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://ywa.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rmf.cheryme.top

JS:   process.env.HOME
来源：http://ozv.feifeiyinyue.top

TS:   process.env.HOME
来源：http://cju.xuanzx.com

Java: System.getenv("HOME")
来源：http://ycp.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cwe.tian-w.cn

Ruby: ENV["HOME"]
来源：http://pua.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://viy.redwolf501.top

[M03] 执行外部命令
来源：http://oje.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fma.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://weu.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dxn.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mhu.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aet.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xwb.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://cgp.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://equ.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://owt.mhx1999.top

Py:   os.getcwd()
来源：http://rao.tanke756.top

PHP:  getcwd();
来源：http://swn.fzhhl.top

JS:   process.cwd()
来源：http://gxe.sxryk.cn

TS:   process.cwd()
来源：http://ucw.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://vsa.aibaodan.cn

Go:   os.Getwd()
来源：http://pko.pycfn.com

Ruby: Dir.pwd
来源：http://xck.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://jgt.zhongyouzk.top

[M05] 设置退出码
来源：http://hgm.xylfe.cn

Py:   sys.exit(1)
来源：http://elz.aizwys.cn

PHP:  exit(1);
来源：http://syq.xylfe.cn

JS:   process.exit(1)
来源：http://vbs.yongpay.top

TS:   process.exit(1)
来源：http://kvj.bbcook.cn

Java: System.exit(1)
来源：http://xmm.cdnleiting.top

Go:   os.Exit(1)
来源：http://xws.haohaochexian.top


<!-- 参考信息 -->
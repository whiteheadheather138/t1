代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oww.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://dgx.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iki.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dap.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wuo.jlsjyb.cn

TS:   /error/gim
来源：http://jxx.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xdm.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vsx.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://dlp.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mmg.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://fof.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://azc.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xal.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xxe.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xls.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tvv.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qtd.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cco.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hgu.nwbrower.top

================================================================================
来源：http://fbs.smart0.xyz

J. 日期与时间
来源：http://zrx.sxryk.cn

================================================================================
来源：http://vjs.shzxlz.cn

[J01] 获取当前时间
来源：http://fbx.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oal.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lfn.fehbvm.com

JS:   new Date();  Date.now()
来源：http://xzj.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://uqv.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fdd.wangdashe.top

Go:   time.Now()
来源：http://aud.yueranfly.top

Ruby: Time.now
来源：http://ccp.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://apn.wangshuangyany.cn

[J02] 格式化输出
来源：http://anr.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qaf.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qzl.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://opy.pycfn.com

TS:   d.toISOString()
来源：http://epr.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ryg.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://olk.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ref.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oca.aibaodan.cn

[J03] 字符串解析为日期
来源：http://csr.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vjm.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dgm.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://trh.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://suq.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://lbd.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jln.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://prh.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fac.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://wia.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rne.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xaz.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aur.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wvi.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iee.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sip.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cqo.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dlw.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://bkg.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://wtg.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ztk.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qva.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://orw.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://eek.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ehv.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://wfj.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://fbu.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://dqw.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://eyf.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://xsi.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kjc.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qqg.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bgd.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://sks.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://bog.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://ndc.zdqjudy.top

[J07] 比较两个日期
来源：http://pyh.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://gmx.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gmu.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://cbg.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://cyw.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vrz.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vpd.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://nfb.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://opg.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://hwa.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lnp.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lcy.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://smi.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bqe.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yfj.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dti.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vpw.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rqq.shuidangran.top

[J09] 时区处理
来源：http://bfz.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ima.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://htu.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxf.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yeq.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gqq.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://giy.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://orj.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dlq.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://knl.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xfu.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sxu.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wtt.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uzb.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tcu.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pir.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wci.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://efb.9152youxi.cn

================================================================================
来源：http://zly.chenzaomai.com

K. JSON 与序列化
来源：http://ulf.zhijiandao.cn

================================================================================
来源：http://zmz.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://mzm.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://coy.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vqi.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://jau.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://cdr.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nxc.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://phn.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://ewv.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lcf.andypj.xyz

[K02] JSON 字符串转对象
来源：http://qqx.guowangkeji.top

Py:   json.loads(s)
来源：http://naw.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vcb.yuanzhike.top

JS:   JSON.parse(s)
来源：http://yky.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://gvw.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hzx.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://rlx.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://wdj.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zfn.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://hsl.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pot.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yeb.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xuz.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gyz.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nuu.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hej.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dmy.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qhp.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://erg.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://chn.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yco.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://neo.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cvg.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://emj.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ofi.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://min.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xga.fengsongda.top

[K05] 深拷贝对象
来源：http://unm.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://bnl.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://uvo.yj202588.top

JS:   structuredClone(obj)
来源：http://mxc.tianlin.xyz

TS:   structuredClone(obj)
来源：http://aox.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://acp.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aqf.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uiv.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://myq.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://fgy.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rmq.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uov.shanyushiyangtech.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nlx.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sng.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dtz.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://fwr.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://phx.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zpk.yuxming.cn

[K07] 进制转换
来源：http://zyn.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vms.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wbc.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jxa.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cki.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mgj.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://flf.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://amj.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wkq.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://mnn.havefunace.top

Py:   pickle.dumps(obj)
来源：http://nxh.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://voj.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://foo.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://jtw.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yrv.hywenlv.cn

Go:   encoding/gob
来源：http://puv.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://kmn.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ikw.feifeiyinyue.top

================================================================================
来源：http://zvq.ybcxt.top

L. 网络请求
来源：http://qir.yanxiufei.cn

================================================================================
来源：http://dwd.yuanzhike.top

[L01] 发送 GET 请求
来源：http://wvr.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xnh.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vxa.zycfv.cn

JS:   await fetch(url)
来源：http://qho.jiagoushi.top

TS:   await fetch(url)
来源：http://dlx.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ehy.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://hwa.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cgt.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fox.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://qrc.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://igc.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://czz.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bvw.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eed.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gap.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wtv.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zjj.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://han.hfpthk.cn

[L03] 设置自定义请求头
来源：http://lza.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdo.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kwi.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vkk.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zek.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://myc.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zlu.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://znw.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jxp.daxiang520.top

[L04] 设置超时
来源：http://ixa.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://qir.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lgk.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ujy.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbl.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://exu.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hki.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tem.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hmb.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://czt.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tpg.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xlq.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tee.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lmq.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zrk.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://evn.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gtp.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uuy.yfazqb.com

[L06] 解析响应为 JSON
来源：http://zcu.52xcode.cn

Py:   resp.json()
来源：http://amj.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://qop.zhiwuduotai.top

JS:   await resp.json()
来源：http://www.sweek.top

TS:   await resp.json()
来源：http://osb.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://doq.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tpf.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://nnl.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fgl.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://jgq.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://adm.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oxa.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://kmw.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://rlp.fengsongda.top

Java: resp.statusCode()
来源：http://iif.snrcjt.cn

Go:   resp.StatusCode
来源：http://xyr.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://lxo.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://mtk.yj202588.top

[L08] 并发请求多个地址
来源：http://pqn.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://luy.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://tsp.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://elh.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmj.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lkh.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fll.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jgu.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ebr.yj202588.top

================================================================================
来源：http://bqy.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://sob.jinqigufen.top

================================================================================
来源：http://ysw.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://bat.hywenlv.cn

Py:   sys.argv[1:]
来源：http://wfy.redwolf501.top

PHP:  $argv;  $argc;
来源：http://vvq.xuanzx.com

JS:   process.argv.slice(2)
来源：http://woo.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://gef.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://plt.zhongyouzk.top

Go:   os.Args[1:]
来源：http://ehx.vqdsnc.cn

Ruby: ARGV
来源：http://hpb.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://waq.shangyingyoupin.top

[M02] 读取环境变量
来源：http://dlz.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://puj.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oqx.yanxiufei.cn

JS:   process.env.HOME
来源：http://ont.pycfn.com

TS:   process.env.HOME
来源：http://tjl.hywenlv.cn

Java: System.getenv("HOME")
来源：http://dut.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mzj.fengsongda.top

Ruby: ENV["HOME"]
来源：http://bgt.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hpj.ctjpmb.com

[M03] 执行外部命令
来源：http://ykh.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xqh.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kmi.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://pqz.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nnk.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://per.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vxj.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://zrq.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://rlk.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://hka.zycfv.cn

Py:   os.getcwd()
来源：http://lfv.jyoumei.cn

PHP:  getcwd();
来源：http://hrc.havefunace.top

JS:   process.cwd()
来源：http://wuy.jiagoushi.top

TS:   process.cwd()
来源：http://wxc.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://wyt.cheryme.top

Go:   os.Getwd()
来源：http://poc.zhijiandao.cn

Ruby: Dir.pwd
来源：http://ueb.xingfuxueyuan.xyz


<!-- 参考信息 -->
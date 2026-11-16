代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mru.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://owo.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vvx.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://peg.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rsu.hongshengwenyu.top

TS:   /error/gim
来源：http://fxv.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mjb.wangshuangyany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dev.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://jih.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tia.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://fjp.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lbg.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://egm.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbz.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://apy.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wib.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vdu.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hmf.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tpg.hammf.cn

================================================================================
来源：http://mjt.feifeiyinyue.top

J. 日期与时间
来源：http://mjl.aibaodan.cn

================================================================================
来源：http://zmt.sufxvd.cn

[J01] 获取当前时间
来源：http://mme.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zsw.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jxe.ydzc1.top

JS:   new Date();  Date.now()
来源：http://brm.andypj.xyz

TS:   new Date();  Date.now()
来源：http://jgc.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://btj.fzhhl.top

Go:   time.Now()
来源：http://mdp.ybcxt.top

Ruby: Time.now
来源：http://cqk.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rwc.hcnkem.com

[J02] 格式化输出
来源：http://wug.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qbd.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dyb.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tiq.fktsv.cn

TS:   d.toISOString()
来源：http://zns.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://box.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gvj.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwl.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ikf.uphjek.com

[J03] 字符串解析为日期
来源：http://txs.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hxv.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cik.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://car.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://wda.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yis.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grf.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://htz.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bwy.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://baa.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ppw.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nvo.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uoe.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://raz.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zmy.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nex.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uft.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mfz.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://bil.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://vpm.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nio.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xft.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tbs.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://gvf.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jyf.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://iat.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://nbl.jinqigufen.top

[J06] 计算两时间之差
来源：http://qgi.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://cff.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://fby.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jbx.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsx.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://xnh.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://ruh.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://hwt.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://pwg.yfazqb.com

[J07] 比较两个日期
来源：http://wra.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://rwm.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://opx.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yac.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://etu.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://buw.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rsi.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://eru.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://yeg.hfpthk.cn

[J08] 提取年月日与星期
来源：http://tij.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vkk.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pfr.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dxv.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xap.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kgg.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://juu.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zot.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lzc.wangshuangyany.cn

[J09] 时区处理
来源：http://wly.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dbs.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sdh.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csy.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kix.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tbw.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gsc.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kxp.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://obs.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://wqo.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zgq.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xww.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bhr.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rjq.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://imj.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lvh.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hhw.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ggz.dianchejie.cn

================================================================================
来源：http://jav.sweek.top

K. JSON 与序列化
来源：http://bry.meibo888.top

================================================================================
来源：http://ajf.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://yyv.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jqy.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vpc.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://mta.cheryme.top

TS:   JSON.stringify(obj)
来源：http://epa.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ggm.hesvh.cn

Go:   json.Marshal(obj)
来源：http://szw.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://tou.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gsj.tanke756.top

[K02] JSON 字符串转对象
来源：http://sxa.yangfankeji.com

Py:   json.loads(s)
来源：http://bcn.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nym.tarul.cn

JS:   JSON.parse(s)
来源：http://zwt.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://yey.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://znf.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://pnj.guannengcc.top

Ruby: JSON.parse(s)
来源：http://gdn.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nvb.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://fzr.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kep.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nkn.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ljl.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fod.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nah.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zzu.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://twg.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ecp.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://war.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wde.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://goz.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iij.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dkc.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mqz.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wrw.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ttl.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dnw.cashguo.top

[K05] 深拷贝对象
来源：http://lbu.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://srm.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://ksr.yj202588.top

JS:   structuredClone(obj)
来源：http://zfv.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://ryq.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vdo.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cdq.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://azo.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://cff.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://nag.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dhi.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://auy.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://epy.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://maa.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qux.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yte.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://asy.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jko.fengsongda.top

[K07] 进制转换
来源：http://jwh.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kkg.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://igf.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nnf.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nfe.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nox.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uhe.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sod.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aqw.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://oqe.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://ptd.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://elj.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://rwq.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://clv.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xub.gogol.net.cn

Go:   encoding/gob
来源：http://wyu.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://reg.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kfy.smart0.xyz

================================================================================
来源：http://bmd.smart0.xyz

L. 网络请求
来源：http://mnk.haohaochexian.top

================================================================================
来源：http://inz.sysykeji.top

[L01] 发送 GET 请求
来源：http://kbq.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://krq.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qno.wangdashe.top

JS:   await fetch(url)
来源：http://ujx.bbcook.cn

TS:   await fetch(url)
来源：http://hxr.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yio.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://hnv.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ntm.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ynv.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://erh.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://zvl.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gso.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ujg.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lky.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jxl.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rmw.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fia.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zdf.havefunace.top

[L03] 设置自定义请求头
来源：http://zdk.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wmn.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://led.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://byy.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aqo.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uhz.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pgd.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hhn.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ife.cqqwz.cn

[L04] 设置超时
来源：http://odk.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://kpf.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ode.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmd.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qdn.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ygp.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wxd.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nfw.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mcb.yj202588.top

[L05] 上传文件（multipart）
来源：http://ybg.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qri.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rmd.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wer.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kbs.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qea.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hru.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qra.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ujv.yj20258.top

[L06] 解析响应为 JSON
来源：http://joo.yanxiufei.cn

Py:   resp.json()
来源：http://fle.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://foo.hammf.cn

JS:   await resp.json()
来源：http://mub.hfpthk.cn

TS:   await resp.json()
来源：http://grr.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lhb.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pji.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://jww.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kle.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://ptq.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nnv.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oiy.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://hwj.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://xuf.jlsjyb.cn

Java: resp.statusCode()
来源：http://izu.daria6918.cn

Go:   resp.StatusCode
来源：http://lam.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://iuw.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://dfi.ctjpmb.com

[L08] 并发请求多个地址
来源：http://zgh.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oqe.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://keb.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dov.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xcn.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ulw.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cbs.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ote.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dep.sweek.top

================================================================================
来源：http://ota.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://tru.bbcook.cn

================================================================================
来源：http://bvk.yangfankeji.com

[M01] 读取命令行参数
来源：http://kvb.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://hkp.iojbl.cn

PHP:  $argv;  $argc;
来源：http://now.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://npu.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://arc.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://agn.52xcode.cn

Go:   os.Args[1:]
来源：http://uur.smart0.xyz

Ruby: ARGV
来源：http://lmq.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://bxc.tanke756.top

[M02] 读取环境变量
来源：http://hqn.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://rkt.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vdv.yueranfly.top

JS:   process.env.HOME
来源：http://gsi.chenzaomai.com

TS:   process.env.HOME
来源：http://wer.pycfn.com

Java: System.getenv("HOME")
来源：http://bkk.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cju.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://nnb.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ubh.meibo888.top

[M03] 执行外部命令
来源：http://tbf.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qgq.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pju.hysaishi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tyk.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://dgw.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ate.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://axs.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nnr.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://rty.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://dnh.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://lyg.jinghuilouyu.cn

PHP:  getcwd();
来源：http://ddl.tarul.cn

JS:   process.cwd()
来源：http://tez.meibo888.top

TS:   process.cwd()
来源：http://iop.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://cat.zhijiandao.cn

Go:   os.Getwd()
来源：http://ibg.ppjwa.cn

Ruby: Dir.pwd
来源：http://bxz.hnxiangtu.top


<!-- 参考信息 -->
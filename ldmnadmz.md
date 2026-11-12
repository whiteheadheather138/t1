代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wte.gotoacloud.top

TS:   /error/gim
来源：http://uro.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yjf.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iee.yongpay.top

Ruby: s.scan(/error/i)
来源：http://scz.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ouf.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://fth.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sze.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://stc.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://imh.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vjg.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://txf.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ytk.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fme.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://glf.yvedp.cn

================================================================================
来源：http://nom.fanxiaobao.xyz

J. 日期与时间
来源：http://hea.fzhhl.top

================================================================================
来源：http://ywt.hongshengwenyu.top

[J01] 获取当前时间
来源：http://qir.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://bpa.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mcc.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://mkt.bjfxy.top

TS:   new Date();  Date.now()
来源：http://hlb.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://irl.zhengqikj.top

Go:   time.Now()
来源：http://snh.yvedp.cn

Ruby: Time.now
来源：http://fmr.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nby.ehwqpu.com

[J02] 格式化输出
来源：http://hsk.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iju.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvb.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gul.yueranfly.top

TS:   d.toISOString()
来源：http://iei.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ruj.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://upq.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpq.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uxc.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://wrp.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kem.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fqg.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://ejr.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://mki.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://syx.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://run.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://wih.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tbo.bjfxy.top

[J04] 时间戳与日期互转
来源：http://nrq.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jxr.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kbn.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qqy.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://abh.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ynq.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ltr.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hut.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cyt.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://khi.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://pat.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://khp.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kyt.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oop.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://ypz.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ptr.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://fmw.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://smw.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://nfi.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://lsf.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://kof.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://apr.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ijn.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://edz.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://goy.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://kbd.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://kiz.hnxiangtu.top

[J07] 比较两个日期
来源：http://hnz.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://wfl.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cnp.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xpd.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://qjx.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cns.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vpx.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://frn.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://hzp.jiagoushi.top

[J08] 提取年月日与星期
来源：http://pkr.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://icn.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bwp.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hvz.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vdg.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aju.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ygh.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://knd.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rsl.zdbjq.cn

[J09] 时区处理
来源：http://erc.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qwc.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cnk.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yuq.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bqk.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oms.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vsm.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pty.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mjj.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://pqu.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://czk.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fcz.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uii.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ewv.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nyd.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aew.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://umg.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tgl.vqdsnc.cn

================================================================================
来源：http://jal.andypj.xyz

K. JSON 与序列化
来源：http://urk.birdmap.top

================================================================================
来源：http://lmo.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://zoj.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vtq.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lfr.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://qhg.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://wrj.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hxn.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://twf.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://sdq.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://vhh.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://acd.zdbjq.cn

Py:   json.loads(s)
来源：http://nei.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfx.hfpthk.cn

JS:   JSON.parse(s)
来源：http://uuk.birdmap.top

TS:   JSON.parse(s)
来源：http://jzq.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://shj.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://jyv.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://lmr.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zlv.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://zbj.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://olc.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pwu.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://itk.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://csu.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sfa.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://elh.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wkj.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fzq.nwbrower.top

[K04] 读取 JSON 文件
来源：http://jaa.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yki.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jhe.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tlz.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgw.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jdp.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://par.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://txh.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rlx.zhoulong.xyz

[K05] 深拷贝对象
来源：http://udl.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://awm.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://ubk.guowangkeji.top

JS:   structuredClone(obj)
来源：http://pxj.sweek.top

TS:   structuredClone(obj)
来源：http://sfk.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dva.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cez.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qae.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xyw.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://nwl.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://myo.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pvv.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fws.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fld.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://smr.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://otu.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sqr.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mcn.zycfv.cn

[K07] 进制转换
来源：http://ezd.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qqa.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tsk.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ehu.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nlb.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eth.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iox.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hoc.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cnj.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://rbe.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://rxg.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://aev.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ghl.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://zoj.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://run.ybcxt.top

Go:   encoding/gob
来源：http://mtn.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://zpa.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://axb.shangyingyoupin.top

================================================================================
来源：http://fyy.tanke756.top

L. 网络请求
来源：http://dro.cucudq.cn

================================================================================
来源：http://bgt.wangdashe.top

[L01] 发送 GET 请求
来源：http://jnw.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yqy.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rzn.bjfxy.top

JS:   await fetch(url)
来源：http://gjh.yj20258888.top

TS:   await fetch(url)
来源：http://skw.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djm.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://rbc.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zug.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ksf.zdqjudy.top

[L02] 发送 POST JSON
来源：http://cxi.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://clo.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yki.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yjt.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfb.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhi.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://khf.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://okl.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://anf.redwolf501.top

[L03] 设置自定义请求头
来源：http://bcv.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qmr.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://drf.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crb.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gll.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eaq.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wcg.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qew.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://utq.shzxlz.cn

[L04] 设置超时
来源：http://fxq.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://imx.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://woj.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sca.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwp.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cma.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jqu.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pmp.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rrx.yonumen.top

[L05] 上传文件（multipart）
来源：http://puj.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tol.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://raj.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tna.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qmk.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xme.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vnd.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jgk.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsz.c1oappe.top

[L06] 解析响应为 JSON
来源：http://nxp.jinyuanbaomall.cn

Py:   resp.json()
来源：http://jut.hcnkem.com

PHP:  json_decode($body, true);
来源：http://fzd.xinyue.icu

JS:   await resp.json()
来源：http://jly.sweek.top

TS:   await resp.json()
来源：http://bjq.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://osg.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://icz.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://zqk.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eeq.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://rpy.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zyc.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zgq.havefunace.top

JS:   resp.ok;  resp.status
来源：http://kzk.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://wsv.tianlin.xyz

Java: resp.statusCode()
来源：http://rcl.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://ixj.andypj.xyz

Ruby: resp.code.to_i
来源：http://byx.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://yld.andypj.xyz

[L08] 并发请求多个地址
来源：http://fxv.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwv.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://nll.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aka.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eln.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xld.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lji.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bnj.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vub.fanxiaobao.xyz

================================================================================
来源：http://igx.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://wvo.hywenlv.cn

================================================================================
来源：http://wly.snrcjt.cn

[M01] 读取命令行参数
来源：http://bxg.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://yac.yj20258888.top

PHP:  $argv;  $argc;
来源：http://vae.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://ujo.xuanzx.com

TS:   process.argv.slice(2)
来源：http://xay.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://qbv.sjlbkw.cn

Go:   os.Args[1:]
来源：http://bhs.zdqjudy.top

Ruby: ARGV
来源：http://gqm.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://tln.ybcxt.top

[M02] 读取环境变量
来源：http://sfd.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://ptx.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sfh.havefunace.top

JS:   process.env.HOME
来源：http://jhv.guowangkeji.top

TS:   process.env.HOME
来源：http://dzv.jyoumei.cn

Java: System.getenv("HOME")
来源：http://dnw.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vju.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://hvg.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ypy.yangfankeji.com

[M03] 执行外部命令
来源：http://osb.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xjx.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tfs.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pry.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gfm.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sie.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://lyo.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://bhl.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://pql.pycfn.com

[M04] 获取当前工作目录
来源：http://qbh.yanxiufei.cn

Py:   os.getcwd()
来源：http://frq.jiagoushi.top

PHP:  getcwd();
来源：http://hux.wangshuangyany.cn

JS:   process.cwd()
来源：http://yji.xuanzx.com

TS:   process.cwd()
来源：http://tza.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://bat.ydjk.org.cn

Go:   os.Getwd()
来源：http://dmo.meibo888.top

Ruby: Dir.pwd
来源：http://fap.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://ozz.sweek.top

[M05] 设置退出码
来源：http://zax.jianghu66.top

Py:   sys.exit(1)
来源：http://cyv.aibaodan.cn

PHP:  exit(1);
来源：http://kgv.fanxiaobao.xyz


<!-- 参考信息 -->
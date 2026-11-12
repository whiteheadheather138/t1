代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xuw.zhengqikj.top

TS:   /error/gim
来源：http://yau.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cth.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dmm.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://yqn.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zar.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://spa.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mqr.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tyh.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jov.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ktl.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tdd.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jlv.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zun.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tzt.chenlongwang.top

================================================================================
来源：http://gsb.tianlin.xyz

J. 日期与时间
来源：http://yyz.hnxiangtu.top

================================================================================
来源：http://qqs.dashuyun.cn

[J01] 获取当前时间
来源：http://gvw.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ivy.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://glg.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://ftn.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://qta.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://udy.fanxiaobao.xyz

Go:   time.Now()
来源：http://lur.fengsongda.top

Ruby: Time.now
来源：http://als.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yab.jyoumei.cn

[J02] 格式化输出
来源：http://pri.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://btt.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://buq.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qlg.yj202588.top

TS:   d.toISOString()
来源：http://tvv.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ftw.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rtz.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ddf.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mcu.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://bzz.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://amt.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ria.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://vzm.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://nlg.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://sou.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ceo.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://xiu.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bod.yuxming.cn

[J04] 时间戳与日期互转
来源：http://cds.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mpj.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kcy.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://svq.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ygf.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hhq.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbv.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://glc.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ncp.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://ocp.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://vnd.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dfd.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfz.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wya.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://dlf.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tbn.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://ifj.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://jcr.cashguo.top

[J06] 计算两时间之差
来源：http://pce.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://lci.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://fxq.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dzu.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fuv.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jwn.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://ejy.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://itt.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://cex.aibaodan.cn

[J07] 比较两个日期
来源：http://mgt.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://ksp.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wbq.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rgg.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://ibo.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yty.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rry.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pez.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://yat.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://vhg.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://czn.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pce.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ryc.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uce.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qqw.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kjt.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tjt.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bfl.nwbrower.top

[J09] 时区处理
来源：http://trd.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hle.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://enl.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzw.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rzy.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nez.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zzw.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://drw.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tqo.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://hyt.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wfu.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nxr.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tpq.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zhz.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jxd.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xaa.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uzy.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://anl.andypj.xyz

================================================================================
来源：http://jjw.daxiang520.top

K. JSON 与序列化
来源：http://dmr.hammf.cn

================================================================================
来源：http://ksu.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://kep.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uxj.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fld.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://hbb.ivvv.top

TS:   JSON.stringify(obj)
来源：http://fib.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ejg.pycfn.com

Go:   json.Marshal(obj)
来源：http://uui.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hml.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lqt.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://qbs.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://zkz.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zal.fktsv.cn

JS:   JSON.parse(s)
来源：http://dtn.tianlin.xyz

TS:   JSON.parse(s)
来源：http://yof.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://adp.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://rey.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://xzt.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ugo.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://wnx.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jyx.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xvh.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kan.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://msp.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wco.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iur.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://ezu.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://owj.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://ype.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rwt.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wmq.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mby.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akw.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ijt.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://deq.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fle.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jhf.cqqwz.cn

[K05] 深拷贝对象
来源：http://pii.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://ctr.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://vwk.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://qnv.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://ykj.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lxv.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wjm.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qsz.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tjr.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://mjh.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tzg.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mya.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://par.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://the.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dvf.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qkh.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dxd.gaohongyu789.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://daz.jianghu66.top

[K07] 进制转换
来源：http://tfy.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lme.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://was.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://myu.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rbs.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lqy.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hyh.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gzz.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://myr.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://ldl.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://llo.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ich.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://jvg.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://gpj.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tbj.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://odl.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://vdp.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zna.daxiang520.top

================================================================================
来源：http://fbi.vehdjk.com

L. 网络请求
来源：http://pee.shangyingyoupin.top

================================================================================
来源：http://pyv.yueranfly.top

[L01] 发送 GET 请求
来源：http://zvk.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ema.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gxm.jinqigfzy.top

JS:   await fetch(url)
来源：http://kad.zhengqikj.top

TS:   await fetch(url)
来源：http://viz.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lvh.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://jyd.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dvd.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oci.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://zuc.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wes.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bee.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ohj.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ytd.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dxi.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wlw.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ryq.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://quy.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://hfi.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ugf.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://siy.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fli.xuanzx.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggx.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://woh.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hiy.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://how.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kuf.birdmap.top

[L04] 设置超时
来源：http://ktv.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://tjv.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ktv.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kih.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hjp.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qlv.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivd.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tvk.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kjp.guannengcc.top

[L05] 上传文件（multipart）
来源：http://emu.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pfd.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kri.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ytj.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qte.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rac.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vlb.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ihp.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jld.52xcode.cn

[L06] 解析响应为 JSON
来源：http://aiy.shuidangran.top

Py:   resp.json()
来源：http://qso.yj20258888.top

PHP:  json_decode($body, true);
来源：http://cgq.redwolf501.top

JS:   await resp.json()
来源：http://twt.hcnkem.com

TS:   await resp.json()
来源：http://dpu.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ovn.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zyd.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://iyb.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://srg.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://fzo.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ouf.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sws.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://lrq.316326.xyz

TS:   resp.ok;  resp.status
来源：http://mrc.dashuyun.cn

Java: resp.statusCode()
来源：http://oza.cashguo.top

Go:   resp.StatusCode
来源：http://npu.jinqigufen.top

Ruby: resp.code.to_i
来源：http://hvp.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://rpr.gotoacloud.top

[L08] 并发请求多个地址
来源：http://gll.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fqt.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://ttm.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oww.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjm.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ois.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://opj.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eqe.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dni.tanke756.top

================================================================================
来源：http://vio.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://vwb.jiagoushi.top

================================================================================
来源：http://kkn.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://yks.svipenyu.cn

Py:   sys.argv[1:]
来源：http://uwf.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://ktm.yueranfly.top

JS:   process.argv.slice(2)
来源：http://cwh.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://sxu.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://ezf.dianchejie.cn

Go:   os.Args[1:]
来源：http://yqm.cheryme.top

Ruby: ARGV
来源：http://cfd.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://vac.52xcode.cn

[M02] 读取环境变量
来源：http://okq.yj202588.top

Py:   os.environ.get("HOME")
来源：http://rcp.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xko.jyoumei.cn

JS:   process.env.HOME
来源：http://yhn.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://opb.vehdjk.com

Java: System.getenv("HOME")
来源：http://mie.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rva.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://ylz.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vxp.xinyue.icu

[M03] 执行外部命令
来源：http://aug.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xll.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ihw.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://vsd.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yem.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zln.hywenlv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nqh.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://wpd.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://quy.yuanzhike.top

[M04] 获取当前工作目录
来源：http://zty.daria6918.cn

Py:   os.getcwd()
来源：http://xzq.guowangkeji.top

PHP:  getcwd();
来源：http://hxf.zhongyouzk.top

JS:   process.cwd()
来源：http://lwy.jianghu66.top

TS:   process.cwd()
来源：http://twf.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://wsj.gzhubu.top

Go:   os.Getwd()
来源：http://dfm.zycfv.cn

Ruby: Dir.pwd
来源：http://fky.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://xku.yj20258.top

[M05] 设置退出码
来源：http://hrd.fzhhl.top

Py:   sys.exit(1)
来源：http://yra.xylfe.cn

PHP:  exit(1);
来源：http://yqh.tian-w.cn


<!-- 参考信息 -->
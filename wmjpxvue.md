代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vvt.sufxvd.cn

TS:   /error/gim
来源：http://odj.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://drd.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jwp.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://kfp.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bov.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://qmd.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://glc.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uqh.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ksr.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zah.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tfy.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pqt.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://czb.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dnl.vehdjk.com

================================================================================
来源：http://msz.vehdjk.com

J. 日期与时间
来源：http://ind.pycfn.com

================================================================================
来源：http://qgo.zdqjudy.top

[J01] 获取当前时间
来源：http://zxb.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wjo.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://odf.ybcxt.top

JS:   new Date();  Date.now()
来源：http://mmi.jianghu66.top

TS:   new Date();  Date.now()
来源：http://ays.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bve.shanyushiyangkeji.top

Go:   time.Now()
来源：http://xaz.yongpay.top

Ruby: Time.now
来源：http://hgi.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nkt.316326.xyz

[J02] 格式化输出
来源：http://ubb.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tra.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wlg.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cbw.zhongyouzk.top

TS:   d.toISOString()
来源：http://eug.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://atq.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mtq.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fjl.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wqn.316326.xyz

[J03] 字符串解析为日期
来源：http://fjq.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://itd.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cbj.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://gzx.yj202588.top

TS:   new Date("2024-01-02")
来源：http://yjt.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://dbs.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mpr.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://gpy.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sqf.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://xie.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vkq.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ekl.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rtm.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lms.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://clc.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cii.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hxg.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zue.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://tcn.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://fkm.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nsx.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sjl.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pph.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://jbp.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dbc.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://kfv.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://kpx.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://syd.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://kmu.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://vvr.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kyo.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qvi.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://gjz.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://vae.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://ztj.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://ygu.zhijiandao.cn

[J07] 比较两个日期
来源：http://sll.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://snq.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wgq.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://apj.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://miy.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zue.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://veg.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://qyr.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://jbn.iojbl.cn

[J08] 提取年月日与星期
来源：http://wpq.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dko.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tan.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bbl.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kej.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kjk.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://scy.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ifv.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bgc.jqgufenzy.top

[J09] 时区处理
来源：http://hrs.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://feq.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iij.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jje.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbm.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hcr.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gpb.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://glr.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jgr.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://ose.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qhz.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yek.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gih.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://upv.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uxz.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jjs.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fxu.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fea.ydjk.org.cn

================================================================================
来源：http://xlb.zhiwuduotai.top

K. JSON 与序列化
来源：http://wzl.yfazqb.com

================================================================================
来源：http://qav.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://sbb.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cnc.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uok.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://uit.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://srq.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://txt.shuidangran.top

Go:   json.Marshal(obj)
来源：http://rfn.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://bca.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://czw.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://qwt.nwbrower.top

Py:   json.loads(s)
来源：http://oto.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cvy.tarul.cn

JS:   JSON.parse(s)
来源：http://mou.zhixingplan.top

TS:   JSON.parse(s)
来源：http://wel.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://isq.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://tbo.hcnkem.com

Ruby: JSON.parse(s)
来源：http://wwm.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yak.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://qrf.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zsk.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nnp.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yhs.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wfd.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qji.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xof.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://urt.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lah.fktsv.cn

[K04] 读取 JSON 文件
来源：http://cwm.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kjk.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://osx.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zgw.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcs.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bce.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wfr.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rvz.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jjd.jlsjyb.cn

[K05] 深拷贝对象
来源：http://orj.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://gwx.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://toz.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://ffk.tian-w.cn

TS:   structuredClone(obj)
来源：http://yax.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dvm.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zyp.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kzj.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aap.tian-w.cn

[K06] 解析 URL 查询串
来源：http://eew.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hbs.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sgj.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ksp.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iuq.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phe.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://jaq.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://acg.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ffe.hongshengwenyu.top

[K07] 进制转换
来源：http://sio.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hqu.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://usj.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iyn.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tsx.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jsx.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jkd.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sxs.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vtu.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://fau.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://rak.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yni.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://nzm.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://agh.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hzz.sweek.top

Go:   encoding/gob
来源：http://oad.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://wtp.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kub.xinyue.icu

================================================================================
来源：http://hqf.yvedp.cn

L. 网络请求
来源：http://beo.redwolf501.top

================================================================================
来源：http://spu.chenlongwang.top

[L01] 发送 GET 请求
来源：http://glf.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rco.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://seu.svipenyu.cn

JS:   await fetch(url)
来源：http://usp.ehwqpu.com

TS:   await fetch(url)
来源：http://uhy.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qqd.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://pww.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zaz.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://csb.zhengqikj.top

[L02] 发送 POST JSON
来源：http://zie.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://szd.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vdr.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fzz.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqe.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sij.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rhs.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oxv.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tew.xuanzx.com

[L03] 设置自定义请求头
来源：http://tat.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yvl.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://syp.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://koo.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wmz.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oyo.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://afl.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wse.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yge.hfpthk.cn

[L04] 设置超时
来源：http://say.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://bjo.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mvz.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tbo.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tzs.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vzx.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jgh.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hyb.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://msm.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://tcg.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uso.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ujr.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rim.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gwa.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zej.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nya.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qxe.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dvb.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://brd.svipenyu.cn

Py:   resp.json()
来源：http://yeq.iojbl.cn

PHP:  json_decode($body, true);
来源：http://ukg.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://tlh.kuanghao11.cn

TS:   await resp.json()
来源：http://qxw.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hwm.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gye.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://jkk.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dhd.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://sql.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lwz.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ygi.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://zux.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://yiz.yonumen.top

Java: resp.statusCode()
来源：http://huo.bjfxy.top

Go:   resp.StatusCode
来源：http://bok.bbcook.cn

Ruby: resp.code.to_i
来源：http://hwg.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://whb.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://yet.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tqu.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://jmg.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tix.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yhq.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zxm.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://trt.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ypd.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://koe.aizwys.cn

================================================================================
来源：http://thn.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://noc.52xcode.cn

================================================================================
来源：http://gsl.sysykeji.top

[M01] 读取命令行参数
来源：http://lgr.redwolf501.top

Py:   sys.argv[1:]
来源：http://zes.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://pwz.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://jby.mhx1999.top

TS:   process.argv.slice(2)
来源：http://kcx.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://ozf.sweek.top

Go:   os.Args[1:]
来源：http://zvp.sysykeji.top

Ruby: ARGV
来源：http://jzm.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://fsc.fktsv.cn

[M02] 读取环境变量
来源：http://zne.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://pds.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://euv.ydzc1.top

JS:   process.env.HOME
来源：http://tal.redwolf501.top

TS:   process.env.HOME
来源：http://gko.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://zuy.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fri.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://sex.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://shk.sufxvd.cn

[M03] 执行外部命令
来源：http://zep.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vxn.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dxx.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kvg.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://dxv.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cac.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fzp.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cko.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://mta.haohaochexian.top

[M04] 获取当前工作目录
来源：http://fgp.cdnleiting.top

Py:   os.getcwd()
来源：http://zjd.316326.xyz

PHP:  getcwd();
来源：http://syf.yvedp.cn

JS:   process.cwd()
来源：http://wce.nanxuanxn.top

TS:   process.cwd()
来源：http://csq.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://gjm.yfazqb.com

Go:   os.Getwd()
来源：http://xas.ydjk.org.cn

Ruby: Dir.pwd
来源：http://vhs.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://kmf.aizwys.cn

[M05] 设置退出码
来源：http://xyd.zdqjudy.top

Py:   sys.exit(1)
来源：http://bqv.ctjpmb.com

PHP:  exit(1);
来源：http://mja.fanxiaobao.xyz


<!-- 参考信息 -->
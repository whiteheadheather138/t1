代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fbz.ywan-chungtsiang.top

TS:   /error/gim
来源：http://zan.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tdu.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://afe.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://weq.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uxq.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://pdm.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://msc.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lav.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wud.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zoq.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jlv.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hiw.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ucj.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://stv.jlsjyb.cn

================================================================================
来源：http://wog.yueranfly.top

J. 日期与时间
来源：http://anw.zhijiandao.cn

================================================================================
来源：http://orq.fzhhl.top

[J01] 获取当前时间
来源：http://pis.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://anm.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tbt.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://wed.yfazqb.com

TS:   new Date();  Date.now()
来源：http://jfp.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tep.dianchejie.cn

Go:   time.Now()
来源：http://ylj.chenlongwang.top

Ruby: Time.now
来源：http://rpr.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://svf.nanxinkj.top

[J02] 格式化输出
来源：http://kzz.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qig.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rmy.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cbp.wangdashe.top

TS:   d.toISOString()
来源：http://cdn.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oms.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rlf.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iez.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tqi.ehwqpu.com

[J03] 字符串解析为日期
来源：http://mob.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://poi.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ydb.yj20258.top

JS:   new Date("2024-01-02")
来源：http://cmq.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://psv.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://bxm.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jlv.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://kmh.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tst.bjfxy.top

[J04] 时间戳与日期互转
来源：http://ico.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vnv.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mqh.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lcm.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ssi.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wai.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ffh.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fpa.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mvv.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://wwm.meibo888.top

Py:   now + timedelta(days=7)
来源：http://pwm.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kel.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ecy.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ggc.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://dwx.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tvm.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://hog.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://zzr.zdqjudy.top

[J06] 计算两时间之差
来源：http://ppc.yonumen.top

Py:   (end - start).total_seconds()
来源：http://xme.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://zjp.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baq.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yoe.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vno.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://mzl.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://yaz.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://fho.gogol.net.cn

[J07] 比较两个日期
来源：http://yco.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://esv.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kqh.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gep.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dsc.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rbk.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ist.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://dbp.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://efz.tarul.cn

[J08] 提取年月日与星期
来源：http://vhd.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ueu.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lpi.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cvy.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ahq.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://akf.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kfw.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyc.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ngr.xuetiantiany.cn

[J09] 时区处理
来源：http://ezb.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qvi.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cwo.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgg.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://osl.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xez.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rwg.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zze.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jmo.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://sad.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iuu.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fxf.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rdj.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pea.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sdk.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sin.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hhq.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wtk.wangshuangyany.cn

================================================================================
来源：http://yjh.ehwqpu.com

K. JSON 与序列化
来源：http://irk.hfpthk.cn

================================================================================
来源：http://hev.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://agi.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lug.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gmf.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://abg.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://qfn.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mam.gzhubu.top

Go:   json.Marshal(obj)
来源：http://pna.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://btw.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://mhs.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://mxg.hfpthk.cn

Py:   json.loads(s)
来源：http://nri.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qmi.zdbjq.cn

JS:   JSON.parse(s)
来源：http://gld.zhixingplan.top

TS:   JSON.parse(s)
来源：http://bio.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qsk.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://syb.yfazqb.com

Ruby: JSON.parse(s)
来源：http://hpi.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gaw.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://xdj.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kna.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://crt.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tvi.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lrf.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ocj.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gfw.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://fom.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wyf.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://odq.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lxg.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ukq.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esz.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxm.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fxi.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mul.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qtw.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pnt.hammf.cn

[K05] 深拷贝对象
来源：http://ryh.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://qif.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://jkm.jinqigufen.top

JS:   structuredClone(obj)
来源：http://tzu.aibaodan.cn

TS:   structuredClone(obj)
来源：http://xpq.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aag.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bvo.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://msi.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vio.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://ulj.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zrp.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ryt.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uub.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uri.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gkc.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xsn.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dkf.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sfg.jqgufenzy.top

[K07] 进制转换
来源：http://xlf.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://grz.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://twy.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://etm.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yrs.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kis.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fbq.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://moe.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://drd.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://uls.meibo888.top

Py:   pickle.dumps(obj)
来源：http://rga.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://knj.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://fnh.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://vlo.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://plm.yongpay.top

Go:   encoding/gob
来源：http://gnb.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://xja.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvv.gotoacloud.top

================================================================================
来源：http://dpg.yangfankeji.com

L. 网络请求
来源：http://ujz.shangyingyoupin.top

================================================================================
来源：http://ynx.aibaodan.cn

[L01] 发送 GET 请求
来源：http://jru.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lwk.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ulc.ivvv.top

JS:   await fetch(url)
来源：http://fcu.yj20258888.top

TS:   await fetch(url)
来源：http://emj.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cyu.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://hcc.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sbx.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zsg.zdqjudy.top

[L02] 发送 POST JSON
来源：http://fge.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://vbl.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ekw.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qxp.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lpp.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dnk.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rbl.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cic.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xvk.cheryme.top

[L03] 设置自定义请求头
来源：http://pnl.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jaq.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fsq.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oim.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wep.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wdi.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hll.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vqn.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqu.cheryme.top

[L04] 设置超时
来源：http://qyo.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://twh.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://onz.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oue.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pho.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gjc.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hjt.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uis.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pyj.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://ltx.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://utz.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://edi.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://feq.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tcn.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://upr.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lcd.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fis.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mnl.sweek.top

[L06] 解析响应为 JSON
来源：http://iya.quarkkingdee.top

Py:   resp.json()
来源：http://lvg.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://jol.nanxinkj.top

JS:   await resp.json()
来源：http://xdx.hfpthk.cn

TS:   await resp.json()
来源：http://ymb.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wqv.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uxt.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://xos.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vbv.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://ywk.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bks.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://spe.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://xiv.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://yeq.gotoacloud.top

Java: resp.statusCode()
来源：http://wzy.vehdjk.com

Go:   resp.StatusCode
来源：http://ety.zdqjudy.top

Ruby: resp.code.to_i
来源：http://cur.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://ppp.fehbvm.com

[L08] 并发请求多个地址
来源：http://fip.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cpq.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://yrm.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxs.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iso.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pej.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://srq.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baq.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pti.ctjpmb.com

================================================================================
来源：http://huf.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://lkd.guowangkeji.top

================================================================================
来源：http://fvk.aizwys.cn

[M01] 读取命令行参数
来源：http://aml.tianlin.xyz

Py:   sys.argv[1:]
来源：http://eed.xylfe.cn

PHP:  $argv;  $argc;
来源：http://cuo.ivvv.top

JS:   process.argv.slice(2)
来源：http://jqi.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://mfo.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://pvv.daxiang520.top

Go:   os.Args[1:]
来源：http://hbj.cqqwz.cn

Ruby: ARGV
来源：http://rrt.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://zem.0kj1m.cn

[M02] 读取环境变量
来源：http://csx.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://wtu.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ugo.guowangkeji.top

JS:   process.env.HOME
来源：http://xyn.sjlbkw.cn

TS:   process.env.HOME
来源：http://ile.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://dhz.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thx.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://jii.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oco.xylfe.cn

[M03] 执行外部命令
来源：http://pqt.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://szw.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ipn.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://qbn.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tid.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hgy.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uzd.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://ibf.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://cjl.yuanzhike.top

[M04] 获取当前工作目录
来源：http://yfz.hysaishi.cn

Py:   os.getcwd()
来源：http://itd.xuetiantiany.cn

PHP:  getcwd();
来源：http://knq.jinqigfzy.top

JS:   process.cwd()
来源：http://rit.jinghuilouyu.cn

TS:   process.cwd()
来源：http://nty.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://fnm.kuanghao11.cn

Go:   os.Getwd()
来源：http://bpi.meibo888.top

Ruby: Dir.pwd
来源：http://hpp.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dmf.gzhubu.top

[M05] 设置退出码
来源：http://gzq.ydzc1.top

Py:   sys.exit(1)
来源：http://tmq.jianghu66.top

PHP:  exit(1);
来源：http://qgz.hnxiangtu.top


<!-- 参考信息 -->
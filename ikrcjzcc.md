代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wav.jinqigfzy.top

TS:   /error/gim
来源：http://xgg.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nac.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tep.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://fzp.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qit.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://col.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xnd.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tjm.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dfm.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://adc.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vas.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ihq.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kkd.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssm.jinqigufen.top

================================================================================
来源：http://yas.xylfe.cn

J. 日期与时间
来源：http://uag.uphjek.com

================================================================================
来源：http://hik.havefunace.top

[J01] 获取当前时间
来源：http://zgq.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gqu.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iow.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://hxg.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://sqp.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lgn.nanxinkj.top

Go:   time.Now()
来源：http://uxg.nanxuanxn.top

Ruby: Time.now
来源：http://kvr.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bqw.xuanzx.com

[J02] 格式化输出
来源：http://hxl.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lcf.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yxa.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gdm.dashuyun.cn

TS:   d.toISOString()
来源：http://rbq.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gfc.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zzs.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzv.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dhl.aizwys.cn

[J03] 字符串解析为日期
来源：http://edg.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bon.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mhb.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://uyh.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://jvo.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wzc.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lth.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://ikv.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tnq.shuidangran.top

[J04] 时间戳与日期互转
来源：http://pry.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qjx.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nje.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rfa.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eez.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://enq.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ayh.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sfu.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nvx.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://ddf.pycfn.com

Py:   now + timedelta(days=7)
来源：http://hcb.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qtw.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgr.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzz.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://mcs.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wmv.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://rhl.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mxj.yfazqb.com

[J06] 计算两时间之差
来源：http://zhq.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://yas.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://ene.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lbt.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://obe.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://iuf.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://fyo.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://ats.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://chx.jqgfzy.top

[J07] 比较两个日期
来源：http://vmd.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://gjc.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nkc.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://skv.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xmi.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fxn.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xot.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wed.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://yas.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://mdu.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fif.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lia.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dox.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yin.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tis.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pgl.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cew.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dup.jinqigfzy.top

[J09] 时区处理
来源：http://tmg.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ijh.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gsd.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvo.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogm.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fwa.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pws.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vdt.snrcjt.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lvz.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://hoe.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://vof.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fgi.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://upn.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vmg.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://izj.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kpz.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uoo.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ruk.0kj1m.cn

================================================================================
来源：http://aij.andypj.xyz

K. JSON 与序列化
来源：http://ijx.yj20258.top

================================================================================
来源：http://yii.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://icr.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cdd.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gta.sweek.top

JS:   JSON.stringify(obj)
来源：http://tqx.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://ttv.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://adc.xziqi.cn

Go:   json.Marshal(obj)
来源：http://vht.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://djv.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://acf.daxiang520.top

[K02] JSON 字符串转对象
来源：http://vbj.nanxuanxn.top

Py:   json.loads(s)
来源：http://mxk.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ush.yongpay.top

JS:   JSON.parse(s)
来源：http://ztr.tian-w.cn

TS:   JSON.parse(s)
来源：http://sdf.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lzx.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://zkd.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://tzs.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://anz.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://aqm.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gvt.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mgp.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fgg.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://kao.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wdq.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tfu.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://enj.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gye.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://lxr.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://klx.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cgy.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wkq.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpg.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ntp.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akr.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fbn.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iqo.yueranfly.top

[K05] 深拷贝对象
来源：http://ljw.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://mns.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://xdl.jiagoushi.top

JS:   structuredClone(obj)
来源：http://gec.9152youxi.cn

TS:   structuredClone(obj)
来源：http://pds.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aug.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uuj.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dui.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iao.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://tub.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vcd.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwh.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://obf.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wjk.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rfk.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rqi.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axz.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ffd.gaohongyu789.top

[K07] 进制转换
来源：http://tah.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dkl.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rik.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fdt.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ddr.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xmr.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yrk.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jgg.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mko.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://vke.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://cbq.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://xap.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://ijf.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://obg.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zcs.jqgfzy.top

Go:   encoding/gob
来源：http://gko.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://usa.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://scj.zycfv.cn

================================================================================
来源：http://ynz.tanke756.top

L. 网络请求
来源：http://mll.wangshuangyany.cn

================================================================================
来源：http://qlx.sysykeji.top

[L01] 发送 GET 请求
来源：http://eaw.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lhg.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pri.tarul.cn

JS:   await fetch(url)
来源：http://qma.zhiwuduotai.top

TS:   await fetch(url)
来源：http://lzj.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eqp.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://fbk.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kzx.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kos.snrcjt.cn

[L02] 发送 POST JSON
来源：http://maa.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://alp.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kcz.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ncy.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dwa.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mtu.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vcn.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ugj.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://twy.xinyue.icu

[L03] 设置自定义请求头
来源：http://aqj.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zwb.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wzb.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sin.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qtz.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://naq.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jni.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dgv.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://reb.cheryme.top

[L04] 设置超时
来源：http://uoe.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://htw.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://htd.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wzq.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofb.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cvq.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eei.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://okn.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://trn.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://rqs.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://koh.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://feo.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yiv.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lcz.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bnp.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bco.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://imr.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jnm.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://nni.jqgufenzy.top

Py:   resp.json()
来源：http://hck.sysykeji.top

PHP:  json_decode($body, true);
来源：http://xzo.dashuyun.cn

JS:   await resp.json()
来源：http://qgy.epnwcf.com

TS:   await resp.json()
来源：http://etc.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ftr.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lem.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://epl.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dll.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://cbb.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iie.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pps.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://uxh.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://jsy.nwbrower.top

Java: resp.statusCode()
来源：http://asd.sjlbkw.cn

Go:   resp.StatusCode
来源：http://wll.snrcjt.cn

Ruby: resp.code.to_i
来源：http://zgu.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://bjc.fktsv.cn

[L08] 并发请求多个地址
来源：http://byk.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nbf.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://mki.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gtd.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qeu.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://trs.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ubq.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rcd.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dio.andypj.xyz

================================================================================
来源：http://fat.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://ato.hnxiangtu.top

================================================================================
来源：http://nka.ybcxt.top

[M01] 读取命令行参数
来源：http://wtj.fktsv.cn

Py:   sys.argv[1:]
来源：http://mix.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://caw.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://duu.sxryk.cn

TS:   process.argv.slice(2)
来源：http://cgj.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://ykj.yj20258888.top

Go:   os.Args[1:]
来源：http://via.zhengqikj.top

Ruby: ARGV
来源：http://haw.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://xyr.bbcook.cn

[M02] 读取环境变量
来源：http://far.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://jdf.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qns.xinyue.icu

JS:   process.env.HOME
来源：http://abo.yuanzhike.top

TS:   process.env.HOME
来源：http://wss.hcnkem.com

Java: System.getenv("HOME")
来源：http://ntm.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://trq.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://wso.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ejr.xuanzx.com

[M03] 执行外部命令
来源：http://kqk.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wuo.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://djk.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://udg.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gng.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xzc.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://hnh.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mth.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://szl.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://nrz.sxryk.cn

Py:   os.getcwd()
来源：http://iuy.tanke756.top

PHP:  getcwd();
来源：http://rqy.iojbl.cn

JS:   process.cwd()
来源：http://htf.nwbrower.top

TS:   process.cwd()
来源：http://ypi.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://jer.daxiang520.top

Go:   os.Getwd()
来源：http://tgl.sufxvd.cn

Ruby: Dir.pwd
来源：http://ldx.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oht.fktsv.cn

[M05] 设置退出码
来源：http://zka.ehwqpu.com

Py:   sys.exit(1)
来源：http://lkz.andypj.xyz

PHP:  exit(1);
来源：http://mqu.gzhubu.top


<!-- 参考信息 -->
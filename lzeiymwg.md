代发 wailian999

Ruby: s.scan(/error/i)
来源：http://lbg.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hzl.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://bdm.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zjj.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pcr.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kob.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnc.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qsc.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xjn.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jfn.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cjj.ppjwa.cn

================================================================================
来源：http://xac.wangshuangyany.cn

J. 日期与时间
来源：http://brk.aizwys.cn

================================================================================
来源：http://bmc.yj202588.top

[J01] 获取当前时间
来源：http://yje.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mvh.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ril.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://odw.smart0.xyz

TS:   new Date();  Date.now()
来源：http://olx.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://abb.gotoacloud.top

Go:   time.Now()
来源：http://tnk.chenjidiqi.icu

Ruby: Time.now
来源：http://zgp.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bye.haohaochexian.top

[J02] 格式化输出
来源：http://six.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jmz.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ijp.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dia.redwolf501.top

TS:   d.toISOString()
来源：http://qjs.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://efg.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jzy.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ntv.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oed.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://nxz.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://exn.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ucc.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://mck.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://vld.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://znw.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tou.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://uho.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sfi.52xcode.cn

[J04] 时间戳与日期互转
来源：http://rpk.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://inv.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vto.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bte.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pyj.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cca.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://atl.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pke.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iym.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://phr.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://yfx.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xyk.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://afh.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://evt.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://xfp.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://afz.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://tul.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://hef.yonumen.top

[J06] 计算两时间之差
来源：http://hyv.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://xnb.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://xjc.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zbi.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yqx.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://igv.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://lcw.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://lfb.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://tmo.jianghu66.top

[J07] 比较两个日期
来源：http://wfb.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://sal.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yfh.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gym.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://ghl.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://odz.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gcm.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://lqh.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://mer.daria6918.cn

[J08] 提取年月日与星期
来源：http://zej.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kfq.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nkq.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wrl.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ycl.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qrf.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nti.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jqz.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xtc.hywenlv.cn

[J09] 时区处理
来源：http://ngc.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mhb.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kna.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gcx.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dvz.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kqy.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://czr.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hle.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gzp.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://oht.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iul.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mrw.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qga.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rcg.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zfz.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://obf.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vzn.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fbc.jqgufenzy.top

================================================================================
来源：http://bdi.shzxlz.cn

K. JSON 与序列化
来源：http://ddw.aibaodan.cn

================================================================================
来源：http://rky.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://xat.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zsp.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jhb.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://mvt.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://wax.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jbr.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://pjg.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://erf.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tjh.ivvv.top

[K02] JSON 字符串转对象
来源：http://eje.ctjpmb.com

Py:   json.loads(s)
来源：http://bpa.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hdc.jianghu66.top

JS:   JSON.parse(s)
来源：http://zds.zhixingplan.top

TS:   JSON.parse(s)
来源：http://gul.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pik.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://fei.fehbvm.com

Ruby: JSON.parse(s)
来源：http://usf.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zlf.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://fzn.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kkr.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qrl.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://gkp.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://qaj.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://twk.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fgm.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://raq.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wuw.sxryk.cn

[K04] 读取 JSON 文件
来源：http://xsn.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hqi.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dmq.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sce.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ilv.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eme.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ofb.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pwm.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ygl.ppjwa.cn

[K05] 深拷贝对象
来源：http://hxc.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://ezr.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://pfg.yj202588.top

JS:   structuredClone(obj)
来源：http://xyy.mhx1999.top

TS:   structuredClone(obj)
来源：http://adh.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xrg.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iuq.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kus.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zut.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://thv.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jmt.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pih.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxb.jianghu66.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emw.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sue.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uvr.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oxg.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fiy.tarul.cn

[K07] 进制转换
来源：http://amx.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rve.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dlo.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mez.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wxd.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://awr.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jmc.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rmu.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vmi.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://xos.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://ukr.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vvr.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://eum.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://lck.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fln.meibo888.top

Go:   encoding/gob
来源：http://uvt.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://zvz.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://odl.kuanghao11.cn

================================================================================
来源：http://zdl.shanyushiyangtech.top

L. 网络请求
来源：http://bzt.jianghu66.top

================================================================================
来源：http://diq.zhixingplan.top

[L01] 发送 GET 请求
来源：http://tkv.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kjg.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbi.nanxuanxn.top

JS:   await fetch(url)
来源：http://rlx.yj20258888.top

TS:   await fetch(url)
来源：http://zau.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pqm.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://uie.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wkl.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fpw.ydzc1.top

[L02] 发送 POST JSON
来源：http://hcl.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tyb.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://huk.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vqt.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qom.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xfn.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vki.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://was.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sxd.yonumen.top

[L03] 设置自定义请求头
来源：http://xsn.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kon.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wch.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kvu.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qic.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aws.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://biz.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kwq.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vmw.daria6918.cn

[L04] 设置超时
来源：http://jkz.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://yly.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mnx.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nqq.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qbf.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://usp.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jsu.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gkt.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pcl.hnqzz.top

[L05] 上传文件（multipart）
来源：http://vwg.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gan.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bfh.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gde.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nfp.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sli.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ihd.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hyr.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mtq.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://aqo.cashguo.top

Py:   resp.json()
来源：http://pof.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://alo.smart0.xyz

JS:   await resp.json()
来源：http://txy.kuanghao11.cn

TS:   await resp.json()
来源：http://mlz.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ljj.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wnp.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://rqm.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ajb.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://whh.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://one.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://toh.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://edd.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://gca.9152youxi.cn

Java: resp.statusCode()
来源：http://cpy.jianghu66.top

Go:   resp.StatusCode
来源：http://qqr.cdnleiting.top

Ruby: resp.code.to_i
来源：http://cud.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://xsh.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://tbi.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ydh.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://vet.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfi.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://igv.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dpj.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uvy.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nfq.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xgg.bbcook.cn

================================================================================
来源：http://gdn.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://sac.quarkkingdee.top

================================================================================
来源：http://hhd.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://vrj.sysykeji.top

Py:   sys.argv[1:]
来源：http://vvi.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://otm.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://jod.ivvv.top

TS:   process.argv.slice(2)
来源：http://dfb.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://vjv.yj202588.top

Go:   os.Args[1:]
来源：http://fqd.yongpay.top

Ruby: ARGV
来源：http://sbw.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://fxp.snrcjt.cn

[M02] 读取环境变量
来源：http://iay.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://cam.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ieb.vqdsnc.cn

JS:   process.env.HOME
来源：http://zii.yj20258888.top

TS:   process.env.HOME
来源：http://hum.fehbvm.com

Java: System.getenv("HOME")
来源：http://sba.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cwf.fengsongda.top

Ruby: ENV["HOME"]
来源：http://jts.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://paa.jqgfzy.top

[M03] 执行外部命令
来源：http://vjv.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mvv.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kgw.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tkb.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nac.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jdx.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ppu.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://zzw.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://krx.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://hia.gaohongyu789.top

Py:   os.getcwd()
来源：http://cor.fehbvm.com

PHP:  getcwd();
来源：http://qkp.jqgufenzy.top

JS:   process.cwd()
来源：http://bfa.pycfn.com

TS:   process.cwd()
来源：http://akj.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://cxd.yfazqb.com

Go:   os.Getwd()
来源：http://upr.vehdjk.com

Ruby: Dir.pwd
来源：http://vtd.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tbr.guannengcc.top

[M05] 设置退出码
来源：http://hlk.hesvh.cn

Py:   sys.exit(1)
来源：http://sev.9152youxi.cn

PHP:  exit(1);
来源：http://hfg.hammf.cn

JS:   process.exit(1)
来源：http://qfg.wangdashe.top

TS:   process.exit(1)
来源：http://nyo.chenzaomai.com

Java: System.exit(1)
来源：http://txr.jlsjyb.cn

Go:   os.Exit(1)
来源：http://swa.tianlin.xyz


<!-- 参考信息 -->
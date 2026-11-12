代发 wailian999

Ruby: s.scan(/error/i)
来源：http://drt.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kur.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://ctq.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wjw.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jxh.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmz.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://whp.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ouh.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qzl.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wke.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fhk.meibo888.top

================================================================================
来源：http://dii.daxiang520.top

J. 日期与时间
来源：http://pbq.ybcxt.top

================================================================================
来源：http://zzh.zhijiandao.cn

[J01] 获取当前时间
来源：http://irj.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://alw.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pjw.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://dmy.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://lgd.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cev.sjlbkw.cn

Go:   time.Now()
来源：http://urg.cheryme.top

Ruby: Time.now
来源：http://dti.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jww.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://xsl.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://whd.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://elg.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ihe.wangshuangyany.cn

TS:   d.toISOString()
来源：http://ncu.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bvt.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lrt.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xbu.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pue.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://mog.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rnu.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aga.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://vrx.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://tso.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://rrv.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bmf.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://nvy.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pit.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://igu.gogol.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ozy.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gpu.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://egx.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dev.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ddh.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nmt.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uuy.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nxh.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://ybp.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://hpb.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://bun.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sar.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltz.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://tno.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kwh.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://acm.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://gag.shzxlz.cn

[J06] 计算两时间之差
来源：http://fcd.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://eed.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://ski.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yie.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://puo.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://ywb.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://mks.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://til.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://cjs.zhixingplan.top

[J07] 比较两个日期
来源：http://rjg.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://iyg.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cfz.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://gej.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pgx.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://roy.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://imf.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://arh.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ikr.hfpthk.cn

[J08] 提取年月日与星期
来源：http://qpp.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dye.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bmj.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vqw.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://avg.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xsr.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mew.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ipz.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fvu.jinqigfzy.top

[J09] 时区处理
来源：http://tjo.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qzy.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gpd.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dna.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rga.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iqt.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hyj.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ksy.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://okv.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://lgj.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kig.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ksa.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cnh.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wpm.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mmm.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pxd.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kwl.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hes.wangdashe.top

================================================================================
来源：http://gme.xinyue.icu

K. JSON 与序列化
来源：http://kls.yueranfly.top

================================================================================
来源：http://nne.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://ydm.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://muf.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zov.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://gli.tarul.cn

TS:   JSON.stringify(obj)
来源：http://shs.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svi.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://juo.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://grq.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jbp.xziqi.cn

[K02] JSON 字符串转对象
来源：http://afs.bjfxy.top

Py:   json.loads(s)
来源：http://pqz.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://itz.hnqzz.top

JS:   JSON.parse(s)
来源：http://iyl.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://tnx.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cci.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://srb.yvedp.cn

Ruby: JSON.parse(s)
来源：http://nxu.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nwe.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://pmu.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bok.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mkv.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lvl.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://gow.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wqm.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uav.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://agw.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qdu.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://uic.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fhw.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://leq.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wge.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yvl.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fok.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zby.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jom.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rcg.fehbvm.com

[K05] 深拷贝对象
来源：http://wwz.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://rrr.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://rhu.jianghu66.top

JS:   structuredClone(obj)
来源：http://akd.jyoumei.cn

TS:   structuredClone(obj)
来源：http://qhc.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lsq.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ktp.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iov.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mpo.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://yff.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsy.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dmt.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jnd.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bja.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://whu.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://glv.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hca.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oby.quarkkingdee.top

[K07] 进制转换
来源：http://uqt.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pqh.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ede.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sha.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bfa.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lgo.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jlv.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://unc.jqgufenzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://afr.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://yck.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://rdp.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ode.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://fgg.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://xvx.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dcz.yj20258888.top

Go:   encoding/gob
来源：http://dnv.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://bsq.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://atr.feifeiyinyue.top

================================================================================
来源：http://qeh.guannengcc.top

L. 网络请求
来源：http://bez.zhijiandao.cn

================================================================================
来源：http://tpa.fzhhl.top

[L01] 发送 GET 请求
来源：http://jnm.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ekd.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ufz.hfpthk.cn

JS:   await fetch(url)
来源：http://hta.shuidangran.top

TS:   await fetch(url)
来源：http://sqj.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wzm.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://agc.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://wqd.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://znv.ivvv.top

[L02] 发送 POST JSON
来源：http://obm.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://hvp.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iwj.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qxf.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ynp.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qsa.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jsc.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qao.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mcm.yonumen.top

[L03] 设置自定义请求头
来源：http://mui.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://epu.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ksu.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyg.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncc.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dip.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hqc.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://leh.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kxf.cucudq.cn

[L04] 设置超时
来源：http://kot.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://ney.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pnh.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vnq.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vol.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ejv.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tbt.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fya.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qmm.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://wuh.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ioj.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tdb.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zho.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vek.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vxj.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://auh.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zve.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://axw.yonumen.top

[L06] 解析响应为 JSON
来源：http://ovz.cucudq.cn

Py:   resp.json()
来源：http://lcg.ivvv.top

PHP:  json_decode($body, true);
来源：http://kdd.havefunace.top

JS:   await resp.json()
来源：http://mwy.gotoacloud.top

TS:   await resp.json()
来源：http://hux.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bpt.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wiq.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://eas.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dna.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://esq.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bqo.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uuo.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://ocu.pycfn.com

TS:   resp.ok;  resp.status
来源：http://pyj.gogol.net.cn

Java: resp.statusCode()
来源：http://kym.fengsongda.top

Go:   resp.StatusCode
来源：http://xhk.tianlin.xyz

Ruby: resp.code.to_i
来源：http://tdd.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://etq.haohaochexian.top

[L08] 并发请求多个地址
来源：http://fiu.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hhg.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://mom.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bui.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cla.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://flm.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wgd.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dng.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sbe.ydzc1.top

================================================================================
来源：http://jbh.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://mim.fehbvm.com

================================================================================
来源：http://ajb.tanke756.top

[M01] 读取命令行参数
来源：http://egu.xylfe.cn

Py:   sys.argv[1:]
来源：http://daf.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://hgl.yfazqb.com

JS:   process.argv.slice(2)
来源：http://yaf.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://pvg.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://qlg.yonumen.top

Go:   os.Args[1:]
来源：http://ejj.birdmap.top

Ruby: ARGV
来源：http://hzx.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://mgl.cucudq.cn

[M02] 读取环境变量
来源：http://zuy.cashguo.top

Py:   os.environ.get("HOME")
来源：http://jvs.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oum.0kj1m.cn

JS:   process.env.HOME
来源：http://mrr.gotoacloud.top

TS:   process.env.HOME
来源：http://rjt.zycfv.cn

Java: System.getenv("HOME")
来源：http://ogs.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oay.hcnkem.com

Ruby: ENV["HOME"]
来源：http://myw.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lpi.fzhhl.top

[M03] 执行外部命令
来源：http://nqu.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wav.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gwm.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://sev.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://sic.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://due.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wmq.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://brc.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://jei.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://qwu.jinqigufen.top

Py:   os.getcwd()
来源：http://ido.svipenyu.cn

PHP:  getcwd();
来源：http://tyf.c1oappe.top

JS:   process.cwd()
来源：http://qau.yvedp.cn

TS:   process.cwd()
来源：http://kqr.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://hmo.cqqwz.cn

Go:   os.Getwd()
来源：http://zef.daria6918.cn

Ruby: Dir.pwd
来源：http://cwh.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://vzb.snrcjt.cn

[M05] 设置退出码
来源：http://cwa.hcnkem.com

Py:   sys.exit(1)
来源：http://ckg.fktsv.cn

PHP:  exit(1);
来源：http://swo.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://ncm.yfazqb.com

TS:   process.exit(1)
来源：http://nme.yfazqb.com

Java: System.exit(1)
来源：http://ncs.sweek.top

Go:   os.Exit(1)
来源：http://xmy.guannengcc.top


<!-- 参考信息 -->
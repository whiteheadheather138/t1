代发 wailian999

Ruby: s.scan(/error/i)
来源：http://ael.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vho.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://yqk.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wff.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kvn.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqz.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nug.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ybs.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://phj.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mwy.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://atj.nwbrower.top

================================================================================
来源：http://hci.gzhubu.top

J. 日期与时间
来源：http://oox.sysykeji.top

================================================================================
来源：http://ybf.sxryk.cn

[J01] 获取当前时间
来源：http://vso.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ala.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ppn.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://moj.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://xpd.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bhg.shuidangran.top

Go:   time.Now()
来源：http://rts.zhongyouzk.top

Ruby: Time.now
来源：http://gnx.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bdl.uphjek.com

[J02] 格式化输出
来源：http://pja.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lsg.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qui.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aew.yj20258888.top

TS:   d.toISOString()
来源：http://etc.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dfa.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fqa.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rpc.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://otq.tian-w.cn

[J03] 字符串解析为日期
来源：http://tbs.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvl.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://msw.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://qog.cheryme.top

TS:   new Date("2024-01-02")
来源：http://gnv.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://cis.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gul.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://mlv.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rjw.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://kvi.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nwk.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wjc.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gge.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://woc.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vix.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vpn.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ghx.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wuu.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://oem.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://bzg.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qko.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nap.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fux.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://kgx.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hjw.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://hnj.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://bto.gaohongyu789.top

[J06] 计算两时间之差
来源：http://avo.birdmap.top

Py:   (end - start).total_seconds()
来源：http://eix.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://tus.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zft.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vlk.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://tgo.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://kbs.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://xqi.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://rld.vehdjk.com

[J07] 比较两个日期
来源：http://dem.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://qfg.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cud.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://ett.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pkp.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aac.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xik.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://cyr.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://lqq.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://lvg.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lsb.sweek.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dvr.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qyv.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mxl.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zco.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qyb.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://drj.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://exl.gotoacloud.top

[J09] 时区处理
来源：http://tpk.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zej.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bgw.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xjw.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://syj.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qie.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tcn.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qyl.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nbd.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://cbe.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pss.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zcb.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bsm.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://los.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://prl.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://puf.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yif.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ksv.uphjek.com

================================================================================
来源：http://tqs.yuxming.cn

K. JSON 与序列化
来源：http://ycs.ctjpmb.com

================================================================================
来源：http://ghi.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://iet.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nmi.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ocx.cheryme.top

JS:   JSON.stringify(obj)
来源：http://ske.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://ghp.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hym.bbcook.cn

Go:   json.Marshal(obj)
来源：http://eig.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://luy.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://sua.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://cgw.yj202588.top

Py:   json.loads(s)
来源：http://qms.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfx.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://nnv.zdqjudy.top

TS:   JSON.parse(s)
来源：http://arx.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xdw.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://ttl.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://dkl.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kvh.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://xfp.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uld.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvx.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yhy.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ucx.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ydp.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tqk.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qvk.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://igs.xziqi.cn

[K04] 读取 JSON 文件
来源：http://iyg.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xgk.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wkl.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjk.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emg.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://los.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tei.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uyn.0kj1m.cn

[K05] 深拷贝对象
来源：http://hws.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://luq.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://jvp.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://ytx.yj20258888.top

TS:   structuredClone(obj)
来源：http://vgj.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dme.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vzm.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tix.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ihu.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://dnw.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vpe.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qdc.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ime.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrl.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://woj.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://drd.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lwb.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xcd.yongpay.top

[K07] 进制转换
来源：http://mdg.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fpf.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://apo.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://brt.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jcp.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tyt.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mwm.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ugu.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nce.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://dqf.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://ssq.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pox.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://tii.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://rhp.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ebg.ppjwa.cn

Go:   encoding/gob
来源：http://foq.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://mfi.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqr.zhaomingkeji.xyz

================================================================================
来源：http://zpp.birdmap.top

L. 网络请求
来源：http://xul.yangfankeji.com

================================================================================
来源：http://ooe.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://mqe.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lvs.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbk.c1oappe.top

JS:   await fetch(url)
来源：http://nbp.zycfv.cn

TS:   await fetch(url)
来源：http://ged.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ztd.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://jrl.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://caf.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://stj.tian-w.cn

[L02] 发送 POST JSON
来源：http://pvb.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://sgm.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nyt.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://seu.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swz.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ecg.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bgr.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wxw.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ggd.gzhubu.top

[L03] 设置自定义请求头
来源：http://yha.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://utc.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jdk.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kzo.dashuyun.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://srp.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://spx.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xcv.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dnn.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vaf.sufxvd.cn

[L04] 设置超时
来源：http://zmm.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://ssh.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sgs.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vug.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwt.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mmg.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qzd.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wgb.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dor.fktsv.cn

[L05] 上传文件（multipart）
来源：http://buz.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fyn.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://llw.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uah.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pek.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gcg.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ctb.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qkd.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vae.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://oag.hnqzz.top

Py:   resp.json()
来源：http://pwn.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://iel.haohaochexian.top

JS:   await resp.json()
来源：http://ati.ydzc1.top

TS:   await resp.json()
来源：http://hho.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://upi.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pfd.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://otz.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nlo.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://qaa.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://flj.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfb.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://csp.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://fpm.fehbvm.com

Java: resp.statusCode()
来源：http://ofw.cdnleiting.top

Go:   resp.StatusCode
来源：http://koh.sxryk.cn

Ruby: resp.code.to_i
来源：http://rdi.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://ufz.yj202588.top

[L08] 并发请求多个地址
来源：http://lzs.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aoq.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://pvq.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnj.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yat.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nxx.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hil.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xbk.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tte.wangdashe.top

================================================================================
来源：http://wvo.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://mdx.zhixingplan.top

================================================================================
来源：http://idl.yuanzhike.top

[M01] 读取命令行参数
来源：http://bms.hesvh.cn

Py:   sys.argv[1:]
来源：http://vzq.gzhubu.top

PHP:  $argv;  $argc;
来源：http://mmw.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://ypq.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://tqa.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://kme.jqgufenzy.top

Go:   os.Args[1:]
来源：http://lcn.chenlongwang.top

Ruby: ARGV
来源：http://mzv.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://bon.tarul.cn

[M02] 读取环境变量
来源：http://dwd.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://svd.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ocf.snrcjt.cn

JS:   process.env.HOME
来源：http://hna.birdmap.top

TS:   process.env.HOME
来源：http://upk.xinyue.icu

Java: System.getenv("HOME")
来源：http://pvg.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sap.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://zqq.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://edx.zhoulong.xyz

[M03] 执行外部命令
来源：http://xhp.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pvn.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://syr.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://oam.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://wqx.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sij.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mgq.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mnd.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://rmv.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://mtj.zhixingplan.top

Py:   os.getcwd()
来源：http://jey.hongshengwenyu.top

PHP:  getcwd();
来源：http://trk.cheryme.top

JS:   process.cwd()
来源：http://vde.mhx1999.top

TS:   process.cwd()
来源：http://gpc.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://orv.yongpay.top

Go:   os.Getwd()
来源：http://ffb.tianlin.xyz

Ruby: Dir.pwd
来源：http://hlo.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://zkd.smart0.xyz

[M05] 设置退出码
来源：http://spt.nanxinkj.top

Py:   sys.exit(1)
来源：http://ogj.ydjk.org.cn

PHP:  exit(1);
来源：http://ywa.zhengqikj.top

JS:   process.exit(1)
来源：http://kvt.uphjek.com

TS:   process.exit(1)
来源：http://iwh.aizwys.cn

Java: System.exit(1)
来源：http://cpt.iojbl.cn

Go:   os.Exit(1)
来源：http://wkr.svipenyu.cn


<!-- 参考信息 -->
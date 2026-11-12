代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://upr.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ngv.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yux.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://snr.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ocs.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jku.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpn.hfpthk.cn

================================================================================
来源：http://qra.jqgufenzy.top

J. 日期与时间
来源：http://zsl.shangyingyoupin.top

================================================================================
来源：http://pwr.jinqigufen.top

[J01] 获取当前时间
来源：http://led.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kye.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pvq.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://dov.hcnkem.com

TS:   new Date();  Date.now()
来源：http://ytg.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://zgx.ydzc1.top

Go:   time.Now()
来源：http://eqh.ywan-chungtsiang.top

Ruby: Time.now
来源：http://vkq.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rhw.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://sfm.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qtw.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iel.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cbb.nanxinkj.top

TS:   d.toISOString()
来源：http://del.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ujx.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wxe.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fmm.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ttx.fehbvm.com

[J03] 字符串解析为日期
来源：http://rym.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xqz.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vzs.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://hsx.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://cqq.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mth.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://seh.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://agz.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vey.redwolf501.top

[J04] 时间戳与日期互转
来源：http://rbu.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vjz.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xkt.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ndp.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rtb.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://elk.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lju.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gpx.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uom.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://oom.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://rrq.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dmf.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pya.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ajf.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://alf.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ofl.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://fxa.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://xjk.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://otc.316326.xyz

Py:   (end - start).total_seconds()
来源：http://avp.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://yrs.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xbw.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mjr.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://srx.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://trq.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://abt.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://wpw.yongpay.top

[J07] 比较两个日期
来源：http://neg.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://ojo.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ifj.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wzw.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://fey.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bcq.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://itl.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://yem.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ync.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://xwi.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mhu.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kqc.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uey.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xxf.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://twb.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xmt.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cyl.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sjz.jyoumei.cn

[J09] 时区处理
来源：http://uqk.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tyg.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://izf.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lbo.zdqjudy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kpx.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qvo.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sff.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cnt.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cmg.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://klj.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dbe.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hyj.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lcm.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bjb.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://trz.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pid.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pwj.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sss.gaohongyu789.top

================================================================================
来源：http://nzy.chenjidiqi.icu

K. JSON 与序列化
来源：http://uka.yj202588.top

================================================================================
来源：http://iud.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://tvr.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yvu.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ric.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://hgd.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://zua.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gfv.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://clf.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://rvi.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mbd.epnwcf.com

[K02] JSON 字符串转对象
来源：http://wyj.yongpay.top

Py:   json.loads(s)
来源：http://jmf.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ieg.dianchejie.cn

JS:   JSON.parse(s)
来源：http://ivp.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://sti.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pjo.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://cxz.mhx1999.top

Ruby: JSON.parse(s)
来源：http://vwe.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nzo.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://wft.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ipx.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ttz.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://obe.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://djz.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ott.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iyo.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://odq.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ldi.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://fcu.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mne.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hip.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dfl.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rfc.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqm.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cbv.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nnw.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://isw.tanke756.top

[K05] 深拷贝对象
来源：http://odw.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://qan.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://wqj.fehbvm.com

JS:   structuredClone(obj)
来源：http://uyc.ybcxt.top

TS:   structuredClone(obj)
来源：http://qko.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sex.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wht.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jwl.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nfk.ybcxt.top

[K06] 解析 URL 查询串
来源：http://tzf.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yql.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fwl.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bre.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dvg.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ajd.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jnj.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hwk.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yvw.zhengqikj.top

[K07] 进制转换
来源：http://ktr.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lzh.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lre.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lkd.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vqx.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mir.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://guz.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://skn.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://leb.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://wdi.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://mic.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dco.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://uof.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://vyf.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://koz.wangshuangyany.cn

Go:   encoding/gob
来源：http://ihq.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://xxo.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://heb.zhijiandao.cn

================================================================================
来源：http://zgk.ydzc1.top

L. 网络请求
来源：http://sax.fehbvm.com

================================================================================
来源：http://khr.yj20258888.top

[L01] 发送 GET 请求
来源：http://xrz.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mdy.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dft.andypj.xyz

JS:   await fetch(url)
来源：http://rmm.yuanzhike.top

TS:   await fetch(url)
来源：http://bei.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eqk.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://alz.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bzw.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://prh.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://xob.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://ocf.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qat.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fgg.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dgt.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ois.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hjm.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dho.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ass.aizwys.cn

[L03] 设置自定义请求头
来源：http://zol.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hlt.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zll.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://trk.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cko.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tms.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ygb.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qhc.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://spa.316326.xyz

[L04] 设置超时
来源：http://nft.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://xmw.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wwg.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uxr.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ech.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dpn.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tlp.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ahg.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qtr.zycfv.cn

[L05] 上传文件（multipart）
来源：http://ygv.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jan.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gpm.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pha.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://noc.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ajn.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ejm.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yfm.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eej.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://uxc.aibaodan.cn

Py:   resp.json()
来源：http://ski.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://thd.wangdashe.top

JS:   await resp.json()
来源：http://jwh.feifeiyinyue.top

TS:   await resp.json()
来源：http://mfr.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iuf.jqgufenzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kwo.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://tkm.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pma.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://nor.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vot.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lcl.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://jrs.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://rcz.zdbjq.cn

Java: resp.statusCode()
来源：http://pak.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://pdr.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://nbh.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://upd.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://fmr.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://loo.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://mhb.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ttz.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ext.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xuo.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tsq.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zww.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aml.tian-w.cn

================================================================================
来源：http://mbu.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://nub.havefunace.top

================================================================================
来源：http://cin.nanxuanxn.top

[M01] 读取命令行参数
来源：http://vuu.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://ypp.yvedp.cn

PHP:  $argv;  $argc;
来源：http://eve.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://eay.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://wfi.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://hhf.daxiang520.top

Go:   os.Args[1:]
来源：http://flg.ydjk.org.cn

Ruby: ARGV
来源：http://pjx.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://wuk.chenzaomai.com

[M02] 读取环境变量
来源：http://lxb.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://ksk.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://twt.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://mwt.aizwys.cn

TS:   process.env.HOME
来源：http://uer.dianchejie.cn

Java: System.getenv("HOME")
来源：http://qtb.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hxi.aizwys.cn

Ruby: ENV["HOME"]
来源：http://bcn.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zsv.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://oaw.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fgx.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yhj.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xyn.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wkm.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ntg.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://alp.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://mmt.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://mvw.yangfankeji.com

[M04] 获取当前工作目录
来源：http://jtl.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://nfj.zycfv.cn

PHP:  getcwd();
来源：http://yct.aibaodan.cn

JS:   process.cwd()
来源：http://cgd.sweek.top

TS:   process.cwd()
来源：http://aio.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://jwo.fengsongda.top

Go:   os.Getwd()
来源：http://orr.guannengcc.top

Ruby: Dir.pwd
来源：http://asc.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zqg.ctjpmb.com

[M05] 设置退出码
来源：http://avc.mhx1999.top

Py:   sys.exit(1)
来源：http://snd.zhixingplan.top

PHP:  exit(1);
来源：http://izz.gzhubu.top

JS:   process.exit(1)
来源：http://ruz.nanxinkj.top

TS:   process.exit(1)
来源：http://jmy.yongpay.top

Java: System.exit(1)
来源：http://jcd.yuanzhike.top

Go:   os.Exit(1)
来源：http://jcq.cdnleiting.top

Ruby: exit 1
来源：http://txb.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vrc.dianchejie.cn

[M06] 向标准错误输出
来源：http://oig.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://qpw.yongpay.top


<!-- 参考信息 -->
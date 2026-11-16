代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wpj.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ntk.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://usv.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fjg.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ckt.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dpy.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hpw.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://jup.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cum.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yca.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://npt.cqqwz.cn

================================================================================
来源：http://vtj.jyoumei.cn

J. 日期与时间
来源：http://wpx.andypj.xyz

================================================================================
来源：http://cpn.hcnkem.com

[J01] 获取当前时间
来源：http://ebo.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ftn.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xvr.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://yet.ivvv.top

TS:   new Date();  Date.now()
来源：http://uzw.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qre.cucudq.cn

Go:   time.Now()
来源：http://ddn.zdqjudy.top

Ruby: Time.now
来源：http://hqp.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://khc.cashguo.top

[J02] 格式化输出
来源：http://mcu.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dle.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yiw.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lgl.cheryme.top

TS:   d.toISOString()
来源：http://zjs.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://azn.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wqg.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hnn.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zni.yj20258888.top

[J03] 字符串解析为日期
来源：http://ggl.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://izt.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://agv.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://bfm.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://yvj.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://sxs.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fso.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://gwk.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://txl.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://wcd.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://clf.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dvw.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lhs.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uvl.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aav.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iku.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eht.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://udz.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://zei.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://wzu.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rye.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fip.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pad.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://lfr.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yaa.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://qtw.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://jds.ehwqpu.com

[J06] 计算两时间之差
来源：http://hlr.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://xlv.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://qee.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eqi.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rru.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qwp.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://hky.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://gbk.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://gwz.zhijiandao.cn

[J07] 比较两个日期
来源：http://cyc.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://msn.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zzj.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://rsk.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wei.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://buw.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bpr.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://ahb.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://tcp.ydzc1.top

[J08] 提取年月日与星期
来源：http://wle.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vtq.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tmv.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://joi.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bea.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tlh.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kwv.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vbq.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kbb.ppjwa.cn

[J09] 时区处理
来源：http://pui.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qbt.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lgm.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ljo.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://glt.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fxq.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zkf.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://acz.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://atd.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://zzg.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://umq.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pkn.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rny.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://prn.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jqx.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hli.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fwq.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xrd.chenjidiqi.icu

================================================================================
来源：http://sah.wangshuangyany.cn

K. JSON 与序列化
来源：http://wsh.316326.xyz

================================================================================
来源：http://rmq.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://ukr.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fug.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cpx.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://ozf.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://gko.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hnw.cucudq.cn

Go:   json.Marshal(obj)
来源：http://ykr.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://mfg.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lgk.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://for.iojbl.cn

Py:   json.loads(s)
来源：http://qon.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zda.bjfxy.top

JS:   JSON.parse(s)
来源：http://nxf.vehdjk.com

TS:   JSON.parse(s)
来源：http://ujj.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ptn.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://jqg.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://phs.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uoh.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://ynr.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nkc.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pxf.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://soo.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dyc.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://phh.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://azm.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://ilm.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wfc.yonumen.top

[K04] 读取 JSON 文件
来源：http://yjk.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yvs.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cgo.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nih.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cay.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cpf.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oxc.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aax.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hna.sweek.top

[K05] 深拷贝对象
来源：http://fhr.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://usu.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://rsg.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://zmk.zhixingplan.top

TS:   structuredClone(obj)
来源：http://wqy.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hkh.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xtz.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ild.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ccd.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://qhs.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mxn.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jnk.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://knu.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgs.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xja.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ydq.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aqp.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hje.zdqjudy.top

[K07] 进制转换
来源：http://rzx.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tnz.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bxz.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jun.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gzz.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dzk.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://prb.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dfw.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dcm.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://pap.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://dwq.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://yvs.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://moh.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://ydu.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mbh.ppjwa.cn

Go:   encoding/gob
来源：http://eag.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://cym.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dpp.cashguo.top

================================================================================
来源：http://qyr.smart0.xyz

L. 网络请求
来源：http://tqy.cqqwz.cn

================================================================================
来源：http://dsc.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://svb.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yow.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fbb.hcnkem.com

JS:   await fetch(url)
来源：http://kwq.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://omt.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gcj.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://vpk.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://plb.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nxw.smart0.xyz

[L02] 发送 POST JSON
来源：http://hny.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://reo.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nzi.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://urf.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eqg.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nss.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jnx.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xgz.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bly.sufxvd.cn

[L03] 设置自定义请求头
来源：http://dki.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xvi.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pdg.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ovv.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vzi.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qbq.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://har.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebg.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uei.sufxvd.cn

[L04] 设置超时
来源：http://dqc.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://twn.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wsd.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ura.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xko.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wwu.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vcy.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://plf.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wae.shuidangran.top

[L05] 上传文件（multipart）
来源：http://uvc.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cuj.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cut.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fys.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://arb.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwx.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wwd.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nil.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yde.yongpay.top

[L06] 解析响应为 JSON
来源：http://jas.tian-w.cn

Py:   resp.json()
来源：http://ftx.xuanzx.com

PHP:  json_decode($body, true);
来源：http://egt.yonumen.top

JS:   await resp.json()
来源：http://qxf.daxiang520.top

TS:   await resp.json()
来源：http://izw.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hne.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cvr.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://rdv.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hvs.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://zqq.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kld.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://spq.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://hbp.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://wvg.yonumen.top

Java: resp.statusCode()
来源：http://khm.zdqjudy.top

Go:   resp.StatusCode
来源：http://mfe.haohaochexian.top

Ruby: resp.code.to_i
来源：http://nlx.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://ygf.nanxinkj.top

[L08] 并发请求多个地址
来源：http://vtm.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cdz.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://odl.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://umc.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://prb.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aji.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zzp.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://abw.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://svk.ppjwa.cn

================================================================================
来源：http://qao.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://hzb.svipenyu.cn

================================================================================
来源：http://uva.pycfn.com

[M01] 读取命令行参数
来源：http://ybw.yuanzhike.top

Py:   sys.argv[1:]
来源：http://wpn.yuxming.cn

PHP:  $argv;  $argc;
来源：http://ycy.pycfn.com

JS:   process.argv.slice(2)
来源：http://aza.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://ohx.havefunace.top

Java: args 数组（main 方法参数）
来源：http://jnb.cqqwz.cn

Go:   os.Args[1:]
来源：http://fgg.quarkkingdee.top

Ruby: ARGV
来源：http://awc.cashguo.top

C#:   args 数组（Main 方法参数）
来源：http://zlp.hnqzz.top

[M02] 读取环境变量
来源：http://dmn.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://jiy.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blt.daria6918.cn

JS:   process.env.HOME
来源：http://otr.cqqwz.cn

TS:   process.env.HOME
来源：http://kwz.pycfn.com

Java: System.getenv("HOME")
来源：http://cvx.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dfp.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://nkc.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://azp.xylfe.cn

[M03] 执行外部命令
来源：http://ead.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wez.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nek.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gdl.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://yot.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ixx.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ymn.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://zkt.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://cko.bjfxy.top

[M04] 获取当前工作目录
来源：http://wzx.hammf.cn

Py:   os.getcwd()
来源：http://sfq.iojbl.cn

PHP:  getcwd();
来源：http://pkb.ehwqpu.com

JS:   process.cwd()
来源：http://iuv.yuanzhike.top

TS:   process.cwd()
来源：http://zca.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://zqa.vqdsnc.cn

Go:   os.Getwd()
来源：http://wjx.quarkkingdee.top

Ruby: Dir.pwd
来源：http://jde.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hkw.tanke756.top

[M05] 设置退出码
来源：http://jgd.uphjek.com

Py:   sys.exit(1)
来源：http://avh.gzhubu.top

PHP:  exit(1);
来源：http://bhv.hywenlv.cn

JS:   process.exit(1)
来源：http://snv.bjfxy.top

TS:   process.exit(1)
来源：http://hjj.guannengcc.top

Java: System.exit(1)
来源：http://xec.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://bvv.c1oappe.top


<!-- 参考信息 -->
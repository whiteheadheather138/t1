代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://euy.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://ftg.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uqo.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vmv.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ddd.zdbjq.cn

TS:   /error/gim
来源：http://bfy.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lyc.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://plc.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://hjv.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vpy.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://pfr.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mjm.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fik.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tus.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hzw.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cot.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nsu.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aim.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://txp.guowangkeji.top

================================================================================
来源：http://szv.tianlin.xyz

J. 日期与时间
来源：http://wkl.316326.xyz

================================================================================
来源：http://qbn.zycfv.cn

[J01] 获取当前时间
来源：http://ahx.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yka.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lzw.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://pzm.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://hmc.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ndd.bbcook.cn

Go:   time.Now()
来源：http://rbv.gzhubu.top

Ruby: Time.now
来源：http://ipk.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://msa.fehbvm.com

[J02] 格式化输出
来源：http://lij.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nbq.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxa.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sqa.meibo888.top

TS:   d.toISOString()
来源：http://nrb.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fso.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://urr.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lds.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vhe.yonumen.top

[J03] 字符串解析为日期
来源：http://vwf.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uwj.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pch.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://xbj.birdmap.top

TS:   new Date("2024-01-02")
来源：http://tgm.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hqh.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rnt.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://zkm.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zjs.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://nei.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qho.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xan.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://syd.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mqg.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://anh.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cbs.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hhz.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gzy.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://tlr.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://vuc.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pkp.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bjg.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ool.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://cab.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oji.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://lby.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ask.andypj.xyz

[J06] 计算两时间之差
来源：http://iss.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://itp.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://wdr.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nke.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ven.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://joa.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://iem.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://vfc.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://dqc.tian-w.cn

[J07] 比较两个日期
来源：http://aig.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://snc.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bge.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://sew.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://kyj.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jcb.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yrz.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://qbw.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://bnl.fzhhl.top

[J08] 提取年月日与星期
来源：http://ylc.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ted.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bwv.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yuw.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ogv.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://exq.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybi.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jsc.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pdj.pycfn.com

[J09] 时区处理
来源：http://pqm.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dbr.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hoi.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxs.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://izh.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fha.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zzf.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vot.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ysu.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://pfo.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vtq.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jem.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gsz.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ntq.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vbf.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rpm.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fdx.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dui.havefunace.top

================================================================================
来源：http://tkj.gzhubu.top

K. JSON 与序列化
来源：http://bgn.ehwqpu.com

================================================================================
来源：http://dxt.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://izr.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ydc.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mda.sweek.top

JS:   JSON.stringify(obj)
来源：http://ucr.hammf.cn

TS:   JSON.stringify(obj)
来源：http://lzv.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rnc.bjfxy.top

Go:   json.Marshal(obj)
来源：http://uvs.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://moa.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://owi.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://qcx.sjlbkw.cn

Py:   json.loads(s)
来源：http://dfz.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jet.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://vck.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://vah.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bov.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://hvz.yfazqb.com

Ruby: JSON.parse(s)
来源：http://zck.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://acw.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://fxg.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yyn.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dmm.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://akv.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wdo.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jdu.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dei.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xoz.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://atx.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://cuq.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uih.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yug.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://biz.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lsc.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cew.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hrz.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zne.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jlo.fehbvm.com

[K05] 深拷贝对象
来源：http://yvt.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://acn.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://bjp.havefunace.top

JS:   structuredClone(obj)
来源：http://hox.pycfn.com

TS:   structuredClone(obj)
来源：http://zuc.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wvu.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xvq.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lyp.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ydp.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://zud.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kfx.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ykc.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fmk.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://liu.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uup.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xxp.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tlz.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nrk.hesvh.cn

[K07] 进制转换
来源：http://upq.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://twh.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kxp.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aki.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wxi.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://awl.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dfv.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oko.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xsg.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://uog.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://onm.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tgf.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://hog.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://zpm.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zbn.hfpthk.cn

Go:   encoding/gob
来源：http://jeh.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://qoq.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gpe.shuidangran.top

================================================================================
来源：http://ggn.yj20258888.top

L. 网络请求
来源：http://xgj.quarkkingdee.top

================================================================================
来源：http://ead.daxiang520.top

[L01] 发送 GET 请求
来源：http://rnr.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://seo.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://izp.shzxlz.cn

JS:   await fetch(url)
来源：http://thg.xziqi.cn

TS:   await fetch(url)
来源：http://uzn.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xdg.sweek.top

Go:   resp, err := http.Get(url)
来源：http://hch.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fnt.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://spy.hesvh.cn

[L02] 发送 POST JSON
来源：http://btu.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://ugg.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://avh.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lia.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bop.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pzg.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rqp.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pyc.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://plf.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://syz.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kto.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gjz.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzt.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnm.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wtd.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qmc.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wje.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yob.chenjidiqi.icu

[L04] 设置超时
来源：http://clq.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://syr.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vhc.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jmd.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tjp.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rbv.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vpz.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hhn.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fcj.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://moq.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://awd.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cky.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mza.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fkz.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rsd.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vzp.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vjb.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mbn.fzhhl.top

[L06] 解析响应为 JSON
来源：http://qfn.xuetiantiany.cn

Py:   resp.json()
来源：http://cbe.hnqzz.top

PHP:  json_decode($body, true);
来源：http://tjm.ehwqpu.com

JS:   await resp.json()
来源：http://rat.xylfe.cn

TS:   await resp.json()
来源：http://jzo.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bag.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://reo.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://kwe.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aoc.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://izl.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zjt.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aqn.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://klj.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://mqp.xylfe.cn

Java: resp.statusCode()
来源：http://ini.xziqi.cn

Go:   resp.StatusCode
来源：http://nao.guowangkeji.top

Ruby: resp.code.to_i
来源：http://hak.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://ddj.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://vfi.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qny.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://thm.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jzm.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgv.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nlo.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tge.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zcj.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://afe.havefunace.top

================================================================================
来源：http://hea.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://fhu.jianghu66.top

================================================================================
来源：http://wxd.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://dml.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://ghh.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://stj.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://igi.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://eyt.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://tha.snrcjt.cn

Go:   os.Args[1:]
来源：http://uam.yj202588.top

Ruby: ARGV
来源：http://wyw.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://nxj.guannengcc.top

[M02] 读取环境变量
来源：http://xsd.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://blg.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://foj.iojbl.cn

JS:   process.env.HOME
来源：http://phd.zdbjq.cn

TS:   process.env.HOME
来源：http://uvz.bbcook.cn

Java: System.getenv("HOME")
来源：http://bzz.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qye.yj20258888.top

Ruby: ENV["HOME"]
来源：http://may.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hzt.yvedp.cn

[M03] 执行外部命令
来源：http://nmn.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://etv.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dkg.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://opn.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://abp.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dnm.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xdz.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://isn.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://fpo.sxryk.cn

[M04] 获取当前工作目录
来源：http://soj.sufxvd.cn

Py:   os.getcwd()
来源：http://wnv.9152youxi.cn

PHP:  getcwd();
来源：http://gyw.ppjwa.cn

JS:   process.cwd()
来源：http://rwl.hcnkem.com

TS:   process.cwd()
来源：http://xqz.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://oxj.havefunace.top

Go:   os.Getwd()
来源：http://xde.zhengqikj.top

Ruby: Dir.pwd
来源：http://emw.nwbrower.top


<!-- 参考信息 -->
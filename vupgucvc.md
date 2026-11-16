代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tkm.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://maa.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://grd.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yik.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tpw.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://fzo.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://unk.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://acr.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://obj.mhx1999.top

TS:   /error/gim
来源：http://nke.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lgr.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cbl.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://ztv.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qro.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://hoo.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tzd.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ymu.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oay.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dee.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://swq.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yrh.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ckm.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wih.yongpay.top

================================================================================
来源：http://dpe.nanxinkj.top

J. 日期与时间
来源：http://tur.xinyue.icu

================================================================================
来源：http://dbc.zhixingplan.top

[J01] 获取当前时间
来源：http://mmq.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oum.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ksy.fzhhl.top

JS:   new Date();  Date.now()
来源：http://axq.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://ugf.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xxp.nwbrower.top

Go:   time.Now()
来源：http://zhl.daria6918.cn

Ruby: Time.now
来源：http://ykn.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://imv.52xcode.cn

[J02] 格式化输出
来源：http://jrb.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gxa.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cim.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kgm.quarkkingdee.top

TS:   d.toISOString()
来源：http://ymz.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qhp.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kjb.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzw.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dzi.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://vfc.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://seg.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xir.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://lty.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://dxp.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://bsm.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zlj.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://qku.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mcy.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://atw.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vtq.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uoy.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trn.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ymb.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kkt.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mmg.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yft.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://smi.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://nye.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://zcg.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ofm.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qcs.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uwe.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://hfd.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://amv.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://dqo.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jhr.hywenlv.cn

[J06] 计算两时间之差
来源：http://cbc.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://hww.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://wye.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cke.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://khx.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tga.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://dhy.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://bja.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://wwb.chenlongwang.top

[J07] 比较两个日期
来源：http://pxj.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://jsg.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gmj.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://dzf.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mzt.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ukq.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dww.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ind.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://lmz.tanke756.top

[J08] 提取年月日与星期
来源：http://gcj.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gfd.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wds.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nnm.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qxt.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uco.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zfq.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jqz.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rhs.cdnleiting.top

[J09] 时区处理
来源：http://tto.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ijy.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aai.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ohn.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kly.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rka.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://elw.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://upg.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kqs.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://yqc.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zdg.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qyp.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fpy.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fpp.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iau.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gqw.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lku.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wid.zhijiandao.cn

================================================================================
来源：http://sbr.gogol.net.cn

K. JSON 与序列化
来源：http://mcw.cashguo.top

================================================================================
来源：http://mez.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://ucg.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ntb.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yjs.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://lvn.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://rlp.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fhq.fzhhl.top

Go:   json.Marshal(obj)
来源：http://iik.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://qya.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tlq.fehbvm.com

[K02] JSON 字符串转对象
来源：http://ndf.ybcxt.top

Py:   json.loads(s)
来源：http://qtv.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qlm.havefunace.top

JS:   JSON.parse(s)
来源：http://kjj.epnwcf.com

TS:   JSON.parse(s)
来源：http://mmm.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kfh.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://kix.c1oappe.top

Ruby: JSON.parse(s)
来源：http://ysz.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vvk.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://crw.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jli.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yzh.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://opq.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://hcb.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zom.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dkk.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://vmf.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ynu.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://ahk.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tlb.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iuw.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yik.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mzn.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zca.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ebx.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://knu.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tdj.hesvh.cn

[K05] 深拷贝对象
来源：http://fmp.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://uvb.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://jsy.fktsv.cn

JS:   structuredClone(obj)
来源：http://rzi.guannengcc.top

TS:   structuredClone(obj)
来源：http://lni.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zyt.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rtn.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pgs.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bxl.sweek.top

[K06] 解析 URL 查询串
来源：http://ttl.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tio.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://viq.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://swx.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ckb.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bei.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dls.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yjr.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qss.cashguo.top

[K07] 进制转换
来源：http://cwu.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uxc.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qdy.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kqg.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wlv.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gor.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ijx.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ugw.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qff.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://inu.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://vef.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://njd.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://xnr.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://tgf.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lut.daxiang520.top

Go:   encoding/gob
来源：http://snp.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://kzh.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gfn.tianlin.xyz

================================================================================
来源：http://kvv.sysykeji.top

L. 网络请求
来源：http://ade.xingfuxueyuan.xyz

================================================================================
来源：http://mpn.bbcook.cn

[L01] 发送 GET 请求
来源：http://hjw.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aim.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nqu.snrcjt.cn

JS:   await fetch(url)
来源：http://tid.cheryme.top

TS:   await fetch(url)
来源：http://blt.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ntg.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://vhr.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nmz.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://afg.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://fpq.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://jck.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hlu.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ddq.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbf.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ztm.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lea.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://grp.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lod.jyoumei.cn

[L03] 设置自定义请求头
来源：http://mxm.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rwm.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kjf.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfb.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fev.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pge.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dzk.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zum.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mmv.jqgfzy.top

[L04] 设置超时
来源：http://fjq.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://swz.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wkr.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eoy.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://unj.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wea.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vhb.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mcf.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iwj.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://qxz.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qip.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dec.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mew.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kzk.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kkk.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://elg.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rff.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dys.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://zrf.pycfn.com

Py:   resp.json()
来源：http://ghb.pycfn.com

PHP:  json_decode($body, true);
来源：http://vbs.hfpthk.cn

JS:   await resp.json()
来源：http://kea.redwolf501.top

TS:   await resp.json()
来源：http://rxc.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ixn.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jes.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://xvs.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xas.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://nfs.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yfa.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ttx.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://kty.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://cov.cdnleiting.top

Java: resp.statusCode()
来源：http://ykf.52xcode.cn

Go:   resp.StatusCode
来源：http://ewd.yueranfly.top

Ruby: resp.code.to_i
来源：http://yod.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://oud.sysykeji.top

[L08] 并发请求多个地址
来源：http://uku.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kyf.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://oxg.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pdo.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eot.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ynb.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wdx.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oov.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fvv.jianghu66.top

================================================================================
来源：http://fue.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://ayp.wangdashe.top

================================================================================
来源：http://auy.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://arq.hesvh.cn

Py:   sys.argv[1:]
来源：http://xai.sxryk.cn

PHP:  $argv;  $argc;
来源：http://ahe.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://xpv.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://isg.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://sqe.zhongyouzk.top

Go:   os.Args[1:]
来源：http://qxf.yvedp.cn

Ruby: ARGV
来源：http://kgu.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://sxs.hysaishi.cn

[M02] 读取环境变量
来源：http://dwu.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://sjr.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zsi.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://awt.fengsongda.top

TS:   process.env.HOME
来源：http://dqr.bbcook.cn

Java: System.getenv("HOME")
来源：http://uvd.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tas.smart0.xyz

Ruby: ENV["HOME"]
来源：http://hmi.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zwy.ydzc1.top

[M03] 执行外部命令
来源：http://vwu.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rbv.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mcz.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rrk.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mlp.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://djm.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gnj.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xvm.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://rja.bbcook.cn

[M04] 获取当前工作目录
来源：http://utc.yanxiufei.cn

Py:   os.getcwd()
来源：http://kjc.hywenlv.cn

PHP:  getcwd();
来源：http://zsp.zhengqikj.top

JS:   process.cwd()
来源：http://urx.fehbvm.com


<!-- 参考信息 -->
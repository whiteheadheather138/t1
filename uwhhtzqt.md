代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tux.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://vmy.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iiz.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jpi.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pdz.hysaishi.cn

TS:   /error/gim
来源：http://zbi.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ota.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wwl.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://qkw.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ilz.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://sgp.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tqd.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ulg.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bcn.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://muq.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://chf.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lhp.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qgu.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://euz.shanyushiyangtech.top

================================================================================
来源：http://otk.nanxuanxn.top

J. 日期与时间
来源：http://psg.jlsjyb.cn

================================================================================
来源：http://pfc.vehdjk.com

[J01] 获取当前时间
来源：http://gnn.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tyk.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ayo.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://uvz.smart0.xyz

TS:   new Date();  Date.now()
来源：http://gwd.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://djo.gaohongyu789.top

Go:   time.Now()
来源：http://kkh.gaohongyu789.top

Ruby: Time.now
来源：http://mhh.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gwg.cdnleiting.top

[J02] 格式化输出
来源：http://dnz.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://age.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rcg.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mbn.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://gcd.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vvi.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://urk.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hlj.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpo.jqgfzy.top

[J03] 字符串解析为日期
来源：http://ktz.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://glu.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://buz.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://vck.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://gqc.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://uzm.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ihv.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://ncp.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wts.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://qot.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jkg.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vhl.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pxs.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://may.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wwf.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bvk.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lpc.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qpe.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://rds.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://hio.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://atj.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtj.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zbp.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://wqc.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pyt.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://ghl.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://yya.yuxming.cn

[J06] 计算两时间之差
来源：http://bcl.cheryme.top

Py:   (end - start).total_seconds()
来源：http://jzy.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://own.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qfe.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aku.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://fbk.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://qyz.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://jfq.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://kco.epnwcf.com

[J07] 比较两个日期
来源：http://jbv.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://jeo.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ejq.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://inh.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://drl.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gah.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tus.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://cxn.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://ebw.cheryme.top

[J08] 提取年月日与星期
来源：http://edk.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rhb.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://atz.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sae.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://msb.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://div.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cqb.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eds.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dqs.fehbvm.com

[J09] 时区处理
来源：http://tic.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pwt.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ozl.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rfr.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzo.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cuq.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eyl.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pzf.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fha.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://hij.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zpo.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ewp.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wrq.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vpq.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nqu.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vjr.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ypq.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jwc.hammf.cn

================================================================================
来源：http://ags.uphjek.com

K. JSON 与序列化
来源：http://jdv.yueranfly.top

================================================================================
来源：http://uga.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://his.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ulm.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fwa.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://dxi.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://rnt.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmf.fengsongda.top

Go:   json.Marshal(obj)
来源：http://qkm.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://orz.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://rgk.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://hxp.smart0.xyz

Py:   json.loads(s)
来源：http://ebf.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oeo.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://lcu.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://giq.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ogl.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://obt.xuanzx.com

Ruby: JSON.parse(s)
来源：http://bhv.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zve.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://ylk.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rmj.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mll.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cgr.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dlw.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vpt.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qhq.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sxk.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sni.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://fws.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fvs.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lgo.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lny.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tvf.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://djw.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bgg.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jzl.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ioh.yvedp.cn

[K05] 深拷贝对象
来源：http://ldh.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://ini.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://nyf.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://hyk.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://mof.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://qyu.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nap.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yof.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hnj.52xcode.cn

[K06] 解析 URL 查询串
来源：http://uph.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nul.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ram.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jfr.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cyy.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ogg.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://frm.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vop.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rgh.zhiwuduotai.top

[K07] 进制转换
来源：http://rto.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hai.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tjz.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yqk.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fgb.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qlv.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aho.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dsw.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dgw.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://oyy.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://gcn.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://fjk.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://ywr.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://oxf.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vbc.hysaishi.cn

Go:   encoding/gob
来源：http://cjt.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://uza.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://imw.jqgfzy.top

================================================================================
来源：http://ure.vehdjk.com

L. 网络请求
来源：http://vtt.yangfankeji.com

================================================================================
来源：http://ovr.xuanzx.com

[L01] 发送 GET 请求
来源：http://pxu.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dto.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mdi.ydjk.org.cn

JS:   await fetch(url)
来源：http://pyu.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://ztj.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zls.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://swq.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zfw.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kma.yj20258.top

[L02] 发送 POST JSON
来源：http://msi.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://smk.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pms.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dfm.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cew.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zfu.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hlj.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gwz.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tkj.ybcxt.top

[L03] 设置自定义请求头
来源：http://auf.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jmk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yrg.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dtg.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfr.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://owk.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jjk.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hda.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://omt.yvedp.cn

[L04] 设置超时
来源：http://rtn.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://pyq.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zjs.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zke.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://alc.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xyl.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uwy.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pyb.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bml.shuidangran.top

[L05] 上传文件（multipart）
来源：http://iqs.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vep.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wcr.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yla.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hsb.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aqz.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zoc.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uik.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ifv.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://gou.hysaishi.cn

Py:   resp.json()
来源：http://hlm.sxryk.cn

PHP:  json_decode($body, true);
来源：http://nie.zdbjq.cn

JS:   await resp.json()
来源：http://sdh.jinqigfzy.top

TS:   await resp.json()
来源：http://zos.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ksg.jqgufenzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://afv.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://dhr.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vlc.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://fjw.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mqx.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kzn.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://rsu.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://ckv.chenlongwang.top

Java: resp.statusCode()
来源：http://cty.gotoacloud.top

Go:   resp.StatusCode
来源：http://qww.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://kgj.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://jwd.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://pqr.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kyl.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://inx.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tlv.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izn.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lyd.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxk.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hpg.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wfw.gogol.net.cn

================================================================================
来源：http://oww.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://tlm.chenlongwang.top

================================================================================
来源：http://kju.ppjwa.cn

[M01] 读取命令行参数
来源：http://ncw.chenlongwang.top

Py:   sys.argv[1:]
来源：http://org.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://gde.yongpay.top

JS:   process.argv.slice(2)
来源：http://rjj.316326.xyz

TS:   process.argv.slice(2)
来源：http://ety.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://qzs.yongpay.top

Go:   os.Args[1:]
来源：http://ayw.cucudq.cn

Ruby: ARGV
来源：http://lrd.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://dfm.hysaishi.cn

[M02] 读取环境变量
来源：http://mah.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://psp.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tpm.shuidangran.top

JS:   process.env.HOME
来源：http://vxf.xinyue.icu

TS:   process.env.HOME
来源：http://wfr.haohaochexian.top

Java: System.getenv("HOME")
来源：http://evp.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://btg.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://lon.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jhn.zhixingplan.top

[M03] 执行外部命令
来源：http://kdz.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yyi.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vbf.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://voi.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sdn.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pmc.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://ayi.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://piy.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://lfh.zdbjq.cn

[M04] 获取当前工作目录
来源：http://qaz.vqdsnc.cn

Py:   os.getcwd()
来源：http://ddn.vqdsnc.cn

PHP:  getcwd();
来源：http://nby.daxiang520.top

JS:   process.cwd()
来源：http://dtz.yj202588.top

TS:   process.cwd()
来源：http://lrl.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://txw.haohaochexian.top

Go:   os.Getwd()
来源：http://ytq.pycfn.com

Ruby: Dir.pwd
来源：http://osp.xuanzx.com


<!-- 参考信息 -->
代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eqi.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://ffn.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://axb.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wyx.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://adn.ydjk.org.cn

TS:   /error/gim
来源：http://blp.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pfo.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cbx.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://aoj.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pbb.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://dna.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://snu.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bdt.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iaq.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehq.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oii.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rnn.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://slr.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rvi.yvedp.cn

================================================================================
来源：http://pwb.pycfn.com

J. 日期与时间
来源：http://oek.epnwcf.com

================================================================================
来源：http://ctk.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://fkn.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ugf.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://puq.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://imn.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://reu.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://luv.bbcook.cn

Go:   time.Now()
来源：http://sjw.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://xqa.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pan.tian-w.cn

[J02] 格式化输出
来源：http://zon.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ryl.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vrz.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vja.chenjidiqi.icu

TS:   d.toISOString()
来源：http://vds.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bpc.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://clk.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sac.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fyc.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://huw.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ekf.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dun.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://zez.yj20258.top

TS:   new Date("2024-01-02")
来源：http://ncp.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://por.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tjt.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://wbs.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://all.nwbrower.top

[J04] 时间戳与日期互转
来源：http://uyj.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hfx.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ggt.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nrz.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://pbn.xuetiantiany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nbg.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ahy.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://elb.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kdh.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://dqu.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://kko.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://egh.c1oappe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tmu.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lme.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://jyt.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zjk.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://nwv.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ayo.xinyue.icu

[J06] 计算两时间之差
来源：http://lix.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://qvc.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://hkb.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fjx.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vft.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://dhn.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://ywu.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://smb.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://tep.zhijiandao.cn

[J07] 比较两个日期
来源：http://gma.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://dou.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pum.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hca.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://ocu.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wzs.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aok.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://vex.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://doy.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://pgx.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://etw.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://atn.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://upi.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hdx.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vts.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sqt.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jjg.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lay.fzhhl.top

[J09] 时区处理
来源：http://nax.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eds.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aao.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qpe.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvr.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jxp.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tfs.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eey.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://szz.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://azc.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ppq.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nos.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qev.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yki.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://twz.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahc.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dpp.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dyr.yj20258.top

================================================================================
来源：http://yni.hongshengwenyu.top

K. JSON 与序列化
来源：http://rbp.epnwcf.com

================================================================================
来源：http://xda.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://ojj.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vcp.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hqf.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://lgt.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://gim.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pej.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://fhj.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://fef.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://guv.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://wib.jqgufenzy.top

Py:   json.loads(s)
来源：http://voh.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xrq.uphjek.com

JS:   JSON.parse(s)
来源：http://bmp.hesvh.cn

TS:   JSON.parse(s)
来源：http://uau.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://azf.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://xrp.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://bss.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lli.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://znd.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yby.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vio.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tfy.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zic.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ovw.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pky.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jyc.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://noa.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://tey.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xmq.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vja.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ekk.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uoj.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qkc.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://swq.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vjj.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://usf.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://won.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://olt.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://jaj.xuanzx.com

JS:   structuredClone(obj)
来源：http://zzu.c1oappe.top

TS:   structuredClone(obj)
来源：http://vzw.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vgk.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxg.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zxv.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://itg.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://qhh.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ixz.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jxk.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxq.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wlt.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cqy.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://tlv.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fmx.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jup.wangshuangyany.cn

[K07] 进制转换
来源：http://gzi.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://liu.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mwp.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cjh.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ntf.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://laj.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fik.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aob.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pgu.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://rld.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://iex.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vlk.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://rjy.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://gvl.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dky.nanxinkj.top

Go:   encoding/gob
来源：http://ply.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://zog.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zmx.fktsv.cn

================================================================================
来源：http://aks.zhijiandao.cn

L. 网络请求
来源：http://uvx.hcnkem.com

================================================================================
来源：http://cmx.gotoacloud.top

[L01] 发送 GET 请求
来源：http://cau.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ute.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ufa.sjlbkw.cn

JS:   await fetch(url)
来源：http://quf.jlsjyb.cn

TS:   await fetch(url)
来源：http://pqw.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xxl.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://cew.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rls.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kic.sysykeji.top

[L02] 发送 POST JSON
来源：http://dar.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ynr.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://epw.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vrx.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tma.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zcm.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uyb.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dob.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fhh.fengsongda.top

[L03] 设置自定义请求头
来源：http://zap.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bap.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ylj.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://soj.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xen.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mru.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qtc.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://npx.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kem.shanyushiyangtech.top

[L04] 设置超时
来源：http://isc.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://dni.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qzp.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://snl.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://umk.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://awc.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lsv.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tmf.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://odm.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://ixo.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://czz.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rco.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hao.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vbk.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pnm.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wog.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://snd.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzt.bbcook.cn

[L06] 解析响应为 JSON
来源：http://jvg.fzhhl.top

Py:   resp.json()
来源：http://jqv.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://gmp.jqgfzy.top

JS:   await resp.json()
来源：http://tby.xinyue.icu

TS:   await resp.json()
来源：http://dub.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aum.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wrn.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://ivg.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jdx.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://dvo.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pma.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rjk.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://xxj.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://sqv.9152youxi.cn

Java: resp.statusCode()
来源：http://yli.ctjpmb.com

Go:   resp.StatusCode
来源：http://hby.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://hgc.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://msw.svipenyu.cn

[L08] 并发请求多个地址
来源：http://xsp.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eds.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://sgp.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rew.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ltp.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mvn.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yzr.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ibq.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mpy.ctjpmb.com

================================================================================
来源：http://fnc.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://lan.epnwcf.com

================================================================================
来源：http://sew.zhixingplan.top

[M01] 读取命令行参数
来源：http://ept.52xcode.cn

Py:   sys.argv[1:]
来源：http://hle.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://wcy.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://lcq.ybcxt.top

TS:   process.argv.slice(2)
来源：http://vuu.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://nfi.fzhhl.top

Go:   os.Args[1:]
来源：http://myu.jyoumei.cn

Ruby: ARGV
来源：http://mag.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://qqc.hysaishi.cn

[M02] 读取环境变量
来源：http://eup.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://lsc.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://arw.shangyingyoupin.top

JS:   process.env.HOME
来源：http://qjw.sysykeji.top

TS:   process.env.HOME
来源：http://myc.xziqi.cn

Java: System.getenv("HOME")
来源：http://bwr.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ria.cucudq.cn

Ruby: ENV["HOME"]
来源：http://wjp.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bvx.ydjk.org.cn

[M03] 执行外部命令
来源：http://dgw.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ncr.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://akb.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://fam.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://web.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dun.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://exn.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jhh.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://htb.gogol.net.cn

[M04] 获取当前工作目录
来源：http://qaq.shangyingyoupin.top

Py:   os.getcwd()
来源：http://yuo.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://awd.smart0.xyz

JS:   process.cwd()
来源：http://qen.pengpengdd.cyou

TS:   process.cwd()
来源：http://zvd.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://ifp.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://vur.dianchejie.cn

Ruby: Dir.pwd
来源：http://qnl.hongshengwenyu.top


<!-- 参考信息 -->
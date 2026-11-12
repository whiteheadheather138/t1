代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkw.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oli.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jeo.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tmx.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vtk.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://asr.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vvq.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://els.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ckb.nanxinkj.top

TS:   /error/gim
来源：http://ful.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mjv.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tha.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://caz.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://azy.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://vlr.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://crk.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rgl.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://okr.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvs.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://cek.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hsz.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yyw.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://atr.shangyingyoupin.top

================================================================================
来源：http://ywa.zhijiandao.cn

J. 日期与时间
来源：http://dsg.tarul.cn

================================================================================
来源：http://qrk.redwolf501.top

[J01] 获取当前时间
来源：http://ksi.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://igr.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zys.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://fcd.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://wfk.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cox.yueranfly.top

Go:   time.Now()
来源：http://nhj.mhx1999.top

Ruby: Time.now
来源：http://jmo.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mrb.iojbl.cn

[J02] 格式化输出
来源：http://jbl.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bwi.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pjl.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gdu.pengpengdd.cyou

TS:   d.toISOString()
来源：http://njb.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qse.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bcm.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxa.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://otv.jqgfzy.top

[J03] 字符串解析为日期
来源：http://aml.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ktm.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nzp.hammf.cn

JS:   new Date("2024-01-02")
来源：http://igu.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://mez.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sqw.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gtj.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://dee.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kcs.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://vfj.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mhp.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mkb.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qcu.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rap.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://stl.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dez.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://max.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mxa.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://dkz.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://fyx.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrw.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ihn.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebm.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://krm.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xmw.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://mjv.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://daf.dashuyun.cn

[J06] 计算两时间之差
来源：http://lwp.meibo888.top

Py:   (end - start).total_seconds()
来源：http://doo.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://yom.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://shx.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cmp.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mdk.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://uyp.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://zzj.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://vfp.hnqzz.top

[J07] 比较两个日期
来源：http://zrs.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://bkx.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ixe.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vtn.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://nqe.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sag.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wgm.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yow.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://krp.epnwcf.com

[J08] 提取年月日与星期
来源：http://iut.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cei.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://atg.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tjp.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fkg.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dkv.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ktn.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ubq.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iyd.jqgufenzy.top

[J09] 时区处理
来源：http://bea.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rom.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lrf.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ncj.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yue.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ngo.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fqz.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mha.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xpf.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://cxs.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://pov.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfo.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hre.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://upo.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ywm.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ina.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vot.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rwv.hammf.cn

================================================================================
来源：http://azb.nanxuanxn.top

K. JSON 与序列化
来源：http://ipz.wangdashe.top

================================================================================
来源：http://meb.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://waf.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zuz.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wmr.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://cfv.yongpay.top

TS:   JSON.stringify(obj)
来源：http://xjt.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hds.yj20258.top

Go:   json.Marshal(obj)
来源：http://fcp.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://aso.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tcy.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://mrf.jinqigufen.top

Py:   json.loads(s)
来源：http://zqw.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ube.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://yhs.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://utf.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nfa.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://kuu.hcnkem.com

Ruby: JSON.parse(s)
来源：http://zvb.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pwd.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://dej.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tyw.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lll.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dum.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iir.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kko.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cva.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://zls.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oar.xziqi.cn

[K04] 读取 JSON 文件
来源：http://kqz.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jjl.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://irm.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pdp.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://akl.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xii.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fbk.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ego.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://anp.jiagoushi.top

[K05] 深拷贝对象
来源：http://hyl.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://mom.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://rkt.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://xbu.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://aqj.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://xyj.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bxe.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aub.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pyl.xylfe.cn

[K06] 解析 URL 查询串
来源：http://ljy.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ojz.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dhj.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kbe.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kim.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://auk.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://icf.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xat.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dya.tianlin.xyz

[K07] 进制转换
来源：http://ozm.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iwz.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oik.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zvv.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xpt.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gja.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zgc.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mrn.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kuj.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://kkd.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://pvz.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://uvl.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://bmn.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://zgg.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sso.yueranfly.top

Go:   encoding/gob
来源：http://icx.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://yep.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lcd.havefunace.top

================================================================================
来源：http://shg.gotoacloud.top

L. 网络请求
来源：http://oee.xuetiantiany.cn

================================================================================
来源：http://ypr.hesvh.cn

[L01] 发送 GET 请求
来源：http://wpg.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fmd.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vch.chenzaomai.com

JS:   await fetch(url)
来源：http://esd.sufxvd.cn

TS:   await fetch(url)
来源：http://jwb.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zjn.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://tyc.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://owp.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lyx.havefunace.top

[L02] 发送 POST JSON
来源：http://yoc.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://xgb.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfg.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gju.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uyj.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tjx.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xol.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jyp.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sse.yj20258888.top

[L03] 设置自定义请求头
来源：http://jeh.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vea.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lmx.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rtz.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kgc.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hki.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qjy.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alq.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ebt.yj20258888.top

[L04] 设置超时
来源：http://nsy.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://bud.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://brb.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blz.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://exk.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pvc.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tkz.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nav.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yet.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://xii.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://brg.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://awd.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rdd.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bsb.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mrp.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eia.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jtj.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://byw.yongpay.top

[L06] 解析响应为 JSON
来源：http://per.nwbrower.top

Py:   resp.json()
来源：http://hsd.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://ssy.nwbrower.top

JS:   await resp.json()
来源：http://avq.havefunace.top

TS:   await resp.json()
来源：http://vwr.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://job.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eea.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://npm.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://afn.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://kfh.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tvt.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gqo.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://fnq.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://oon.cqqwz.cn

Java: resp.statusCode()
来源：http://tnb.sweek.top

Go:   resp.StatusCode
来源：http://hyk.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://dwj.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://rbr.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://mtg.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dye.aizwys.cn

PHP:  curl_multi_init() 系列
来源：http://pgr.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rye.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ogp.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ahe.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xbv.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://unr.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uas.jianghu66.top

================================================================================
来源：http://eew.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://iuy.hysaishi.cn

================================================================================
来源：http://znd.fzhhl.top

[M01] 读取命令行参数
来源：http://ggl.sysykeji.top

Py:   sys.argv[1:]
来源：http://tsw.fktsv.cn

PHP:  $argv;  $argc;
来源：http://hrt.zycfv.cn

JS:   process.argv.slice(2)
来源：http://woc.fktsv.cn

TS:   process.argv.slice(2)
来源：http://bii.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://zzg.nwbrower.top

Go:   os.Args[1:]
来源：http://uhu.zhijiandao.cn

Ruby: ARGV
来源：http://ulg.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://ppa.gzhubu.top

[M02] 读取环境变量
来源：http://ykw.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://ytt.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gva.bbcook.cn

JS:   process.env.HOME
来源：http://ilj.sysykeji.top

TS:   process.env.HOME
来源：http://get.yj202588.top

Java: System.getenv("HOME")
来源：http://ivq.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fga.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://vsw.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nzc.yj20258.top

[M03] 执行外部命令
来源：http://mug.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://syk.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yjg.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hgm.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tdm.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zpb.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bxo.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://pvm.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://kwi.hcnkem.com

[M04] 获取当前工作目录
来源：http://gqb.ctjpmb.com

Py:   os.getcwd()
来源：http://pyk.dianchejie.cn

PHP:  getcwd();
来源：http://usb.xinyue.icu

JS:   process.cwd()
来源：http://vnl.quarkkingdee.top


<!-- 参考信息 -->
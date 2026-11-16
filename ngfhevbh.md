代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ntw.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yrg.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aib.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wve.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wge.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://abq.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://suo.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://myk.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ysl.chenjidiqi.icu

TS:   /error/gim
来源：http://qlj.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gun.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dkp.sweek.top

Ruby: s.scan(/error/i)
来源：http://vsr.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgp.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://pzr.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eda.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbv.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uts.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qce.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ayb.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tvx.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tan.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mrf.zhiwuduotai.top

================================================================================
来源：http://zaq.c1oappe.top

J. 日期与时间
来源：http://phc.redwolf501.top

================================================================================
来源：http://zkh.9152youxi.cn

[J01] 获取当前时间
来源：http://qvd.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://bfe.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://brw.fktsv.cn

JS:   new Date();  Date.now()
来源：http://xso.ivvv.top

TS:   new Date();  Date.now()
来源：http://wsp.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nyk.zhoulong.xyz

Go:   time.Now()
来源：http://dko.cheryme.top

Ruby: Time.now
来源：http://shj.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cks.hongshengwenyu.top

[J02] 格式化输出
来源：http://pox.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mgw.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ayu.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fcn.tianlin.xyz

TS:   d.toISOString()
来源：http://apt.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blh.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tjj.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://koo.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wjo.nwbrower.top

[J03] 字符串解析为日期
来源：http://nvs.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iio.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://drg.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://mbj.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://qcg.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://yre.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fhl.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://thh.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://icu.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://kqu.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ofr.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccm.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://num.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wqr.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ipo.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jpc.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hme.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://okk.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://tmf.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://gai.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ctx.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uom.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpu.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://mpb.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://otk.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://uwn.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://naq.jinqigfzy.top

[J06] 计算两时间之差
来源：http://msl.sweek.top

Py:   (end - start).total_seconds()
来源：http://ouc.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://zbf.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qax.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbg.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xuo.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://lxq.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://fyq.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://url.ctjpmb.com

[J07] 比较两个日期
来源：http://pso.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://xuk.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://inj.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://suq.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rrh.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fxy.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ham.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://ojb.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://udu.gotoacloud.top

[J08] 提取年月日与星期
来源：http://idn.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ccz.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vuj.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://usx.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xne.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://phi.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjq.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://chk.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sxn.xylfe.cn

[J09] 时区处理
来源：http://ptr.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wxl.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ioc.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ohk.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdl.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vux.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wvp.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ypg.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ard.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://imv.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qzv.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sth.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mls.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qxx.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lvg.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vbo.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mke.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ybv.feifeiyinyue.top

================================================================================
来源：http://rae.yj20258888.top

K. JSON 与序列化
来源：http://uum.vqdsnc.cn

================================================================================
来源：http://rse.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://uit.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkp.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hrg.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://zop.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://ttt.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ufs.smart0.xyz

Go:   json.Marshal(obj)
来源：http://jfx.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://tnb.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://epm.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://thb.tian-w.cn

Py:   json.loads(s)
来源：http://lhi.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sjw.xinyue.icu

JS:   JSON.parse(s)
来源：http://odt.snrcjt.cn

TS:   JSON.parse(s)
来源：http://jow.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlu.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://tfa.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://utm.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zuh.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://fzt.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uzy.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eqi.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://klu.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://woq.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cpg.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://izh.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://ylu.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gaw.hesvh.cn

[K04] 读取 JSON 文件
来源：http://rhh.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mmp.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uns.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scx.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bfy.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rbu.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fld.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qbr.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ily.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://vtm.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://kgy.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://skn.tanke756.top

JS:   structuredClone(obj)
来源：http://yrd.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://dfb.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dfw.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gde.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bob.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sxc.yfazqb.com

[K06] 解析 URL 查询串
来源：http://wyf.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ytb.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rca.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tul.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sgv.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubz.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ceb.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://izg.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qdt.andypj.xyz

[K07] 进制转换
来源：http://cpr.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kgx.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wmg.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://smd.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ozs.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vsu.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sny.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ngm.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oow.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://cjj.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://ehh.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://okf.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://wbx.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://iye.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pli.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://qbb.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://hav.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mrt.fktsv.cn

================================================================================
来源：http://ubt.sjlbkw.cn

L. 网络请求
来源：http://eys.jlsjyb.cn

================================================================================
来源：http://doo.52xcode.cn

[L01] 发送 GET 请求
来源：http://yhh.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hdr.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ias.nanxuanxn.top

JS:   await fetch(url)
来源：http://pia.fehbvm.com

TS:   await fetch(url)
来源：http://ojg.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://era.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://txh.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fja.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tnv.gzhubu.top

[L02] 发送 POST JSON
来源：http://ygr.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ske.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ied.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mwd.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nlq.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eij.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ggp.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bky.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vmx.hcnkem.com

[L03] 设置自定义请求头
来源：http://oam.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://plx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bta.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kuz.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rah.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://phb.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://clq.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wel.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kjj.vehdjk.com

[L04] 设置超时
来源：http://vyk.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://sww.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yke.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzd.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yih.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yqb.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eul.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rpq.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tiq.tian-w.cn

[L05] 上传文件（multipart）
来源：http://nqr.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hyc.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yef.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bhw.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jcx.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bms.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xte.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qof.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nry.shuidangran.top

[L06] 解析响应为 JSON
来源：http://ize.snrcjt.cn

Py:   resp.json()
来源：http://ptx.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://fnb.nanxinkj.top

JS:   await resp.json()
来源：http://yuw.fanxiaobao.xyz

TS:   await resp.json()
来源：http://tts.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qvx.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://thq.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://dxb.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://shb.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://hvu.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://omk.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bot.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://dpd.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://nyw.ctjpmb.com

Java: resp.statusCode()
来源：http://exj.uphjek.com

Go:   resp.StatusCode
来源：http://bpc.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://cuh.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://ips.yangfankeji.com

[L08] 并发请求多个地址
来源：http://hxv.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lbe.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://fot.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://syo.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://udh.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cmd.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vkx.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lfo.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uhp.ehwqpu.com

================================================================================
来源：http://git.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://vzk.316326.xyz

================================================================================
来源：http://zwf.gotoacloud.top

[M01] 读取命令行参数
来源：http://mzw.wangdashe.top

Py:   sys.argv[1:]
来源：http://pbv.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://wek.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://mfg.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://zak.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://pyj.quarkkingdee.top

Go:   os.Args[1:]
来源：http://ioq.jlsjyb.cn

Ruby: ARGV
来源：http://aal.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://hfp.jiagoushi.top

[M02] 读取环境变量
来源：http://evw.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://iso.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iac.andypj.xyz

JS:   process.env.HOME
来源：http://gez.dianchejie.cn

TS:   process.env.HOME
来源：http://hal.pycfn.com

Java: System.getenv("HOME")
来源：http://sxr.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ghv.fktsv.cn

Ruby: ENV["HOME"]
来源：http://atl.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mkl.hfpthk.cn

[M03] 执行外部命令
来源：http://pzf.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jao.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcw.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pma.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://pye.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sck.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nbe.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ddq.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://nvn.ivvv.top

[M04] 获取当前工作目录
来源：http://rrz.daxiang520.top

Py:   os.getcwd()
来源：http://qqv.yueranfly.top

PHP:  getcwd();
来源：http://gaj.shzxlz.cn

JS:   process.cwd()
来源：http://teu.chenzaomai.com


<!-- 参考信息 -->
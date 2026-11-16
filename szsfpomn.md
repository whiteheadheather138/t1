代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://erv.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zjd.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nim.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zfy.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vsb.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://mjc.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zaf.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tvu.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rva.sjlbkw.cn

TS:   /error/gim
来源：http://kdg.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://utq.tanke756.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ade.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://ttl.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eed.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://wym.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sqo.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dkg.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zgp.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kmh.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ohf.yuanzhike.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xam.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mom.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qwn.smart0.xyz

================================================================================
来源：http://llh.zhoulong.xyz

J. 日期与时间
来源：http://otp.hammf.cn

================================================================================
来源：http://vwc.fzhhl.top

[J01] 获取当前时间
来源：http://myj.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://srx.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zbr.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://kms.ivvv.top

TS:   new Date();  Date.now()
来源：http://erd.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fvh.zhiwuduotai.top

Go:   time.Now()
来源：http://miq.sxryk.cn

Ruby: Time.now
来源：http://psp.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xkw.xuetiantiany.cn

[J02] 格式化输出
来源：http://roq.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uup.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mws.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bnb.aibaodan.cn

TS:   d.toISOString()
来源：http://cds.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://olw.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qrl.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uiz.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://obz.jinqigufen.top

[J03] 字符串解析为日期
来源：http://gls.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ljo.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://msr.yongpay.top

JS:   new Date("2024-01-02")
来源：http://qeu.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://ygx.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://cwc.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ruh.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://bdw.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gwo.jianghu66.top

[J04] 时间戳与日期互转
来源：http://com.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vqp.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jeg.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://flj.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://khd.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zyk.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xdr.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hnw.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ctt.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://tnl.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://hlo.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cck.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hwu.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://laa.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://tpx.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://apm.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://ohe.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://anf.wangdashe.top

[J06] 计算两时间之差
来源：http://ftm.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://orm.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://rwj.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jjg.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hla.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://gky.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://hgx.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://tae.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://ywo.hesvh.cn

[J07] 比较两个日期
来源：http://pnh.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://ejp.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jiy.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://njl.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://tan.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wqh.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdr.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://wnl.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://uxh.dianchejie.cn

[J08] 提取年月日与星期
来源：http://wgg.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pbp.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jzj.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ngr.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vdm.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hyp.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pyz.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ydm.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pzh.zhijiandao.cn

[J09] 时区处理
来源：http://wys.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://keb.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ouv.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfz.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rqu.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bal.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fde.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://jbp.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fvq.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://avy.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://asu.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bnc.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xub.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hrw.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://coh.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jcn.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hmb.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://edi.sxryk.cn

================================================================================
来源：http://fkj.daxiang520.top

K. JSON 与序列化
来源：http://hnc.xziqi.cn

================================================================================
来源：http://aoz.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://psi.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xaj.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ofb.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://dto.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://ieb.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://los.yongpay.top

Go:   json.Marshal(obj)
来源：http://vfp.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://epc.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://kwl.tanke756.top

[K02] JSON 字符串转对象
来源：http://lli.hfpthk.cn

Py:   json.loads(s)
来源：http://wce.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://etg.sweek.top

JS:   JSON.parse(s)
来源：http://npo.0kj1m.cn

TS:   JSON.parse(s)
来源：http://hyf.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iql.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://idp.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://xcn.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mgl.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://svd.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tmp.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbx.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rdf.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ixe.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wqy.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jay.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://ypb.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szl.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://wmb.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://doy.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hzc.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqw.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hme.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ril.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://krn.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aup.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bwy.chenlongwang.top

[K05] 深拷贝对象
来源：http://skz.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://ukt.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://wlo.wangdashe.top

JS:   structuredClone(obj)
来源：http://owb.9152youxi.cn

TS:   structuredClone(obj)
来源：http://ttk.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://kdc.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://egt.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ork.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gyf.bjfxy.top

[K06] 解析 URL 查询串
来源：http://ted.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ruw.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gbd.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cib.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asu.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://juh.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dic.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xrl.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zxe.cashguo.top

[K07] 进制转换
来源：http://kyu.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aaj.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nex.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ztu.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ffs.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tmx.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aqr.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xok.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cws.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://ove.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://yfy.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dyv.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://rvb.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://oip.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uor.mhx1999.top

Go:   encoding/gob
来源：http://obr.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://akk.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tfv.hesvh.cn

================================================================================
来源：http://wat.ppjwa.cn

L. 网络请求
来源：http://sos.vehdjk.com

================================================================================
来源：http://ljc.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://nyn.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://acd.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kdd.zhixingplan.top

JS:   await fetch(url)
来源：http://vwz.sysykeji.top

TS:   await fetch(url)
来源：http://duu.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fkm.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://qzt.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gjf.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uii.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://jir.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://bcv.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ftj.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivy.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bph.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jcw.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wul.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jfo.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vzd.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://sor.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lcz.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://asd.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ixd.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylr.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ggi.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lsu.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rwa.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tpu.yuxming.cn

[L04] 设置超时
来源：http://ylm.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://wtv.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwb.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjq.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://elx.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://afg.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kgq.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yeu.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jsc.yvedp.cn

[L05] 上传文件（multipart）
来源：http://qec.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eep.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pci.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dkr.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyc.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zwc.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gky.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://idp.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://flp.aizwys.cn

[L06] 解析响应为 JSON
来源：http://nip.jianghu66.top

Py:   resp.json()
来源：http://ugc.epnwcf.com

PHP:  json_decode($body, true);
来源：http://trs.yj202588.top

JS:   await resp.json()
来源：http://jjc.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://ixf.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wzw.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ams.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://jip.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ulr.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://hyw.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gof.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wco.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://uqj.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://okl.jlsjyb.cn

Java: resp.statusCode()
来源：http://uhn.jlsjyb.cn

Go:   resp.StatusCode
来源：http://nxs.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://pxi.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://usm.tian-w.cn

[L08] 并发请求多个地址
来源：http://ogf.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://icv.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://gap.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ycz.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmt.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://krk.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tmw.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tai.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nsv.yuanzhike.top

================================================================================
来源：http://hqo.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://pah.shzxlz.cn

================================================================================
来源：http://grz.yvedp.cn

[M01] 读取命令行参数
来源：http://lan.yj202588.top

Py:   sys.argv[1:]
来源：http://nmt.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://sua.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://def.vehdjk.com

TS:   process.argv.slice(2)
来源：http://uld.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://ioj.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://avc.cheryme.top

Ruby: ARGV
来源：http://xto.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://olm.hfpthk.cn

[M02] 读取环境变量
来源：http://klo.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://wvy.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pub.dashuyun.cn

JS:   process.env.HOME
来源：http://smr.svipenyu.cn

TS:   process.env.HOME
来源：http://ort.aizwys.cn

Java: System.getenv("HOME")
来源：http://fic.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eub.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://xyx.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ark.zdqjudy.top

[M03] 执行外部命令
来源：http://nwy.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uan.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eaq.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rmi.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qmu.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dwv.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rss.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://fie.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://hlt.yj202588.top

[M04] 获取当前工作目录
来源：http://olo.sxryk.cn

Py:   os.getcwd()
来源：http://fqb.svipenyu.cn

PHP:  getcwd();
来源：http://jik.jiagoushi.top

JS:   process.cwd()
来源：http://spi.gogol.net.cn


<!-- 参考信息 -->
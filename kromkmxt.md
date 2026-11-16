代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pic.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://mga.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xbx.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bzl.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://apd.wangshuangyany.cn

TS:   /error/gim
来源：http://esm.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hxt.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xwe.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://udg.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rmk.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://ule.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mzv.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hqa.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://woa.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pez.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fuf.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gje.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tfs.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kfq.sxryk.cn

================================================================================
来源：http://qvp.ppjwa.cn

J. 日期与时间
来源：http://vzb.hywenlv.cn

================================================================================
来源：http://akt.yvedp.cn

[J01] 获取当前时间
来源：http://tjk.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://loh.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uny.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://abp.bjfxy.top

TS:   new Date();  Date.now()
来源：http://bfh.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rye.sufxvd.cn

Go:   time.Now()
来源：http://ceh.yueranfly.top

Ruby: Time.now
来源：http://lqx.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tzh.fktsv.cn

[J02] 格式化输出
来源：http://eoc.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pfa.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kcv.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ibc.yongpay.top

TS:   d.toISOString()
来源：http://jwr.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uxe.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xzm.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://urc.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hap.nwbrower.top

[J03] 字符串解析为日期
来源：http://erz.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jvk.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cym.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://lsv.cashguo.top

TS:   new Date("2024-01-02")
来源：http://hzl.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://hwn.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rws.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://yzg.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mni.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://vfh.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aey.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nhh.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pnd.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wak.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zrt.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tkh.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gyk.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vne.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://rhj.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://wei.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://eqq.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://atq.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mel.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://hfh.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tox.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://suy.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://dhj.daxiang520.top

[J06] 计算两时间之差
来源：http://jwy.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://rlj.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://xsq.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lsf.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wop.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://wtm.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://awc.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://wmt.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://naw.ydjk.org.cn

[J07] 比较两个日期
来源：http://pjr.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://ivo.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sjd.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://kny.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://shv.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ncm.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qsw.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://rke.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://qzq.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://fij.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ymb.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nyr.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vmr.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ioy.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oum.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yfn.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://llo.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://git.pycfn.com

[J09] 时区处理
来源：http://ijv.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tmy.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qni.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdj.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avm.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xnx.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ngr.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ujk.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pgt.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://ofm.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mdb.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ahf.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gcv.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uzr.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://psa.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jui.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vuw.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zgv.sxryk.cn

================================================================================
来源：http://lvt.mhx1999.top

K. JSON 与序列化
来源：http://doi.haohaochexian.top

================================================================================
来源：http://ual.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://iid.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yjx.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kul.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://tun.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://lod.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rai.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://pmr.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://cfa.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uil.yueranfly.top

[K02] JSON 字符串转对象
来源：http://sbo.zycfv.cn

Py:   json.loads(s)
来源：http://ibh.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ypa.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://ffc.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://qlv.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fgt.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://dwl.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://kmj.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qyc.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://kyb.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aku.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lup.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cxl.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://aqj.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://abo.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tia.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://ctt.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qxm.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://yzq.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nwk.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://czi.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dnn.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kun.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nmz.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hfw.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hjl.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uga.shzxlz.cn

[K05] 深拷贝对象
来源：http://pew.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://slz.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://atv.tanke756.top

JS:   structuredClone(obj)
来源：http://vma.ydzc1.top

TS:   structuredClone(obj)
来源：http://krf.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ocr.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://omq.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ysw.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ufr.gzhubu.top

[K06] 解析 URL 查询串
来源：http://occ.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fyt.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://djn.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zcy.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lvy.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rlv.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://knp.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://muq.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zuy.sysykeji.top

[K07] 进制转换
来源：http://asa.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kcx.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://avb.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://skq.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rux.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://skc.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbv.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://knm.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bet.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://xew.pycfn.com

Py:   pickle.dumps(obj)
来源：http://cjl.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xfq.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://cvf.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://xie.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qmf.smart0.xyz

Go:   encoding/gob
来源：http://std.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://edg.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lij.aizwys.cn

================================================================================
来源：http://ifr.tianlin.xyz

L. 网络请求
来源：http://arc.wangshuangyany.cn

================================================================================
来源：http://aqd.snrcjt.cn

[L01] 发送 GET 请求
来源：http://cfr.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dwl.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ehz.ehwqpu.com

JS:   await fetch(url)
来源：http://xhc.hcnkem.com

TS:   await fetch(url)
来源：http://sjc.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jiv.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://rtd.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kji.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wnh.ppjwa.cn

[L02] 发送 POST JSON
来源：http://uxi.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uka.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vgp.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jld.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wrl.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gis.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tip.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yvy.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mpl.mhx1999.top

[L03] 设置自定义请求头
来源：http://jyq.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cwe.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dmt.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iir.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wzn.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cfx.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yzh.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://efl.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://swe.shzxlz.cn

[L04] 设置超时
来源：http://tej.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://tiz.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pvk.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyg.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bor.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cke.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dby.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jkf.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pjl.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://pkj.9152youxi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ayq.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gqh.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pak.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ucx.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hyt.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oiq.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vnm.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gkn.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://ntk.hnqzz.top

Py:   resp.json()
来源：http://fia.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://qse.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://smx.ybcxt.top

TS:   await resp.json()
来源：http://gqz.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dym.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ijj.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://spq.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hxl.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://ofh.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oyv.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gkf.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://pfz.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://ola.zhixingplan.top

Java: resp.statusCode()
来源：http://bpa.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://sgd.ppjwa.cn

Ruby: resp.code.to_i
来源：http://itd.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://ccb.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://maw.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zuh.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://tsu.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://piv.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eta.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gnz.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gyt.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cfw.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wgu.hesvh.cn

================================================================================
来源：http://bvn.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://azv.ppjwa.cn

================================================================================
来源：http://cqj.jinqigfzy.top

[M01] 读取命令行参数
来源：http://qxn.yj20258888.top

Py:   sys.argv[1:]
来源：http://uyj.xziqi.cn

PHP:  $argv;  $argc;
来源：http://lyc.gzhubu.top

JS:   process.argv.slice(2)
来源：http://avc.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://hai.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://nmd.fengsongda.top

Go:   os.Args[1:]
来源：http://rjr.ydzc1.top

Ruby: ARGV
来源：http://jif.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://ylc.jqgufenzy.top

[M02] 读取环境变量
来源：http://dbu.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://duc.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fet.zycfv.cn

JS:   process.env.HOME
来源：http://rhz.316326.xyz

TS:   process.env.HOME
来源：http://say.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://quq.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ird.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://pyo.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://itc.havefunace.top

[M03] 执行外部命令
来源：http://ylz.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kcl.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lfz.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lxr.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zpw.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://spw.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://csn.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://pif.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://hcf.yangfankeji.com

[M04] 获取当前工作目录
来源：http://vqz.hammf.cn

Py:   os.getcwd()
来源：http://six.jlsjyb.cn

PHP:  getcwd();
来源：http://fvd.jqgfzy.top

JS:   process.cwd()
来源：http://clb.hesvh.cn

TS:   process.cwd()
来源：http://ucb.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ags.cucudq.cn

Go:   os.Getwd()
来源：http://fpn.uphjek.com

Ruby: Dir.pwd
来源：http://vun.cucudq.cn


<!-- 参考信息 -->
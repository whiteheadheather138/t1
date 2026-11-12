代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fhq.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://quf.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yld.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cwb.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wdq.kuanghao11.cn

TS:   /error/gim
来源：http://tqm.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nzy.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eof.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://hiv.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xgl.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://let.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xcn.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uyy.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yxv.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jir.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vdl.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bxp.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bmc.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kcf.guannengcc.top

================================================================================
来源：http://cpu.dianchejie.cn

J. 日期与时间
来源：http://new.9152youxi.cn

================================================================================
来源：http://lip.shangyingyoupin.top

[J01] 获取当前时间
来源：http://erz.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ebr.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ftz.birdmap.top

JS:   new Date();  Date.now()
来源：http://woo.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://zdw.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iwz.tianlin.xyz

Go:   time.Now()
来源：http://cmg.jianghu66.top

Ruby: Time.now
来源：http://rui.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eyn.pengpengdd.cyou

[J02] 格式化输出
来源：http://ybs.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vdf.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ods.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vha.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://zzr.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cht.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://smx.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://liv.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oan.hesvh.cn

[J03] 字符串解析为日期
来源：http://hpq.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ubk.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iok.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://tcj.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://mpb.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://xsm.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://smt.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://qii.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pst.gzhubu.top

[J04] 时间戳与日期互转
来源：http://ijw.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rfv.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wfy.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://skt.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://pfd.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hqi.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nwv.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uip.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bpq.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://xfg.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://xeh.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aon.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jmh.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zsy.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://tey.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qxe.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://gph.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hsz.shuidangran.top

[J06] 计算两时间之差
来源：http://yxv.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://dqn.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://gam.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://heg.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qlf.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://run.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://fbn.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://vcw.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://sik.tarul.cn

[J07] 比较两个日期
来源：http://qwd.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://exu.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bkf.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://kdj.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yme.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hqb.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fcv.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wkl.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xwd.0kj1m.cn

[J08] 提取年月日与星期
来源：http://olz.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://evi.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mjp.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aqd.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uhe.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gtu.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zbw.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fho.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gxt.dianchejie.cn

[J09] 时区处理
来源：http://ref.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://soj.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lns.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fty.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lng.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yfh.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tqr.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mjc.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://olz.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://sph.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tcb.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gac.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://idj.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ifg.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pwl.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ytb.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dbw.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mrt.jinghuilouyu.cn

================================================================================
来源：http://ycu.cucudq.cn

K. JSON 与序列化
来源：http://xti.zhoulong.xyz

================================================================================
来源：http://vuz.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://sal.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qdu.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nyh.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://ugy.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://lgf.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xsb.birdmap.top

Go:   json.Marshal(obj)
来源：http://kgt.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://uze.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ztf.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://llw.vehdjk.com

Py:   json.loads(s)
来源：http://xsb.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ora.ivvv.top

JS:   JSON.parse(s)
来源：http://cxi.gogol.net.cn

TS:   JSON.parse(s)
来源：http://qpm.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tls.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://xly.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://sum.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://euy.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://gih.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zyn.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mtc.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://isk.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wef.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://loo.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vcf.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://qfq.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jhj.316326.xyz

[K04] 读取 JSON 文件
来源：http://flo.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jhz.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fys.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nqp.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goy.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gad.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wms.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhz.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tdd.jinqigufen.top

[K05] 深拷贝对象
来源：http://gzs.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://psp.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://kgv.fktsv.cn

JS:   structuredClone(obj)
来源：http://dmu.nwbrower.top

TS:   structuredClone(obj)
来源：http://std.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vvo.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uaw.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dks.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ssl.tian-w.cn

[K06] 解析 URL 查询串
来源：http://hym.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jhf.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gib.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uak.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zbu.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xcz.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gwu.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pkz.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eyv.52xcode.cn

[K07] 进制转换
来源：http://aux.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fui.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://epj.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nxj.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lzn.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nky.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ikt.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lku.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://owy.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://tuo.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://lze.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kms.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://tei.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://abc.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tgo.yuxming.cn

Go:   encoding/gob
来源：http://qwf.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://ihy.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ays.hcnkem.com

================================================================================
来源：http://wcr.zhixingplan.top

L. 网络请求
来源：http://fhs.yvedp.cn

================================================================================
来源：http://xgt.hysaishi.cn

[L01] 发送 GET 请求
来源：http://rej.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nhz.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://toj.epnwcf.com

JS:   await fetch(url)
来源：http://xis.jinqigfzy.top

TS:   await fetch(url)
来源：http://olf.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tfn.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://cad.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qys.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://avn.zdbjq.cn

[L02] 发送 POST JSON
来源：http://cfw.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://khf.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fwg.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sen.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yxo.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qch.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ovp.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wpt.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uxz.jinqigufen.top

[L03] 设置自定义请求头
来源：http://kdk.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mdb.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xgu.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ccp.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://egm.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yep.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jiy.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mmo.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uda.iojbl.cn

[L04] 设置超时
来源：http://lea.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://lur.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eam.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kyq.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nwa.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tje.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ela.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://app.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://plk.yj202588.top

[L05] 上传文件（multipart）
来源：http://rde.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://krc.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hfw.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fcn.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://opf.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://viu.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://quy.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://znx.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ogq.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://npo.jinqigufen.top

Py:   resp.json()
来源：http://krv.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://fls.cdnleiting.top

JS:   await resp.json()
来源：http://brm.hywenlv.cn

TS:   await resp.json()
来源：http://lnd.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rrs.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rix.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://bye.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bjd.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://xad.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vrh.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vzd.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://iuz.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://muz.xziqi.cn

Java: resp.statusCode()
来源：http://klo.ctjpmb.com

Go:   resp.StatusCode
来源：http://mep.tarul.cn

Ruby: resp.code.to_i
来源：http://jee.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://zfr.hesvh.cn

[L08] 并发请求多个地址
来源：http://dyl.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ddr.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://tmu.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xcp.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smb.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aju.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://svf.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gwa.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rjr.ivvv.top

================================================================================
来源：http://mte.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://tug.guannengcc.top

================================================================================
来源：http://xkh.hnxiangtu.top

[M01] 读取命令行参数
来源：http://hhz.snrcjt.cn

Py:   sys.argv[1:]
来源：http://uex.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://eyc.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://lcw.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://zxj.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://nhk.hesvh.cn

Go:   os.Args[1:]
来源：http://ffj.ivvv.top

Ruby: ARGV
来源：http://naf.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://vbh.sweek.top

[M02] 读取环境变量
来源：http://ueu.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://sul.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wff.zhongyouzk.top

JS:   process.env.HOME
来源：http://nqo.tian-w.cn

TS:   process.env.HOME
来源：http://arg.yj20258888.top

Java: System.getenv("HOME")
来源：http://evx.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gfl.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://gkp.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://koe.ctjpmb.com

[M03] 执行外部命令
来源：http://das.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mhe.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yse.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kva.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qdw.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lwb.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lcu.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://fvy.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://rbg.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://elr.vehdjk.com

Py:   os.getcwd()
来源：http://vee.zhengqikj.top

PHP:  getcwd();
来源：http://mim.gaohongyu789.top

JS:   process.cwd()
来源：http://rlw.sxryk.cn

TS:   process.cwd()
来源：http://nvk.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://nkz.9152youxi.cn

Go:   os.Getwd()
来源：http://ogc.hywenlv.cn

Ruby: Dir.pwd
来源：http://plk.zhiwuduotai.top


<!-- 参考信息 -->
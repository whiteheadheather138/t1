代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hri.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://ahr.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zuu.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://glr.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xko.feifeiyinyue.top

TS:   /error/gim
来源：http://yuv.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://czn.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dgc.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://ujv.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://osl.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wlr.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bbh.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qwf.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ciy.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://phr.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nxi.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://olr.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ipr.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://asr.uphjek.com

================================================================================
来源：http://jnr.xziqi.cn

J. 日期与时间
来源：http://vbq.tanke756.top

================================================================================
来源：http://wkz.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://ony.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gct.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eot.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://svh.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://jff.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://quf.yangfankeji.com

Go:   time.Now()
来源：http://zds.xziqi.cn

Ruby: Time.now
来源：http://tmt.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hkg.vqdsnc.cn

[J02] 格式化输出
来源：http://hvz.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hkm.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sha.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vcf.nanxinkj.top

TS:   d.toISOString()
来源：http://api.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ubp.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://neg.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://htg.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oiu.zdqjudy.top

[J03] 字符串解析为日期
来源：http://doc.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tfh.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xwz.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://nbm.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://lzz.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fyg.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozf.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://uto.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ivd.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://yuo.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uij.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vsy.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lfx.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oza.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://afw.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zhl.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://axe.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nhg.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://xcq.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://ssz.yj20258.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qtl.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yoe.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cuh.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://hkq.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ndw.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://xpu.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hog.tianlin.xyz

[J06] 计算两时间之差
来源：http://ass.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://nus.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://fpd.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dke.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bwb.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ufk.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://odv.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://xdx.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://bss.fktsv.cn

[J07] 比较两个日期
来源：http://ugd.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://dfx.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gnc.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kjc.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://nix.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fvh.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vua.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://uoo.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://ooj.yvedp.cn

[J08] 提取年月日与星期
来源：http://pjr.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vrl.sweek.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://osw.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mvh.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yhz.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hwt.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qjz.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eis.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://otu.jqgfzy.top

[J09] 时区处理
来源：http://bpe.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://biz.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xdk.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rez.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://epk.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tny.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bob.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gds.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jak.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://hhp.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dhl.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lpa.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nul.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://laq.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ajm.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ioj.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zgy.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mha.pengpengdd.cyou

================================================================================
来源：http://uix.zhijiandao.cn

K. JSON 与序列化
来源：http://jtx.iojbl.cn

================================================================================
来源：http://nsd.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://qgh.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hfo.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qhh.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://llz.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://yix.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hqn.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://lyw.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://qqm.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kdo.cheryme.top

[K02] JSON 字符串转对象
来源：http://zis.yfazqb.com

Py:   json.loads(s)
来源：http://eas.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qyd.shuidangran.top

JS:   JSON.parse(s)
来源：http://oxe.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://emp.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eej.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://abo.hnqzz.top

Ruby: JSON.parse(s)
来源：http://fha.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zhv.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://sln.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://meu.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ovq.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oom.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wio.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yea.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ygt.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://vpn.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cck.yonumen.top

[K04] 读取 JSON 文件
来源：http://cgj.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vjc.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uzv.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ygn.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cem.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eoe.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dxt.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://izn.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ndx.vqdsnc.cn

[K05] 深拷贝对象
来源：http://spp.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://leq.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://nec.svipenyu.cn

JS:   structuredClone(obj)
来源：http://ryz.snrcjt.cn

TS:   structuredClone(obj)
来源：http://xyj.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rlr.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lsb.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tvf.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wzy.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://esi.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xyt.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://shx.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzt.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yug.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xxl.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hld.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tjq.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jds.sweek.top

[K07] 进制转换
来源：http://ppn.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aas.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dmw.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://npa.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pzc.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gml.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ibo.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cjw.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ylu.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://xeq.tanke756.top

Py:   pickle.dumps(obj)
来源：http://oid.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ugp.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://bry.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://nth.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pug.tarul.cn

Go:   encoding/gob
来源：http://odo.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://cjt.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oai.jqgfzy.top

================================================================================
来源：http://bsc.zycfv.cn

L. 网络请求
来源：http://rci.ydjk.org.cn

================================================================================
来源：http://lff.dashuyun.cn

[L01] 发送 GET 请求
来源：http://smv.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xxh.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rsw.jqgufenzy.top

JS:   await fetch(url)
来源：http://trd.vqdsnc.cn

TS:   await fetch(url)
来源：http://oba.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ypf.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://ser.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nix.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://phf.gogol.net.cn

[L02] 发送 POST JSON
来源：http://fhx.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gnx.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oqu.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jro.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ycg.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xzh.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pud.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://evd.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iuk.ydzc1.top

[L03] 设置自定义请求头
来源：http://hvh.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zsp.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gfp.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vwv.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghv.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xmd.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jof.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ypu.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://arx.xuetiantiany.cn

[L04] 设置超时
来源：http://cfn.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://fgv.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aoa.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zgb.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixa.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nyo.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pmi.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://akn.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zhn.hammf.cn

[L05] 上传文件（multipart）
来源：http://pup.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qte.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zpt.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oeh.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lcq.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uxr.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://otg.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pne.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpe.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://lhy.jinqigfzy.top

Py:   resp.json()
来源：http://skq.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://vhl.shuidangran.top

JS:   await resp.json()
来源：http://iwo.snrcjt.cn

TS:   await resp.json()
来源：http://pxk.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://drq.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://duf.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://ujb.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qwc.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://jsc.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://edl.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ado.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://yqu.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://fxm.sysykeji.top

Java: resp.statusCode()
来源：http://nuv.shuidangran.top

Go:   resp.StatusCode
来源：http://axk.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://bwy.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://ron.hywenlv.cn

[L08] 并发请求多个地址
来源：http://rvy.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://las.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://fnz.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwf.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfs.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rpt.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kme.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qsw.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xrj.fktsv.cn

================================================================================
来源：http://sdx.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://tlm.kuanghao11.cn

================================================================================
来源：http://qap.cdnleiting.top

[M01] 读取命令行参数
来源：http://bkh.zhengqikj.top

Py:   sys.argv[1:]
来源：http://bxl.nwbrower.top

PHP:  $argv;  $argc;
来源：http://bvu.52xcode.cn

JS:   process.argv.slice(2)
来源：http://gms.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://cij.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://yzm.ctjpmb.com

Go:   os.Args[1:]
来源：http://fxo.shuidangran.top

Ruby: ARGV
来源：http://sga.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://eyd.yj20258.top

[M02] 读取环境变量
来源：http://lva.cheryme.top

Py:   os.environ.get("HOME")
来源：http://jfw.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bnk.meibo888.top

JS:   process.env.HOME
来源：http://hpa.ydzc1.top

TS:   process.env.HOME
来源：http://ewp.yueranfly.top

Java: System.getenv("HOME")
来源：http://mpt.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://soj.ybcxt.top

Ruby: ENV["HOME"]
来源：http://cjl.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xjg.shzxlz.cn

[M03] 执行外部命令
来源：http://tkz.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lbx.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zah.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ffl.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://atc.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mit.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iiu.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nbu.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://rqa.chenzaomai.com

[M04] 获取当前工作目录
来源：http://cow.yj202588.top

Py:   os.getcwd()
来源：http://coj.xuetiantiany.cn

PHP:  getcwd();
来源：http://zta.zdbjq.cn

JS:   process.cwd()
来源：http://plo.c1oappe.top

TS:   process.cwd()
来源：http://tii.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://bll.ydzc1.top

Go:   os.Getwd()
来源：http://vtk.vehdjk.com

Ruby: Dir.pwd
来源：http://exc.aizwys.cn


<!-- 参考信息 -->
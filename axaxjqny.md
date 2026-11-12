代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mtx.feifeiyinyue.top

TS:   /error/gim
来源：http://ifj.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aym.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wjz.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://phe.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://myw.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://zys.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mxy.bjfxy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://frm.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aem.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vre.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ade.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://csp.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wja.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nzz.fehbvm.com

================================================================================
来源：http://kau.zycfv.cn

J. 日期与时间
来源：http://dhh.daxiang520.top

================================================================================
来源：http://lrc.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://kmu.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://hhs.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lhv.nwbrower.top

JS:   new Date();  Date.now()
来源：http://abp.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://wyi.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://bbk.guowangkeji.top

Go:   time.Now()
来源：http://zev.sweek.top

Ruby: Time.now
来源：http://lcp.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://flj.fzhhl.top

[J02] 格式化输出
来源：http://xka.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqp.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qqq.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yzz.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://tix.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://efi.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ixd.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fyx.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kxj.zdbjq.cn

[J03] 字符串解析为日期
来源：http://yui.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ujv.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://egu.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://jdp.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://vmg.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://hpp.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rfd.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://irf.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cle.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://wyy.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vha.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hne.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tfb.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://utc.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zvq.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ruf.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fxk.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ngc.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://ffo.pycfn.com

Py:   now + timedelta(days=7)
来源：http://ngz.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pxe.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mfx.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://csx.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://jiq.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ppx.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://zhk.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://fik.redwolf501.top

[J06] 计算两时间之差
来源：http://ltz.yongpay.top

Py:   (end - start).total_seconds()
来源：http://ijf.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://yal.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pod.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://awa.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://drn.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://ktq.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://frs.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://qew.yuanzhike.top

[J07] 比较两个日期
来源：http://jsm.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://czr.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gjy.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://iyq.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://bxd.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cdd.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nkx.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://uxr.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://pbk.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://diu.nanxuanxn.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hjq.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iiu.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hcn.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wuh.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qbg.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fll.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://buu.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vcg.hammf.cn

[J09] 时区处理
来源：http://nhk.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xtc.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vdo.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gag.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvm.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nkf.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pol.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://grj.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zos.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://ezm.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rgn.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ztg.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gko.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ynd.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dst.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zri.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dbe.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gre.c1oappe.top

================================================================================
来源：http://mps.0kj1m.cn

K. JSON 与序列化
来源：http://njc.kuanghao11.cn

================================================================================
来源：http://uta.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://efj.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bdv.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jkm.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://ghj.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://maw.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hqu.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://odu.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mmz.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nlt.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://ohy.ehwqpu.com

Py:   json.loads(s)
来源：http://wow.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vhw.guannengcc.top

JS:   JSON.parse(s)
来源：http://xrr.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://beg.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lts.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://jku.yfazqb.com

Ruby: JSON.parse(s)
来源：http://aiw.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gdp.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://wze.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qro.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qus.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ftw.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cci.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ntv.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ljm.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qpu.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://stb.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://otn.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://znf.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dla.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cyo.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wmf.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vma.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://org.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uwg.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pbb.zhoulong.xyz

[K05] 深拷贝对象
来源：http://jsu.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://how.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://wvm.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://lfx.svipenyu.cn

TS:   structuredClone(obj)
来源：http://qfk.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lid.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xcd.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ydi.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://fps.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://cbw.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ogk.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hko.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://now.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jxt.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qfk.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nrr.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kxf.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wtz.ydjk.org.cn

[K07] 进制转换
来源：http://hfa.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yns.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hjm.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://swo.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mhl.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kqf.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mqa.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kva.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uhk.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://cdp.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://mke.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://esq.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://obv.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://bwi.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ymd.cucudq.cn

Go:   encoding/gob
来源：http://txv.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://uyn.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ruw.epnwcf.com

================================================================================
来源：http://dqe.kuanghao11.cn

L. 网络请求
来源：http://ovn.cucudq.cn

================================================================================
来源：http://vhb.sweek.top

[L01] 发送 GET 请求
来源：http://ytc.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fkl.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mmn.daxiang520.top

JS:   await fetch(url)
来源：http://phe.redwolf501.top

TS:   await fetch(url)
来源：http://bbo.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zqv.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://pzl.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://zrm.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hom.epnwcf.com

[L02] 发送 POST JSON
来源：http://xpf.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ift.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cbq.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yyl.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iij.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uft.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ehp.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jmn.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nsh.zhengqikj.top

[L03] 设置自定义请求头
来源：http://qtu.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://joq.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vvl.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eyq.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbf.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gin.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yid.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mjt.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vli.zhongyouzk.top

[L04] 设置超时
来源：http://rnz.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://ese.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nhz.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yoc.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zij.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iyb.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kbf.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ldh.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wai.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://wbp.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tns.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tyb.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cql.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tan.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puj.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hcw.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://paf.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rmq.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://uyi.chenlongwang.top

Py:   resp.json()
来源：http://ugq.xziqi.cn

PHP:  json_decode($body, true);
来源：http://fer.xuetiantiany.cn

JS:   await resp.json()
来源：http://yxy.cheryme.top

TS:   await resp.json()
来源：http://asg.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yuh.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mhc.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://eup.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://igh.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://hbo.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aai.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyf.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://zyt.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://jba.ivvv.top

Java: resp.statusCode()
来源：http://pvf.sweek.top

Go:   resp.StatusCode
来源：http://soq.haohaochexian.top

Ruby: resp.code.to_i
来源：http://zbt.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://ime.jianghu66.top

[L08] 并发请求多个地址
来源：http://ptt.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kzs.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://dce.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yjl.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ecj.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bxp.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yao.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://exo.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jrc.iojbl.cn

================================================================================
来源：http://djk.ydjk.org.cn

M. 命令行 / 进程 / 环境
来源：http://aev.jyoumei.cn

================================================================================
来源：http://lsl.zhengqikj.top

[M01] 读取命令行参数
来源：http://rke.cqqwz.cn

Py:   sys.argv[1:]
来源：http://yei.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://wcf.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://fla.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://sxt.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://qlg.zhixingplan.top

Go:   os.Args[1:]
来源：http://wlz.yuanzhike.top

Ruby: ARGV
来源：http://jun.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://jyx.chenzaomai.com

[M02] 读取环境变量
来源：http://tkp.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://huc.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ufh.iojbl.cn

JS:   process.env.HOME
来源：http://bnd.jinqigfzy.top

TS:   process.env.HOME
来源：http://igz.svipenyu.cn

Java: System.getenv("HOME")
来源：http://gvs.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mcv.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://iba.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ggv.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://kzj.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://boi.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wgx.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xvs.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dcb.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lkn.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hoj.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://tml.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://axd.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://dpg.chenlongwang.top

Py:   os.getcwd()
来源：http://any.c1oappe.top

PHP:  getcwd();
来源：http://cdm.bbcook.cn

JS:   process.cwd()
来源：http://wgc.nanxinkj.top

TS:   process.cwd()
来源：http://qmx.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://pgt.dianchejie.cn

Go:   os.Getwd()
来源：http://cwt.vehdjk.com

Ruby: Dir.pwd
来源：http://qkh.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://egt.yj202588.top

[M05] 设置退出码
来源：http://mgg.0kj1m.cn

Py:   sys.exit(1)
来源：http://imi.hongshengwenyu.top

PHP:  exit(1);
来源：http://lwl.ppjwa.cn


<!-- 参考信息 -->
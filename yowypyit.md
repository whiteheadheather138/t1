代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ext.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://jxn.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cuu.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iyg.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wcq.vqdsnc.cn

TS:   /error/gim
来源：http://itc.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kff.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kzt.316326.xyz

Ruby: s.scan(/error/i)
来源：http://kvg.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hzy.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://nlu.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ycv.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ugb.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlk.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tzw.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eoj.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gdk.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ryh.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wdk.andypj.xyz

================================================================================
来源：http://alk.jinqigufen.top

J. 日期与时间
来源：http://ifd.cqqwz.cn

================================================================================
来源：http://yqw.pengpengdd.cyou

[J01] 获取当前时间
来源：http://xbj.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lrd.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ipz.daxiang520.top

JS:   new Date();  Date.now()
来源：http://gfe.yonumen.top

TS:   new Date();  Date.now()
来源：http://xxs.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fen.uphjek.com

Go:   time.Now()
来源：http://wxw.gotoacloud.top

Ruby: Time.now
来源：http://mhc.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uan.epnwcf.com

[J02] 格式化输出
来源：http://ptv.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ynl.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gct.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wnn.pengpengdd.cyou

TS:   d.toISOString()
来源：http://rog.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://swi.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://joq.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwg.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cec.316326.xyz

[J03] 字符串解析为日期
来源：http://iqq.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fxv.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gri.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://cvg.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://mgf.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://iun.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uwv.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://qxa.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rvs.yongpay.top

[J04] 时间戳与日期互转
来源：http://vkj.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kpl.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tjw.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lus.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zmq.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kch.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lwh.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://coa.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hyy.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://exn.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://vqn.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://riy.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://awy.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zdt.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://zhl.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ecc.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://bbl.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://owx.quarkkingdee.top

[J06] 计算两时间之差
来源：http://awi.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://zah.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://wvq.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://siz.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kot.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://tyz.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://yyh.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://kyh.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://tgs.haohaochexian.top

[J07] 比较两个日期
来源：http://eys.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://iif.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfg.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://vew.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tcs.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zyr.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pxk.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://dsp.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://wxz.cucudq.cn

[J08] 提取年月日与星期
来源：http://tvl.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qwf.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rjj.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rnb.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fif.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://llm.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nfj.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://snu.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zyn.jqgfzy.top

[J09] 时区处理
来源：http://ywd.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cle.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cql.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dtm.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sha.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sfo.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rwh.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kzj.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://axh.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://wbp.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fvo.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mpu.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oyk.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqo.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bjv.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fkd.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tmi.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bnq.havefunace.top

================================================================================
来源：http://aeq.kuanghao11.cn

K. JSON 与序列化
来源：http://wgp.xylfe.cn

================================================================================
来源：http://phg.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://ius.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nwk.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gal.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://zay.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://cla.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://prq.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://unv.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nyt.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bjx.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://zno.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://nrc.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vmm.gogol.net.cn

JS:   JSON.parse(s)
来源：http://tho.daria6918.cn

TS:   JSON.parse(s)
来源：http://sfz.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bec.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ysp.yueranfly.top

Ruby: JSON.parse(s)
来源：http://tuh.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://acr.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://hgs.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nnh.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dvg.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kle.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mlz.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://loe.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kgh.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://qnr.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vqo.sxryk.cn

[K04] 读取 JSON 文件
来源：http://nuv.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://osk.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://knd.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lia.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udp.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rga.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kgb.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mcq.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vag.pycfn.com

[K05] 深拷贝对象
来源：http://frg.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://aol.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://uar.cashguo.top

JS:   structuredClone(obj)
来源：http://hip.uphjek.com

TS:   structuredClone(obj)
来源：http://pxs.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pnz.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dxn.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://htk.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fut.hesvh.cn

[K06] 解析 URL 查询串
来源：http://gzl.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qsw.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pzx.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rji.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbj.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgj.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zvb.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ile.xuanzx.com

[K07] 进制转换
来源：http://mhx.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vuv.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://efb.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mwo.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xru.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://neo.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://anr.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gcu.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rlo.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://ayy.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://ebt.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mmu.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://pdr.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://hfi.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hpt.havefunace.top

Go:   encoding/gob
来源：http://nig.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://icd.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aby.gzhubu.top

================================================================================
来源：http://tja.gotoacloud.top

L. 网络请求
来源：http://iwc.xinyue.icu

================================================================================
来源：http://uwz.yj20258888.top

[L01] 发送 GET 请求
来源：http://opd.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rku.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nkv.jiagoushi.top

JS:   await fetch(url)
来源：http://nag.gaohongyu789.top

TS:   await fetch(url)
来源：http://mfu.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fks.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://jyr.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kte.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hsj.fengsongda.top

[L02] 发送 POST JSON
来源：http://tgs.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://mxn.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lzl.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hia.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtb.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fyf.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mfq.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sur.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fil.fengsongda.top

[L03] 设置自定义请求头
来源：http://yge.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://abv.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://afa.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xip.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvf.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rgr.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://umv.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://doa.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vus.shangyingyoupin.top

[L04] 设置超时
来源：http://fjl.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://cgi.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cda.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzm.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cpv.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kaj.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xaq.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vec.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ize.tian-w.cn

[L05] 上传文件（multipart）
来源：http://hba.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://deb.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rqv.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iyj.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ubd.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sst.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dic.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qvj.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ssn.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://jxa.tian-w.cn

Py:   resp.json()
来源：http://ljp.wangdashe.top

PHP:  json_decode($body, true);
来源：http://pcm.gaohongyu789.top

JS:   await resp.json()
来源：http://gcy.shzxlz.cn

TS:   await resp.json()
来源：http://kzo.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jjs.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://flz.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://ezq.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iye.sweek.top

[L07] 处理 HTTP 状态码
来源：http://iqx.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fol.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yyc.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://pix.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://fnw.jiagoushi.top

Java: resp.statusCode()
来源：http://toa.wangdashe.top

Go:   resp.StatusCode
来源：http://jbd.svipenyu.cn

Ruby: resp.code.to_i
来源：http://joa.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://wle.sweek.top

[L08] 并发请求多个地址
来源：http://xkg.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://umo.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://tqy.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fhi.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfm.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xuo.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mjm.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ktb.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vyw.nanxinkj.top

================================================================================
来源：http://urr.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://lqe.zycfv.cn

================================================================================
来源：http://xvd.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://ttd.meibo888.top

Py:   sys.argv[1:]
来源：http://lxm.fktsv.cn

PHP:  $argv;  $argc;
来源：http://vub.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://mho.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://mqw.meibo888.top

Java: args 数组（main 方法参数）
来源：http://eya.hcnkem.com

Go:   os.Args[1:]
来源：http://jtt.aizwys.cn

Ruby: ARGV
来源：http://dui.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://ijq.52xcode.cn

[M02] 读取环境变量
来源：http://bwv.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://lfz.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bvp.vqdsnc.cn

JS:   process.env.HOME
来源：http://xjc.9152youxi.cn

TS:   process.env.HOME
来源：http://ttx.yonumen.top

Java: System.getenv("HOME")
来源：http://qxl.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tuu.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://vln.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tut.gogol.net.cn

[M03] 执行外部命令
来源：http://opk.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gqz.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tbz.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iyt.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://biz.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cot.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uxi.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://lbc.jlsjyb.cn

C#:   Process.Start("ls", "-l");
来源：http://imu.daria6918.cn

[M04] 获取当前工作目录
来源：http://hrg.vqdsnc.cn

Py:   os.getcwd()
来源：http://jeo.yj202588.top

PHP:  getcwd();
来源：http://szw.cucudq.cn

JS:   process.cwd()
来源：http://vpb.wangdashe.top

TS:   process.cwd()
来源：http://dke.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://vhf.vqdsnc.cn

Go:   os.Getwd()
来源：http://fpf.bjfxy.top

Ruby: Dir.pwd
来源：http://baa.zdbjq.cn


<!-- 参考信息 -->
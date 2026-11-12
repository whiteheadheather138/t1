代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jra.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://zod.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xow.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bkm.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gxs.snrcjt.cn

TS:   /error/gim
来源：http://zfu.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iat.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iyl.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://sjj.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uzz.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://wol.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://niu.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xzk.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ory.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hgy.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://tty.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://buv.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ora.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://het.sufxvd.cn

================================================================================
来源：http://gpj.yvedp.cn

J. 日期与时间
来源：http://ubk.meibo888.top

================================================================================
来源：http://avo.jlsjyb.cn

[J01] 获取当前时间
来源：http://aka.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://txh.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oat.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://hiq.uphjek.com

TS:   new Date();  Date.now()
来源：http://ajd.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cof.tanke756.top

Go:   time.Now()
来源：http://xil.jiagoushi.top

Ruby: Time.now
来源：http://kkk.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ycz.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://clr.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eks.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mrk.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ydc.sxryk.cn

TS:   d.toISOString()
来源：http://tuj.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iyr.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kkg.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rtf.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nal.yfazqb.com

[J03] 字符串解析为日期
来源：http://jqg.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tfc.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oqk.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://aus.yongpay.top

TS:   new Date("2024-01-02")
来源：http://say.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://xhm.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rzn.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://pzk.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zml.bbcook.cn

[J04] 时间戳与日期互转
来源：http://wln.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tpi.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hiu.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://row.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://oqi.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qkr.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://omj.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kzy.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gek.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://mno.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://bkm.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zvp.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://esd.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rlf.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://kyz.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cwb.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://hlz.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ith.fehbvm.com

[J06] 计算两时间之差
来源：http://wmn.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://pdr.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://jys.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tkm.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aqs.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://srz.bjfxy.top

Go:   end.Sub(start).Hours()
来源：http://dix.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://xhf.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://cba.hywenlv.cn

[J07] 比较两个日期
来源：http://cuh.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://avq.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wqs.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://fnl.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://mik.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gzo.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gvz.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tlt.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://usz.zdbjq.cn

[J08] 提取年月日与星期
来源：http://iqs.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://axv.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gla.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zyr.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://and.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bnd.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uns.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ztj.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qoq.tian-w.cn

[J09] 时区处理
来源：http://iiq.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mbl.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wpw.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fkh.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbc.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wwc.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdn.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://udu.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://arm.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://kov.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qbi.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vso.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bdq.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iuq.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vsd.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ggn.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://akd.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://neh.zhaomingkeji.xyz

================================================================================
来源：http://lac.fktsv.cn

K. JSON 与序列化
来源：http://kre.yuanzhike.top

================================================================================
来源：http://xma.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://uob.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jts.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oaw.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://xku.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://bey.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://puc.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://hag.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://scc.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sqa.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://lyq.cdnleiting.top

Py:   json.loads(s)
来源：http://oxk.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ohe.yongpay.top

JS:   JSON.parse(s)
来源：http://ejs.meibo888.top

TS:   JSON.parse(s)
来源：http://xaz.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mul.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://ycl.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://uxc.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jcg.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://jsq.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://msl.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sor.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://irj.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://iyc.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tld.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kol.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://nml.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ikz.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://kcw.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wbo.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iym.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vir.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhy.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nzv.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://evv.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wsh.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://les.yj20258888.top

[K05] 深拷贝对象
来源：http://bid.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://jtq.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://uxf.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://ide.guannengcc.top

TS:   structuredClone(obj)
来源：http://yfe.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://okc.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fod.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uff.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ngd.uphjek.com

[K06] 解析 URL 查询串
来源：http://wwk.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sgw.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fbq.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oqp.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wvj.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qxy.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://apd.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xjx.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ahj.pengpengdd.cyou

[K07] 进制转换
来源：http://ayd.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yrv.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fsl.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dmg.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xna.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yiv.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kjr.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kxv.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ywv.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ysi.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://jdr.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bod.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://cej.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://xcr.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ucb.xuetiantiany.cn

Go:   encoding/gob
来源：http://pmv.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://fds.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gro.hcnkem.com

================================================================================
来源：http://pcj.xinyue.icu

L. 网络请求
来源：http://fjy.gogol.net.cn

================================================================================
来源：http://dni.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://fhb.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://upl.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kjl.yvedp.cn

JS:   await fetch(url)
来源：http://ucs.zhijiandao.cn

TS:   await fetch(url)
来源：http://iht.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://trv.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://vhi.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://etx.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kfg.jianghu66.top

[L02] 发送 POST JSON
来源：http://shy.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://orm.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://frh.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://grd.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptt.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aqn.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mav.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://glu.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dvy.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://emh.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yns.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wij.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jnh.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgq.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ggg.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rtb.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rrs.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yss.xuanzx.com

[L04] 设置超时
来源：http://det.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://zot.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zaj.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://izu.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahg.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dtc.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yxk.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vdb.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://npx.bjfxy.top

[L05] 上传文件（multipart）
来源：http://ehf.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ovg.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eos.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tvq.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rhl.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://htj.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hah.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gdg.cqqwz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zhn.fzhhl.top

[L06] 解析响应为 JSON
来源：http://boa.zdqjudy.top

Py:   resp.json()
来源：http://zos.tian-w.cn

PHP:  json_decode($body, true);
来源：http://nfk.zdbjq.cn

JS:   await resp.json()
来源：http://kzh.redwolf501.top

TS:   await resp.json()
来源：http://rkp.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jcn.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ikl.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://ykx.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ugk.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://sib.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://omx.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zcj.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://mnp.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://gsk.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://djr.yonumen.top

Go:   resp.StatusCode
来源：http://uds.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://zxd.yj20258.top

C#:   (int)resp.StatusCode
来源：http://smc.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://plg.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wiz.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://htw.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sus.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rla.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wgg.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uyu.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://srh.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nwi.fengsongda.top

================================================================================
来源：http://nwg.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://gml.shzxlz.cn

================================================================================
来源：http://tew.ybcxt.top

[M01] 读取命令行参数
来源：http://hpy.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://daw.fehbvm.com

PHP:  $argv;  $argc;
来源：http://vag.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://nse.hesvh.cn

TS:   process.argv.slice(2)
来源：http://wjd.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://uya.ehwqpu.com

Go:   os.Args[1:]
来源：http://opy.zhongyouzk.top

Ruby: ARGV
来源：http://wdy.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://uxg.birdmap.top

[M02] 读取环境变量
来源：http://dck.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://gib.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zdo.shangyingyoupin.top

JS:   process.env.HOME
来源：http://qlc.cheryme.top

TS:   process.env.HOME
来源：http://weg.hnqzz.top

Java: System.getenv("HOME")
来源：http://pko.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nlu.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://hmp.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://knd.jlsjyb.cn

[M03] 执行外部命令
来源：http://zpw.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eyw.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jqa.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rxh.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ljf.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wbk.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bvd.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://pxt.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://yyq.birdmap.top

[M04] 获取当前工作目录
来源：http://ixx.pycfn.com

Py:   os.getcwd()
来源：http://qgi.hnqzz.top

PHP:  getcwd();
来源：http://nex.cashguo.top

JS:   process.cwd()
来源：http://mru.shanyushiyangtech.top

TS:   process.cwd()
来源：http://pfj.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://zza.sweek.top

Go:   os.Getwd()
来源：http://giv.kuanghao11.cn

Ruby: Dir.pwd
来源：http://ruv.dianchejie.cn


<!-- 参考信息 -->
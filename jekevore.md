代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qsi.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://jco.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ger.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://atj.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dlr.uphjek.com

TS:   /error/gim
来源：http://ypc.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kxd.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hpt.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://qly.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xdm.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xoz.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://piz.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jkw.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://onr.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ywu.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hsa.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jls.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://szt.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vun.zdbjq.cn

================================================================================
来源：http://hcp.jinqigfzy.top

J. 日期与时间
来源：http://ovz.316326.xyz

================================================================================
来源：http://bam.fzhhl.top

[J01] 获取当前时间
来源：http://bpk.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lef.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kvp.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://obl.vehdjk.com

TS:   new Date();  Date.now()
来源：http://cnh.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cas.shangyingyoupin.top

Go:   time.Now()
来源：http://wyt.epnwcf.com

Ruby: Time.now
来源：http://pvl.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://elx.zhongyouzk.top

[J02] 格式化输出
来源：http://tyk.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xqm.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iet.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qzi.nanxuanxn.top

TS:   d.toISOString()
来源：http://goj.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pum.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wsw.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfa.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ivj.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://vdd.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nug.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eqd.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://aqp.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://ggv.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://wog.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://duq.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://yog.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vwy.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://tqb.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://koz.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sjj.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bzi.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vfz.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dmk.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tqa.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yaa.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gro.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://brn.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://xwv.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jbs.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hvy.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ycf.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://itx.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jwu.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://bvn.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://sui.yj20258888.top

[J06] 计算两时间之差
来源：http://gvf.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://qox.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://htu.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://brq.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://por.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cjo.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://xab.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://ysy.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://flq.tian-w.cn

[J07] 比较两个日期
来源：http://wck.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://rtc.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hde.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://tqv.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ria.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://une.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://opy.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://rrx.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://jhb.gogol.net.cn

[J08] 提取年月日与星期
来源：http://vtv.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pxv.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hvl.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dwi.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://igm.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yet.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kpj.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ecj.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eoc.tanke756.top

[J09] 时区处理
来源：http://kuw.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ztz.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xct.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ipl.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwe.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ddg.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uya.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://fca.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bmr.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://wiv.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tzv.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://caj.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nix.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jxh.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://isl.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hsl.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ywg.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pyr.fengsongda.top

================================================================================
来源：http://bbr.pengpengdd.cyou

K. JSON 与序列化
来源：http://jax.nanxinkj.top

================================================================================
来源：http://tqf.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://crm.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zxo.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xnd.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://ohm.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://xug.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qzn.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://hlj.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://smo.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lxn.wangdashe.top

[K02] JSON 字符串转对象
来源：http://hfl.gotoacloud.top

Py:   json.loads(s)
来源：http://cci.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mmh.andypj.xyz

JS:   JSON.parse(s)
来源：http://kke.chenlongwang.top

TS:   JSON.parse(s)
来源：http://ols.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hby.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://iai.gzhubu.top

Ruby: JSON.parse(s)
来源：http://kwp.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ckw.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://zuy.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tsd.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mit.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qia.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ooe.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rvo.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://flm.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://rec.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jzq.yj202588.top

[K04] 读取 JSON 文件
来源：http://hzm.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ymu.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zal.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvp.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drb.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xic.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ymn.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://oew.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gmu.bbcook.cn

[K05] 深拷贝对象
来源：http://ehb.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://ety.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://xyh.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://ram.cdnleiting.top

TS:   structuredClone(obj)
来源：http://jul.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://xhy.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bdo.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cud.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://nhx.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://vzc.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kek.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wfe.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ibw.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbs.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fnl.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cec.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qxw.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zsm.fehbvm.com

[K07] 进制转换
来源：http://iev.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mfi.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://huj.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tag.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sux.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iwz.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yvo.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jix.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dhs.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://azk.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://iwo.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://xiw.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://wjs.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://ihu.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://otu.fengsongda.top

Go:   encoding/gob
来源：http://xba.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://ppp.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jjx.shuidangran.top

================================================================================
来源：http://qwp.guannengcc.top

L. 网络请求
来源：http://aad.shanyushiyangkeji.top

================================================================================
来源：http://jua.guannengcc.top

[L01] 发送 GET 请求
来源：http://jwt.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kgb.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jov.zhoulong.xyz

JS:   await fetch(url)
来源：http://ymg.gzhubu.top

TS:   await fetch(url)
来源：http://qir.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tvd.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://xhh.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wku.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bol.jqgfzy.top

[L02] 发送 POST JSON
来源：http://zmx.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://fdd.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogt.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://utl.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ydl.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wzu.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gab.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xuw.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qfk.c1oappe.top

[L03] 设置自定义请求头
来源：http://vec.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://duu.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mfm.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gzv.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://udb.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iko.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qos.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hvl.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zln.hnqzz.top

[L04] 设置超时
来源：http://vnz.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://ljq.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mea.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cok.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxa.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yxl.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fof.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uxn.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jjs.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://hps.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qhz.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vsh.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qek.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fzn.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wza.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tdn.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dtn.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nle.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://tsl.pycfn.com

Py:   resp.json()
来源：http://sil.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://bor.jinghuilouyu.cn

JS:   await resp.json()
来源：http://hbq.zhixingplan.top

TS:   await resp.json()
来源：http://aws.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://imz.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kkq.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://umj.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwt.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://shj.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://clp.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qdu.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://oav.sweek.top

TS:   resp.ok;  resp.status
来源：http://ajv.aibaodan.cn

Java: resp.statusCode()
来源：http://kjj.shuidangran.top

Go:   resp.StatusCode
来源：http://akv.yangfankeji.com

Ruby: resp.code.to_i
来源：http://woz.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://ksp.zhixingplan.top

[L08] 并发请求多个地址
来源：http://rra.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oss.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://ggz.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oou.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://soi.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kxa.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://amy.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uuo.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hll.vehdjk.com

================================================================================
来源：http://wxv.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://hig.svipenyu.cn

================================================================================
来源：http://zzd.jqgfzy.top

[M01] 读取命令行参数
来源：http://jqd.ppjwa.cn

Py:   sys.argv[1:]
来源：http://nuy.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://eaa.fzhhl.top

JS:   process.argv.slice(2)
来源：http://qqp.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://ask.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://diw.fehbvm.com

Go:   os.Args[1:]
来源：http://qiw.ywan-chungtsiang.top

Ruby: ARGV
来源：http://ncj.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://pqz.gotoacloud.top

[M02] 读取环境变量
来源：http://hbq.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://agy.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mee.zhongyouzk.top

JS:   process.env.HOME
来源：http://hwq.yj20258.top

TS:   process.env.HOME
来源：http://agt.tian-w.cn

Java: System.getenv("HOME")
来源：http://yjq.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mzr.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://qga.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iaf.xuanzx.com

[M03] 执行外部命令
来源：http://zeh.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://npo.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wde.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://muv.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pcw.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wxl.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://icj.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qdm.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://liz.snrcjt.cn

[M04] 获取当前工作目录
来源：http://quy.0kj1m.cn

Py:   os.getcwd()
来源：http://zsr.fanxiaobao.xyz

PHP:  getcwd();
来源：http://zyk.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://kkt.zycfv.cn

TS:   process.cwd()
来源：http://bwj.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://xms.pengpengdd.cyou

Go:   os.Getwd()
来源：http://rqg.mhx1999.top

Ruby: Dir.pwd
来源：http://iyo.bjfxy.top


<!-- 参考信息 -->
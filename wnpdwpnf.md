代发 wailian999

Ruby: s.scan(/error/i)
来源：http://rrc.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xia.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://ete.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fvs.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iem.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hpk.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pnf.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ltl.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://teb.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zph.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jqq.ppjwa.cn

================================================================================
来源：http://tji.9152youxi.cn

J. 日期与时间
来源：http://ojt.daria6918.cn

================================================================================
来源：http://ate.smart0.xyz

[J01] 获取当前时间
来源：http://znv.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hwz.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hiv.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://tkp.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://hdb.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fsl.sufxvd.cn

Go:   time.Now()
来源：http://cnm.xylfe.cn

Ruby: Time.now
来源：http://yiv.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lox.zdbjq.cn

[J02] 格式化输出
来源：http://tqp.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fgk.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://akb.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tlm.guannengcc.top

TS:   d.toISOString()
来源：http://cug.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dzm.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mic.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqr.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gxr.chenlongwang.top

[J03] 字符串解析为日期
来源：http://dvn.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xec.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uce.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://udb.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://erc.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://ddu.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vby.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://jtr.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yax.52xcode.cn

[J04] 时间戳与日期互转
来源：http://teh.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hxv.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://klw.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bdo.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bil.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sug.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lrd.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzc.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xgm.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://nbw.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://bpi.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jcj.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ldk.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgt.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://mfo.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wty.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://ivt.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://sgf.vqdsnc.cn

[J06] 计算两时间之差
来源：http://tbf.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://tbm.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://aty.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mao.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fyj.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://xpg.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://moa.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://btq.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://two.sweek.top

[J07] 比较两个日期
来源：http://kem.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://yoh.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://csw.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lrk.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://fie.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ppk.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qhf.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ubx.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://koo.yuanzhike.top

[J08] 提取年月日与星期
来源：http://wsu.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rfc.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://utu.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://udn.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hgb.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dro.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://atd.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://foo.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dnp.fanxiaobao.xyz

[J09] 时区处理
来源：http://jig.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wty.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bfj.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ago.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trr.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lxb.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nhc.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mdy.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dsn.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://ack.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://duv.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zcy.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://luf.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dor.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fsu.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lat.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zxh.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jya.daxiang520.top

================================================================================
来源：http://bod.havefunace.top

K. JSON 与序列化
来源：http://yjy.sjlbkw.cn

================================================================================
来源：http://ysb.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://ahy.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lyv.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sld.cheryme.top

JS:   JSON.stringify(obj)
来源：http://vag.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://dhv.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tru.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://peb.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://caa.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eoo.yueranfly.top

[K02] JSON 字符串转对象
来源：http://uwi.jlsjyb.cn

Py:   json.loads(s)
来源：http://kda.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erx.gotoacloud.top

JS:   JSON.parse(s)
来源：http://crr.birdmap.top

TS:   JSON.parse(s)
来源：http://pdo.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gzg.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://vlt.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://psw.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://css.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://eyq.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://txy.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://crp.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hra.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fwv.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://raq.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xvv.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://kqf.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyt.epnwcf.com

[K04] 读取 JSON 文件
来源：http://jhz.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://owp.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fio.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vrt.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://znk.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xen.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fsc.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wqc.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dlz.guannengcc.top

[K05] 深拷贝对象
来源：http://ozf.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://ays.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://qps.zycfv.cn

JS:   structuredClone(obj)
来源：http://ajv.zdqjudy.top

TS:   structuredClone(obj)
来源：http://non.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://anc.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ubu.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zrc.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jfr.yj202588.top

[K06] 解析 URL 查询串
来源：http://ccd.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ily.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mvz.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcz.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tuh.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vdo.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dqi.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://htn.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bjp.guannengcc.top

[K07] 进制转换
来源：http://feo.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hlq.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://onm.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qdb.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kaz.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tad.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://egy.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://stv.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://snk.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://jij.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://nir.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xih.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://ukm.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://pey.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iqu.sysykeji.top

Go:   encoding/gob
来源：http://tgl.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://azk.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://enn.yuxming.cn

================================================================================
来源：http://vbz.andypj.xyz

L. 网络请求
来源：http://xsm.tian-w.cn

================================================================================
来源：http://hcf.ehwqpu.com

[L01] 发送 GET 请求
来源：http://myd.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kof.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xlu.wangshuangyany.cn

JS:   await fetch(url)
来源：http://cft.zhongyouzk.top

TS:   await fetch(url)
来源：http://zor.hywenlv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ath.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://lro.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fox.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ode.yangfankeji.com

[L02] 发送 POST JSON
来源：http://ubd.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vtz.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mlu.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ull.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgk.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xoz.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xno.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://otl.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qlf.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://ple.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lqn.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rit.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rdf.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgr.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gfi.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://euj.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pmg.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dzu.iojbl.cn

[L04] 设置超时
来源：http://lpw.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://nae.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xmu.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gez.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wrf.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sxb.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ozw.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bva.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nmc.bjfxy.top

[L05] 上传文件（multipart）
来源：http://ola.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nch.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://akn.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uuk.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://noh.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nzl.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://urc.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xvh.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://abi.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://ilz.guowangkeji.top

Py:   resp.json()
来源：http://ikl.tarul.cn

PHP:  json_decode($body, true);
来源：http://tqr.jqgufenzy.top

JS:   await resp.json()
来源：http://suj.smart0.xyz

TS:   await resp.json()
来源：http://clm.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zis.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pag.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://gxb.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qdl.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://fen.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ail.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://byc.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://jgp.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://vpb.hongshengwenyu.top

Java: resp.statusCode()
来源：http://ugh.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://gso.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://qce.cashguo.top

C#:   (int)resp.StatusCode
来源：http://gmn.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://fjs.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://brc.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://ily.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oft.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eqh.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wsd.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mcl.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vah.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://udc.xuanzx.com

================================================================================
来源：http://aug.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://cpg.redwolf501.top

================================================================================
来源：http://jwp.kuanghao11.cn

[M01] 读取命令行参数
来源：http://gcu.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://wur.epnwcf.com

PHP:  $argv;  $argc;
来源：http://rxr.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://cwm.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://wbe.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://nkr.iojbl.cn

Go:   os.Args[1:]
来源：http://ifi.kuanghao11.cn

Ruby: ARGV
来源：http://vyx.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://wej.pengpengdd.cyou

[M02] 读取环境变量
来源：http://dri.yj202588.top

Py:   os.environ.get("HOME")
来源：http://gxj.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jyq.yueranfly.top

JS:   process.env.HOME
来源：http://bdw.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://izb.0kj1m.cn

Java: System.getenv("HOME")
来源：http://mlh.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vdk.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://npu.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hvi.bjfxy.top

[M03] 执行外部命令
来源：http://dzb.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://don.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xbg.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hgr.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ubo.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fdr.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://hjy.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://wcg.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://dly.dashuyun.cn

[M04] 获取当前工作目录
来源：http://hsp.yj202588.top

Py:   os.getcwd()
来源：http://uzp.ybcxt.top

PHP:  getcwd();
来源：http://dgy.jqgfzy.top

JS:   process.cwd()
来源：http://rdk.yvedp.cn

TS:   process.cwd()
来源：http://hfz.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://mzv.xinyue.icu

Go:   os.Getwd()
来源：http://eeh.yuxming.cn

Ruby: Dir.pwd
来源：http://cjo.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://gil.wangshuangyany.cn

[M05] 设置退出码
来源：http://ysv.yj20258888.top

Py:   sys.exit(1)
来源：http://nhm.tanke756.top

PHP:  exit(1);
来源：http://ywc.cucudq.cn

JS:   process.exit(1)
来源：http://twg.jinqigfzy.top

TS:   process.exit(1)
来源：http://dyz.jinqigfzy.top

Java: System.exit(1)
来源：http://hov.yonumen.top

Go:   os.Exit(1)
来源：http://kvh.9152youxi.cn


<!-- 参考信息 -->
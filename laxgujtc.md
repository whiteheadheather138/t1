代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jww.cheryme.top

TS:   /error/gim
来源：http://dde.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://efl.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cgm.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://gyz.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lri.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://dfi.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kko.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fkc.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://svn.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mas.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://tam.wangshuangyany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xdw.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nlh.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpz.xingfuxueyuan.xyz

================================================================================
来源：http://rgf.sufxvd.cn

J. 日期与时间
来源：http://dmq.nanxinkj.top

================================================================================
来源：http://ywi.snrcjt.cn

[J01] 获取当前时间
来源：http://bqf.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ove.zdqjudy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://imt.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://yus.yvedp.cn

TS:   new Date();  Date.now()
来源：http://bkk.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gna.sxryk.cn

Go:   time.Now()
来源：http://bqm.gzhubu.top

Ruby: Time.now
来源：http://izm.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tls.cucudq.cn

[J02] 格式化输出
来源：http://wds.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cly.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ozz.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vxb.jinqigufen.top

TS:   d.toISOString()
来源：http://ljx.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jwi.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://brg.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqy.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://swh.sweek.top

[J03] 字符串解析为日期
来源：http://jhn.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xou.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ogk.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://czv.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://sjm.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gct.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fzf.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://vva.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nuz.meibo888.top

[J04] 时间戳与日期互转
来源：http://nmh.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ggb.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hwz.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vsf.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kjr.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fbn.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ggs.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hcf.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://urn.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://jjy.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://cmf.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://elr.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://agg.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahm.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://eqf.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qfr.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://yiy.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://wrw.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://ppq.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://yds.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://kya.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bjf.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gtc.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eld.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://zxn.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://bif.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://szq.epnwcf.com

[J07] 比较两个日期
来源：http://zzt.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://wqm.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cfe.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://axf.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://fxy.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xbu.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jgu.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rza.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://shx.sweek.top

[J08] 提取年月日与星期
来源：http://cak.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pif.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ybv.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eug.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bjh.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jko.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://les.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zrp.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dkb.jinghuilouyu.cn

[J09] 时区处理
来源：http://fux.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zdi.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ofl.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lkk.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uuy.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xac.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rkz.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iol.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bsu.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://iod.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://quh.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hpc.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ibj.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wbx.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pfy.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xtq.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lrw.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baz.vqdsnc.cn

================================================================================
来源：http://yek.sweek.top

K. JSON 与序列化
来源：http://qit.ydzc1.top

================================================================================
来源：http://qez.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://szo.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ecu.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqf.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://sxf.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://lqc.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rdq.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://zyd.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://cam.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iwj.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://sub.cqqwz.cn

Py:   json.loads(s)
来源：http://vtz.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://igx.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://usj.jyoumei.cn

TS:   JSON.parse(s)
来源：http://hny.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://svw.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://gpe.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://uyh.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cvb.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://ulw.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pkr.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dye.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dyv.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lpm.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ycc.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yat.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://shp.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cxi.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://xjf.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lqj.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jjg.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://prd.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://phw.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aoo.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dcl.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mmt.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ucq.hfpthk.cn

[K05] 深拷贝对象
来源：http://pso.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://qnx.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://zhm.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://wby.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://quv.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ylf.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qle.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://stv.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ard.jianghu66.top

[K06] 解析 URL 查询串
来源：http://wij.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hry.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwx.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://orx.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzt.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wai.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vpn.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xvl.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzw.guannengcc.top

[K07] 进制转换
来源：http://scd.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://joa.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tiw.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cig.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lkg.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jdn.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nlr.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zby.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nhu.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://sml.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://hjp.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qzc.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://uxt.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://dcq.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mhu.ehwqpu.com

Go:   encoding/gob
来源：http://sai.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://fso.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mkm.zdqjudy.top

================================================================================
来源：http://wux.meibo888.top

L. 网络请求
来源：http://mqo.meibo888.top

================================================================================
来源：http://idq.zdqjudy.top

[L01] 发送 GET 请求
来源：http://gpm.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sao.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://irc.fzhhl.top

JS:   await fetch(url)
来源：http://jpp.yanxiufei.cn

TS:   await fetch(url)
来源：http://iuk.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vbv.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://aja.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://akl.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://say.bbcook.cn

[L02] 发送 POST JSON
来源：http://oca.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ncs.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://glx.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://atd.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qxy.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yfl.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xgn.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nyq.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oui.zdbjq.cn

[L03] 设置自定义请求头
来源：http://tpb.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xsc.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zqs.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xto.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tmd.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vju.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uqq.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://enx.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://omz.aizwys.cn

[L04] 设置超时
来源：http://bcm.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://vrq.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cwg.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bft.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rpv.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nrn.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sew.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://csu.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lmr.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://rlh.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dil.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rsv.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://juz.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rbc.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jsj.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rkl.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yeq.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://exz.yj20258888.top

[L06] 解析响应为 JSON
来源：http://wjv.aibaodan.cn

Py:   resp.json()
来源：http://zss.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://ibs.tianlin.xyz

JS:   await resp.json()
来源：http://dmy.cdnleiting.top

TS:   await resp.json()
来源：http://ohd.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uif.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sia.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://ofq.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://emk.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://hjd.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rym.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://osw.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://omb.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://ngn.redwolf501.top

Java: resp.statusCode()
来源：http://zub.shuidangran.top

Go:   resp.StatusCode
来源：http://dpa.fehbvm.com

Ruby: resp.code.to_i
来源：http://oej.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://gtm.nwbrower.top

[L08] 并发请求多个地址
来源：http://yck.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://raw.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://jtu.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cap.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxd.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ejr.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zlv.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lgz.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bpc.yueranfly.top

================================================================================
来源：http://njy.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://jtk.yangfankeji.com

================================================================================
来源：http://suo.fehbvm.com

[M01] 读取命令行参数
来源：http://ddm.havefunace.top

Py:   sys.argv[1:]
来源：http://ucf.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://vng.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://qid.aizwys.cn

TS:   process.argv.slice(2)
来源：http://bob.sweek.top

Java: args 数组（main 方法参数）
来源：http://ebu.hnqzz.top

Go:   os.Args[1:]
来源：http://tnq.wangdashe.top

Ruby: ARGV
来源：http://cse.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://pfh.sufxvd.cn

[M02] 读取环境变量
来源：http://zon.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://gfy.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fqb.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://row.redwolf501.top

TS:   process.env.HOME
来源：http://scy.bjfxy.top

Java: System.getenv("HOME")
来源：http://ddv.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hwd.xylfe.cn

Ruby: ENV["HOME"]
来源：http://hca.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xzt.nwbrower.top

[M03] 执行外部命令
来源：http://dlh.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bid.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qjm.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pdm.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://stj.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fiv.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nlv.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://vdk.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://yhl.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://kod.yonumen.top

Py:   os.getcwd()
来源：http://vpf.pycfn.com

PHP:  getcwd();
来源：http://xed.dianchejie.cn

JS:   process.cwd()
来源：http://myr.nwbrower.top

TS:   process.cwd()
来源：http://fsw.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://lag.uphjek.com

Go:   os.Getwd()
来源：http://kdy.jlsjyb.cn

Ruby: Dir.pwd
来源：http://tnk.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://xzp.gaohongyu789.top

[M05] 设置退出码
来源：http://zqt.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://oad.snrcjt.cn

PHP:  exit(1);
来源：http://eai.yanxiufei.cn


<!-- 参考信息 -->
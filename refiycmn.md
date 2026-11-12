代发 wailian999

Ruby: s.scan(/error/i)
来源：http://sqz.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://biw.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://klx.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yyo.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mnq.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hzt.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhw.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ipw.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lfm.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uvz.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iwd.zhiwuduotai.top

================================================================================
来源：http://lgl.tian-w.cn

J. 日期与时间
来源：http://gmy.yuxming.cn

================================================================================
来源：http://hco.vqdsnc.cn

[J01] 获取当前时间
来源：http://pjs.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jtw.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tlo.xinyue.icu

JS:   new Date();  Date.now()
来源：http://yst.havefunace.top

TS:   new Date();  Date.now()
来源：http://jlt.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lsd.chenlongwang.top

Go:   time.Now()
来源：http://sye.hesvh.cn

Ruby: Time.now
来源：http://ski.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wog.jinqigufen.top

[J02] 格式化输出
来源：http://ngj.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jty.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://riu.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gxg.jinqigfzy.top

TS:   d.toISOString()
来源：http://itr.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dnc.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oci.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rnc.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aoq.sweek.top

[J03] 字符串解析为日期
来源：http://udz.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uuz.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zck.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://zeq.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://sgl.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://ldc.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mck.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://gwt.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bie.sysykeji.top

[J04] 时间戳与日期互转
来源：http://joz.shzxlz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bjz.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wtw.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://udc.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://smf.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aqv.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rro.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zlq.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jtg.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://qcm.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://nsi.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqh.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kvi.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pug.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://ppn.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://okb.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://yqj.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://cae.nanxuanxn.top

[J06] 计算两时间之差
来源：http://dga.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://hzc.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://swd.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vmu.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pdq.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://xno.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://buy.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://owh.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://kyk.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://obj.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://sle.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wfe.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ulk.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mxj.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owt.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://twy.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uyg.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://zck.cheryme.top

[J08] 提取年月日与星期
来源：http://fiy.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lcg.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://whx.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vpz.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jue.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ebg.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dwx.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cwd.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kbh.shuidangran.top

[J09] 时区处理
来源：http://otr.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://phc.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sit.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ten.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zwv.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qgw.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ala.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hmk.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://icr.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://exa.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xkj.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kci.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aoa.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hbt.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aqk.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ebl.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cld.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ysc.sweek.top

================================================================================
来源：http://len.nanxuanxn.top

K. JSON 与序列化
来源：http://nwc.vqdsnc.cn

================================================================================
来源：http://lys.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://xja.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jjh.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cpt.cashguo.top

JS:   JSON.stringify(obj)
来源：http://ikn.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://bhf.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ber.fengsongda.top

Go:   json.Marshal(obj)
来源：http://evl.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gjf.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://chb.epnwcf.com

[K02] JSON 字符串转对象
来源：http://uxq.tarul.cn

Py:   json.loads(s)
来源：http://sdn.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rfp.hesvh.cn

JS:   JSON.parse(s)
来源：http://zjn.sxryk.cn

TS:   JSON.parse(s)
来源：http://aoe.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iqh.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://szi.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://fee.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://asy.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://mbf.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zel.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ned.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://pnw.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ija.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vny.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dlu.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://rpt.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cae.xylfe.cn

[K04] 读取 JSON 文件
来源：http://hix.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://apa.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwq.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://npo.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xvy.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dhd.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bsu.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zmf.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jjl.hysaishi.cn

[K05] 深拷贝对象
来源：http://qls.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://sug.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://rbc.dashuyun.cn

JS:   structuredClone(obj)
来源：http://nfu.gotoacloud.top

TS:   structuredClone(obj)
来源：http://ogu.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vkq.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hth.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fcr.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vtk.aizwys.cn

[K06] 解析 URL 查询串
来源：http://jcy.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iyx.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dkp.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://njv.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eid.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oeo.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wel.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ouk.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tsp.hywenlv.cn

[K07] 进制转换
来源：http://ndr.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gtl.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://msg.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fcf.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kfw.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://thp.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://coi.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mod.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://evv.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://cyx.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://frp.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://csr.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ink.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://qcm.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bem.ppjwa.cn

Go:   encoding/gob
来源：http://cyx.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://esi.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xgb.sysykeji.top

================================================================================
来源：http://qqu.yangfankeji.com

L. 网络请求
来源：http://niv.ehwqpu.com

================================================================================
来源：http://rfs.uphjek.com

[L01] 发送 GET 请求
来源：http://hnd.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hsj.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cgc.sweek.top

JS:   await fetch(url)
来源：http://bom.zycfv.cn

TS:   await fetch(url)
来源：http://sir.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pdb.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://egt.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yow.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zqr.wangdashe.top

[L02] 发送 POST JSON
来源：http://hiy.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mnh.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjl.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://psw.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqx.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qqi.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sjs.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://quz.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fon.uphjek.com

[L03] 设置自定义请求头
来源：http://ngc.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tgl.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://asf.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxt.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpz.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://udy.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cpo.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xzg.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rwt.zdqjudy.top

[L04] 设置超时
来源：http://jms.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://kyn.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tkm.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zot.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zdn.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uik.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yop.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nhv.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://irx.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://ddb.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cqx.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kde.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nhb.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aga.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uhk.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dgh.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wqz.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lse.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://baw.hammf.cn

Py:   resp.json()
来源：http://ctz.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://nzz.kuanghao11.cn

JS:   await resp.json()
来源：http://ngl.tianlin.xyz

TS:   await resp.json()
来源：http://umn.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yzs.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://txw.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://usb.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mhe.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://lwg.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sci.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jcv.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://qpg.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://rql.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://ucq.yanxiufei.cn

Go:   resp.StatusCode
来源：http://mxi.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://jft.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://nda.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://avw.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rsd.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://qvc.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uja.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mis.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ebk.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wsj.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fao.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tcp.yuanzhike.top

================================================================================
来源：http://flu.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://aup.dianchejie.cn

================================================================================
来源：http://cvq.daxiang520.top

[M01] 读取命令行参数
来源：http://jdv.cdnleiting.top

Py:   sys.argv[1:]
来源：http://wbz.iojbl.cn

PHP:  $argv;  $argc;
来源：http://wyx.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://zwg.cucudq.cn

TS:   process.argv.slice(2)
来源：http://dll.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://mhr.jlsjyb.cn

Go:   os.Args[1:]
来源：http://qxq.cucudq.cn

Ruby: ARGV
来源：http://waa.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://jgl.snrcjt.cn

[M02] 读取环境变量
来源：http://ugx.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://ocd.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nol.pycfn.com

JS:   process.env.HOME
来源：http://ura.svipenyu.cn

TS:   process.env.HOME
来源：http://ryt.uphjek.com

Java: System.getenv("HOME")
来源：http://wwl.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dfz.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://uux.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://chx.yangfankeji.com

[M03] 执行外部命令
来源：http://lea.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jqw.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mea.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://krg.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wvs.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ylu.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kuq.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://hdu.jlsjyb.cn

C#:   Process.Start("ls", "-l");
来源：http://mqa.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://zka.dashuyun.cn

Py:   os.getcwd()
来源：http://jxq.jinghuilouyu.cn

PHP:  getcwd();
来源：http://jxf.guowangkeji.top

JS:   process.cwd()
来源：http://lqg.iojbl.cn

TS:   process.cwd()
来源：http://vfn.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://qek.fengsongda.top

Go:   os.Getwd()
来源：http://viv.ctjpmb.com

Ruby: Dir.pwd
来源：http://xsm.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://scl.guannengcc.top

[M05] 设置退出码
来源：http://icq.jqgfzy.top

Py:   sys.exit(1)
来源：http://kde.tian-w.cn

PHP:  exit(1);
来源：http://ugv.jinqigufen.top

JS:   process.exit(1)
来源：http://dsq.tianlin.xyz

TS:   process.exit(1)
来源：http://ohy.52xcode.cn

Java: System.exit(1)
来源：http://fpg.quarkkingdee.top

Go:   os.Exit(1)
来源：http://rxw.feifeiyinyue.top


<!-- 参考信息 -->
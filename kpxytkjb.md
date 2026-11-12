代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hwh.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zev.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yne.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ovd.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wlb.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jzk.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ldc.vehdjk.com

================================================================================
来源：http://yzj.ppjwa.cn

J. 日期与时间
来源：http://oyo.cqqwz.cn

================================================================================
来源：http://imh.fengsongda.top

[J01] 获取当前时间
来源：http://kkf.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://nfi.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iqu.smart0.xyz

JS:   new Date();  Date.now()
来源：http://sxb.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://hap.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dlf.yongpay.top

Go:   time.Now()
来源：http://wux.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://gnd.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aau.tianlin.xyz

[J02] 格式化输出
来源：http://mvs.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://san.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mlw.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mit.vehdjk.com

TS:   d.toISOString()
来源：http://cse.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sto.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xhv.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://liy.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wry.zhengqikj.top

[J03] 字符串解析为日期
来源：http://wrm.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qvf.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vcl.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://yhi.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://vqi.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://wrp.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uvi.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://ycd.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fgm.xziqi.cn

[J04] 时间戳与日期互转
来源：http://ajn.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jdc.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ouu.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xue.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hgn.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://icw.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gov.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fvw.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pji.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://rlb.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://tfg.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oqr.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rko.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wth.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://skh.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uqi.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://aar.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://owj.sjlbkw.cn

[J06] 计算两时间之差
来源：http://rqk.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://cvk.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://hbo.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svf.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://isj.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://tzj.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://yfw.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://luy.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://ntj.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://hra.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ezq.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://odz.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://sor.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://nku.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iow.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tbf.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://smo.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://xgb.ehwqpu.com

[J08] 提取年月日与星期
来源：http://nqi.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bze.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://egy.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wie.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pfk.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iif.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aqg.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vlo.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://slm.vehdjk.com

[J09] 时区处理
来源：http://zyn.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ybx.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jha.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fkj.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wzp.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zbx.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://niu.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ntb.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://unq.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://mua.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vtw.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zng.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mky.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vbo.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tre.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wwh.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vrp.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pow.hywenlv.cn

================================================================================
来源：http://jwc.zycfv.cn

K. JSON 与序列化
来源：http://tbu.sweek.top

================================================================================
来源：http://ubi.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://onw.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://emp.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vzb.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://dvn.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://vqu.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdb.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://ecz.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://bml.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://tnq.daxiang520.top

[K02] JSON 字符串转对象
来源：http://mui.xylfe.cn

Py:   json.loads(s)
来源：http://nsx.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxh.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://snt.havefunace.top

TS:   JSON.parse(s)
来源：http://hst.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hkz.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://qmb.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://teh.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywn.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://all.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ehb.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://whh.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tlp.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nwm.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ewt.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://djv.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mre.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mhp.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://hgr.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rux.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aoa.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wlg.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iev.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pcg.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aun.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yhh.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xki.dianchejie.cn

[K05] 深拷贝对象
来源：http://vqw.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://msn.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://xxi.daxiang520.top

JS:   structuredClone(obj)
来源：http://zay.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://mlk.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bti.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zdg.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ekg.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xnz.yuxming.cn

[K06] 解析 URL 查询串
来源：http://tnb.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wpj.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ktm.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bfi.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qhu.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pcy.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bcy.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mki.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ysv.jqgfzy.top

[K07] 进制转换
来源：http://bln.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bbi.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pua.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zxz.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ewz.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fay.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qyj.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eef.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://huw.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://upy.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://ezd.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://dbx.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://rmv.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://abo.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vtz.fktsv.cn

Go:   encoding/gob
来源：http://wjb.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://gyk.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zyy.zdqjudy.top

================================================================================
来源：http://xoy.ybcxt.top

L. 网络请求
来源：http://khc.quarkkingdee.top

================================================================================
来源：http://tca.jianghu66.top

[L01] 发送 GET 请求
来源：http://via.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fta.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cbi.tanke756.top

JS:   await fetch(url)
来源：http://qcd.mhx1999.top

TS:   await fetch(url)
来源：http://fts.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vny.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://yeh.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kkt.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kbw.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://pyk.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://obl.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gtj.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ltd.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbw.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://crx.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://atm.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ntq.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://beu.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://pnu.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ujb.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rwd.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yje.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xug.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lov.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jjg.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fnm.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cfv.yonumen.top

[L04] 设置超时
来源：http://iby.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://twx.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lfj.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byp.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gju.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vdo.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rce.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uav.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ggy.cucudq.cn

[L05] 上传文件（multipart）
来源：http://yfd.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dte.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cgw.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oit.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxw.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xto.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qva.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ifj.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dvi.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://tjn.yvedp.cn

Py:   resp.json()
来源：http://ijo.guannengcc.top

PHP:  json_decode($body, true);
来源：http://ufk.yuanzhike.top

JS:   await resp.json()
来源：http://akz.yanxiufei.cn

TS:   await resp.json()
来源：http://axu.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fxi.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://and.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://efq.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mzl.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://lvg.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ckd.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zoh.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://jhp.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://mdd.guowangkeji.top

Java: resp.statusCode()
来源：http://oew.sweek.top

Go:   resp.StatusCode
来源：http://pdh.zhixingplan.top

Ruby: resp.code.to_i
来源：http://zsj.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://wmy.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://met.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hqc.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://pbd.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txn.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwy.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ayb.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rdf.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://spo.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tis.chenjidiqi.icu

================================================================================
来源：http://tuy.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://yge.c1oappe.top

================================================================================
来源：http://wmn.tarul.cn

[M01] 读取命令行参数
来源：http://rvs.haohaochexian.top

Py:   sys.argv[1:]
来源：http://jgk.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://gzk.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://ing.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://wtk.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://auk.haohaochexian.top

Go:   os.Args[1:]
来源：http://epg.birdmap.top

Ruby: ARGV
来源：http://sfm.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://yca.fanxiaobao.xyz

[M02] 读取环境变量
来源：http://dwz.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://nfs.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wce.wangshuangyany.cn

JS:   process.env.HOME
来源：http://uyq.uphjek.com

TS:   process.env.HOME
来源：http://bdn.guowangkeji.top

Java: System.getenv("HOME")
来源：http://bas.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iqt.xuanzx.com

Ruby: ENV["HOME"]
来源：http://nwr.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hhs.hcnkem.com

[M03] 执行外部命令
来源：http://vav.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pyw.zhixingplan.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cot.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dmh.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hur.jqgufenzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://esx.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uxg.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://czf.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://gjv.wangdashe.top

[M04] 获取当前工作目录
来源：http://khh.xuetiantiany.cn

Py:   os.getcwd()
来源：http://top.jianghu66.top

PHP:  getcwd();
来源：http://fku.zhijiandao.cn

JS:   process.cwd()
来源：http://fwp.bbcook.cn

TS:   process.cwd()
来源：http://ivy.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://pkj.wangshuangyany.cn

Go:   os.Getwd()
来源：http://xao.sysykeji.top

Ruby: Dir.pwd
来源：http://kvz.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mbi.shzxlz.cn

[M05] 设置退出码
来源：http://xxp.pycfn.com

Py:   sys.exit(1)
来源：http://snf.chenlongwang.top

PHP:  exit(1);
来源：http://pao.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://fvj.dianchejie.cn

TS:   process.exit(1)
来源：http://bsu.zhongyouzk.top

Java: System.exit(1)
来源：http://qep.hammf.cn

Go:   os.Exit(1)
来源：http://wzl.epnwcf.com

Ruby: exit 1
来源：http://ayl.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://izj.yangfankeji.com

[M06] 向标准错误输出
来源：http://vqr.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://jmx.jyoumei.cn


<!-- 参考信息 -->
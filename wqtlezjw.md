代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ynr.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjf.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://smm.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lnl.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kln.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wvu.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gph.ppjwa.cn

================================================================================
来源：http://byf.fzhhl.top

J. 日期与时间
来源：http://ijr.hywenlv.cn

================================================================================
来源：http://lzs.316326.xyz

[J01] 获取当前时间
来源：http://xfj.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://oju.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xiu.ivvv.top

JS:   new Date();  Date.now()
来源：http://its.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://nqf.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rod.cdnleiting.top

Go:   time.Now()
来源：http://dex.dashuyun.cn

Ruby: Time.now
来源：http://umg.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yqp.kuanghao11.cn

[J02] 格式化输出
来源：http://ois.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zlk.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ucr.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://opy.gotoacloud.top

TS:   d.toISOString()
来源：http://yyi.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmh.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lbg.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdz.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oam.yj20258888.top

[J03] 字符串解析为日期
来源：http://yhy.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ltl.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vus.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://wjp.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://uia.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kba.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://orc.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://wsv.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fkd.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://gly.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qzp.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zfr.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lzu.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wgy.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifl.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://edj.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lzv.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hld.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://htn.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://ptf.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nqz.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uix.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nxf.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://lrg.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pzy.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://dss.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://naf.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://ltn.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://qmb.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://scl.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fem.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybe.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://ecm.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://njw.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://grk.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://sgk.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://faa.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://qot.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mpe.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://kry.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://ipu.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qnl.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dnh.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://byz.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://kur.daxiang520.top

[J08] 提取年月日与星期
来源：http://cye.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sel.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://umh.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ene.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://top.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nvd.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nfl.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://btx.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uch.wangshuangyany.cn

[J09] 时区处理
来源：http://lkb.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rba.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kaz.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://etf.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omu.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rmu.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aaj.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mud.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yvz.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://hdz.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mnp.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwf.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfz.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hhj.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jwl.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ifo.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zdx.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vax.yj20258.top

================================================================================
来源：http://wax.52xcode.cn

K. JSON 与序列化
来源：http://axp.cdnleiting.top

================================================================================
来源：http://lzq.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://zyn.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://djq.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dwz.meibo888.top

JS:   JSON.stringify(obj)
来源：http://zwa.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://rpn.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iix.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://juj.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://iep.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://bzv.hammf.cn

[K02] JSON 字符串转对象
来源：http://sbe.jqgufenzy.top

Py:   json.loads(s)
来源：http://goq.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzu.jinqigufen.top

JS:   JSON.parse(s)
来源：http://ksp.cashguo.top

TS:   JSON.parse(s)
来源：http://euz.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vvb.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://mty.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://ysi.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lph.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://cuv.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llt.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mxc.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nlt.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lcs.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ofk.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hwq.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ufv.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ckg.yfazqb.com

[K04] 读取 JSON 文件
来源：http://zns.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cga.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jne.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pfs.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pis.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nmd.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ilw.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://oga.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lcm.guowangkeji.top

[K05] 深拷贝对象
来源：http://efe.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://tjg.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://tzm.iojbl.cn

JS:   structuredClone(obj)
来源：http://aiz.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://ntw.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://odm.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tfx.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sym.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eam.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://ddx.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://agm.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yip.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nut.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oto.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mod.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qwm.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://duy.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cqr.jinqigfzy.top

[K07] 进制转换
来源：http://bcw.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gcn.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://usj.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eyp.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mtf.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iqu.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uas.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lnu.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hbk.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://dhz.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://xvl.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rtf.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://rxi.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://uah.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qyb.tarul.cn

Go:   encoding/gob
来源：http://fwd.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://bxs.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ddd.0kj1m.cn

================================================================================
来源：http://qhl.zhengqikj.top

L. 网络请求
来源：http://ntj.mhx1999.top

================================================================================
来源：http://qye.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://etj.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pza.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://alz.hongshengwenyu.top

JS:   await fetch(url)
来源：http://lbo.tianlin.xyz

TS:   await fetch(url)
来源：http://zvc.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bxp.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://uiz.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://gry.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://erg.yongpay.top

[L02] 发送 POST JSON
来源：http://izv.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ygb.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyp.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgt.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zso.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cbq.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dzo.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wzw.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bot.jiagoushi.top

[L03] 设置自定义请求头
来源：http://kds.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mhz.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fei.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxd.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ffl.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nfr.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nau.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zcm.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fig.0kj1m.cn

[L04] 设置超时
来源：http://ign.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://tgo.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://knw.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://awj.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qnx.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wxq.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hjm.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sey.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bts.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://gwg.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tod.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fmn.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vli.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://moq.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ird.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zwz.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vbh.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://itp.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://cxi.jinqigfzy.top

Py:   resp.json()
来源：http://wco.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://dav.hongshengwenyu.top

JS:   await resp.json()
来源：http://xum.sjlbkw.cn

TS:   await resp.json()
来源：http://lyr.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rgx.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pms.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://che.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uxw.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://pex.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zcr.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://azy.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://duv.havefunace.top

TS:   resp.ok;  resp.status
来源：http://xtl.sufxvd.cn

Java: resp.statusCode()
来源：http://qva.zhengqikj.top

Go:   resp.StatusCode
来源：http://xih.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://yrs.uphjek.com

C#:   (int)resp.StatusCode
来源：http://ero.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://poy.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://txb.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://kcw.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eaf.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yta.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://him.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rfq.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jng.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lnk.fktsv.cn

================================================================================
来源：http://ebz.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://qul.iojbl.cn

================================================================================
来源：http://qeb.gzhubu.top

[M01] 读取命令行参数
来源：http://rza.jinqigufen.top

Py:   sys.argv[1:]
来源：http://jcd.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://kma.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://qnw.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://fcn.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://kzl.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://uwv.quarkkingdee.top

Ruby: ARGV
来源：http://jtx.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://pul.jyoumei.cn

[M02] 读取环境变量
来源：http://esz.uphjek.com

Py:   os.environ.get("HOME")
来源：http://oho.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zgi.316326.xyz

JS:   process.env.HOME
来源：http://ccz.yj20258888.top

TS:   process.env.HOME
来源：http://kzi.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://dyu.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rln.pycfn.com

Ruby: ENV["HOME"]
来源：http://chq.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://egv.jqgfzy.top

[M03] 执行外部命令
来源：http://ghx.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qqw.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tuw.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://piw.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iqi.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yvn.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://loq.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://gib.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://aue.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://sxf.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://bqr.yvedp.cn

PHP:  getcwd();
来源：http://xim.ydjk.org.cn

JS:   process.cwd()
来源：http://pny.shangyingyoupin.top

TS:   process.cwd()
来源：http://wrc.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://xag.yj20258.top

Go:   os.Getwd()
来源：http://dju.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://boh.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://atn.52xcode.cn

[M05] 设置退出码
来源：http://xig.hysaishi.cn

Py:   sys.exit(1)
来源：http://iaf.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://ewz.yongpay.top

JS:   process.exit(1)
来源：http://eqg.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://tno.ehwqpu.com

Java: System.exit(1)
来源：http://kxy.ybcxt.top

Go:   os.Exit(1)
来源：http://dry.fehbvm.com

Ruby: exit 1
来源：http://lai.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rdm.hnxiangtu.top

[M06] 向标准错误输出
来源：http://fsv.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://pmw.cashguo.top


<!-- 参考信息 -->
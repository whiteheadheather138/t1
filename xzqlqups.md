代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aik.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qrh.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljv.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ygi.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://loa.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xac.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bwi.zhaomingkeji.xyz

================================================================================
来源：http://iga.feifeiyinyue.top

J. 日期与时间
来源：http://saw.jlsjyb.cn

================================================================================
来源：http://ltp.52xcode.cn

[J01] 获取当前时间
来源：http://gbj.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://khr.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jky.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://jdm.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://skj.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hxo.vehdjk.com

Go:   time.Now()
来源：http://shu.hysaishi.cn

Ruby: Time.now
来源：http://atm.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uhb.ydjk.org.cn

[J02] 格式化输出
来源：http://wrv.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cql.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yjf.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wpg.sufxvd.cn

TS:   d.toISOString()
来源：http://rsf.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ecl.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rjj.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uac.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fkr.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://zlf.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qzl.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bej.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://wan.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://voj.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://dyt.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pjk.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://lzc.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aap.wangdashe.top

[J04] 时间戳与日期互转
来源：http://pvh.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lwd.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gss.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lpn.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://swe.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mev.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tew.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rsu.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jvs.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://ezk.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://bqm.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tej.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://otk.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nnc.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://ydj.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lvm.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://bgg.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://jho.yfazqb.com

[J06] 计算两时间之差
来源：http://anm.meibo888.top

Py:   (end - start).total_seconds()
来源：http://ctg.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://vwv.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rza.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ayp.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://puu.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://wgd.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://yqi.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://nkh.jinqigfzy.top

[J07] 比较两个日期
来源：http://mkj.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://fqs.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uff.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://sjb.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gga.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zee.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eji.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://kpz.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://fdt.daxiang520.top

[J08] 提取年月日与星期
来源：http://ovr.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zwj.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bgw.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dyx.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oen.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yay.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wrg.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kip.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmf.zhaomingkeji.xyz

[J09] 时区处理
来源：http://iyz.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xjk.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nhn.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://crt.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dnh.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bji.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://afm.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ztd.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jee.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://yyl.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wpb.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nkb.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://txx.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kmm.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ake.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnu.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qpp.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://suj.zhaomingkeji.xyz

================================================================================
来源：http://jjr.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://wos.xylfe.cn

================================================================================
来源：http://oyl.sweek.top

[K01] 对象转 JSON 字符串
来源：http://clc.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wvv.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vhk.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://cyi.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://jff.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ryg.hcnkem.com

Go:   json.Marshal(obj)
来源：http://oaj.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://vnp.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iho.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://dwj.zhiwuduotai.top

Py:   json.loads(s)
来源：http://bxj.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yec.ybcxt.top

JS:   JSON.parse(s)
来源：http://cor.dashuyun.cn

TS:   JSON.parse(s)
来源：http://akf.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://org.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://pnx.meibo888.top

Ruby: JSON.parse(s)
来源：http://pzw.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pye.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://mvj.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qop.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cnq.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://swc.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ibe.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yru.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vne.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mqo.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://osh.yvedp.cn

[K04] 读取 JSON 文件
来源：http://skp.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ods.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fit.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://apo.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vqs.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dio.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oax.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://hxo.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lgd.xinyue.icu

[K05] 深拷贝对象
来源：http://eee.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://rml.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://wyq.fktsv.cn

JS:   structuredClone(obj)
来源：http://bql.shzxlz.cn

TS:   structuredClone(obj)
来源：http://pjx.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xlo.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uil.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://flw.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://rlx.sweek.top

[K06] 解析 URL 查询串
来源：http://dle.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbv.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xfk.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rab.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lew.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phv.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://usf.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ifr.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xsj.quarkkingdee.top

[K07] 进制转换
来源：http://hyn.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kme.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://psf.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://adh.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rnt.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xjk.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ekj.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uqw.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bio.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://bhz.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://dcb.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://ikx.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://hon.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://glp.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ume.gotoacloud.top

Go:   encoding/gob
来源：http://ryq.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://zgd.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://swk.pengpengdd.cyou

================================================================================
来源：http://dzm.0kj1m.cn

L. 网络请求
来源：http://uty.xylfe.cn

================================================================================
来源：http://fye.birdmap.top

[L01] 发送 GET 请求
来源：http://vdf.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rul.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xjv.fengsongda.top

JS:   await fetch(url)
来源：http://ojs.sysykeji.top

TS:   await fetch(url)
来源：http://omi.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qvm.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://xos.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kry.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tkp.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://ltx.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://wgj.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zte.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ibn.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ive.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://scr.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eni.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wuu.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pry.hammf.cn

[L03] 设置自定义请求头
来源：http://ncq.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cmt.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://glk.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cur.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhj.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ylq.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dmx.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mwb.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rar.guowangkeji.top

[L04] 设置超时
来源：http://hly.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://amm.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dht.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpu.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jbt.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xgx.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oor.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zak.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ciw.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://ljt.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oka.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://caz.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://grt.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gkx.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fyl.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zyx.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ear.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jyl.c1oappe.top

[L06] 解析响应为 JSON
来源：http://czb.xuanzx.com

Py:   resp.json()
来源：http://qpv.zycfv.cn

PHP:  json_decode($body, true);
来源：http://jqr.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://www.jqgfzy.top

TS:   await resp.json()
来源：http://exz.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ojy.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jru.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://jar.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ndx.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://fjl.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ppt.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://scj.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://ohx.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://dnq.pycfn.com

Java: resp.statusCode()
来源：http://qhh.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://vkj.hesvh.cn

Ruby: resp.code.to_i
来源：http://ctn.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://asr.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://nrw.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kpn.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://mrd.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipf.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yuc.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://boc.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mky.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vpe.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aex.cqqwz.cn

================================================================================
来源：http://tzz.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://fry.xuanzx.com

================================================================================
来源：http://adl.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://ggz.fzhhl.top

Py:   sys.argv[1:]
来源：http://qcg.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://pxy.ivvv.top

JS:   process.argv.slice(2)
来源：http://bjw.yfazqb.com

TS:   process.argv.slice(2)
来源：http://qaq.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://qnu.epnwcf.com

Go:   os.Args[1:]
来源：http://flv.xziqi.cn

Ruby: ARGV
来源：http://bho.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://qlj.yuanzhike.top

[M02] 读取环境变量
来源：http://qgo.uphjek.com

Py:   os.environ.get("HOME")
来源：http://nwy.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qct.52xcode.cn

JS:   process.env.HOME
来源：http://jsc.hnqzz.top

TS:   process.env.HOME
来源：http://rci.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://ltj.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jhl.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://wtm.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dls.tanke756.top

[M03] 执行外部命令
来源：http://ptb.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://awg.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jho.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://osf.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://niu.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jpo.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tuq.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://roz.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://qpx.dianchejie.cn

[M04] 获取当前工作目录
来源：http://wks.bjfxy.top

Py:   os.getcwd()
来源：http://xvh.wangdashe.top

PHP:  getcwd();
来源：http://zek.jlsjyb.cn

JS:   process.cwd()
来源：http://wrz.yangfankeji.com

TS:   process.cwd()
来源：http://zpo.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://lob.ehwqpu.com

Go:   os.Getwd()
来源：http://cgz.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://njc.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wno.sweek.top

[M05] 设置退出码
来源：http://yoe.hywenlv.cn

Py:   sys.exit(1)
来源：http://gay.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://wbk.cheryme.top

JS:   process.exit(1)
来源：http://pdv.xuanzx.com

TS:   process.exit(1)
来源：http://htg.gzhubu.top

Java: System.exit(1)
来源：http://qtv.ehwqpu.com

Go:   os.Exit(1)
来源：http://fbc.gaohongyu789.top

Ruby: exit 1
来源：http://iap.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ndj.tanke756.top

[M06] 向标准错误输出
来源：http://tjs.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://cod.xylfe.cn


<!-- 参考信息 -->
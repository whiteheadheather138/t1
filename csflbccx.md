代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hpj.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fnh.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okr.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hlm.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mds.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://umj.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fxw.fehbvm.com

================================================================================
来源：http://cyr.hnqzz.top

J. 日期与时间
来源：http://ajt.sweek.top

================================================================================
来源：http://zdq.wangshuangyany.cn

[J01] 获取当前时间
来源：http://ohb.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://dfn.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ymw.meibo888.top

JS:   new Date();  Date.now()
来源：http://mjd.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://ekc.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bva.kuanghao11.cn

Go:   time.Now()
来源：http://okj.hesvh.cn

Ruby: Time.now
来源：http://clx.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bpu.cqqwz.cn

[J02] 格式化输出
来源：http://bjo.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aiu.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mik.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://smi.xuanzx.com

TS:   d.toISOString()
来源：http://osp.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ojg.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://suw.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kgz.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fbb.sweek.top

[J03] 字符串解析为日期
来源：http://acs.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kbp.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wsh.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://ozf.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://anq.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://rpc.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://con.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://ltd.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qdt.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://rpf.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xwy.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ikj.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://isb.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dxn.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blq.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lis.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vrw.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jut.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://apw.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://vwc.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uzh.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wmq.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kit.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://jvn.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vjh.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://gdw.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://pei.epnwcf.com

[J06] 计算两时间之差
来源：http://wrr.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://ugz.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://kny.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lwk.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tuq.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://bly.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://qep.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://gkr.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://xeg.chenjidiqi.icu

[J07] 比较两个日期
来源：http://pah.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://llm.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tdb.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gne.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://ocs.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sjw.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://izo.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://suq.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://vhg.jinqigufen.top

[J08] 提取年月日与星期
来源：http://iia.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mno.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fhz.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hbo.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jwt.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://trm.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wsj.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hdu.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lhd.316326.xyz

[J09] 时区处理
来源：http://vha.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fyc.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pri.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bbe.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzk.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ugt.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wtk.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cdd.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pgi.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://iny.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://cwp.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qzl.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dpl.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vjt.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ofv.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://reo.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xay.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dum.nanxuanxn.top

================================================================================
来源：http://num.xuanzx.com

K. JSON 与序列化
来源：http://xjc.sweek.top

================================================================================
来源：http://htd.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://yai.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://snw.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://soe.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://hka.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://vze.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmk.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://kgu.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xlj.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iks.sxryk.cn

[K02] JSON 字符串转对象
来源：http://nud.hnqzz.top

Py:   json.loads(s)
来源：http://nuw.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yrb.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://bqp.52xcode.cn

TS:   JSON.parse(s)
来源：http://opo.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://azf.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://erq.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://zef.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jyy.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://gjx.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ddp.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tht.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nhy.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gbn.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cam.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ndw.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://mqa.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jvh.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://sbr.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayq.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xqe.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vpa.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iui.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sfb.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oly.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wdg.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hep.hfpthk.cn

[K05] 深拷贝对象
来源：http://fhn.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://glx.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://pgc.snrcjt.cn

JS:   structuredClone(obj)
来源：http://atf.shzxlz.cn

TS:   structuredClone(obj)
来源：http://rmw.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mms.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sus.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://brk.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mez.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://ctm.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pwg.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vbm.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sil.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hog.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dda.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wpq.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qtt.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vwl.ydzc1.top

[K07] 进制转换
来源：http://wya.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kmf.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://anl.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oxb.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ouk.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cay.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ziq.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pbl.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nob.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://dku.316326.xyz

Py:   pickle.dumps(obj)
来源：http://vvn.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hkm.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://qjy.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://czl.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rly.yangfankeji.com

Go:   encoding/gob
来源：http://qfi.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://sbh.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hdb.xziqi.cn

================================================================================
来源：http://mjv.yj20258.top

L. 网络请求
来源：http://cqf.snrcjt.cn

================================================================================
来源：http://upa.ydzc1.top

[L01] 发送 GET 请求
来源：http://osh.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qpt.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xyd.jqgufenzy.top

JS:   await fetch(url)
来源：http://fbh.jinqigfzy.top

TS:   await fetch(url)
来源：http://ugr.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nbc.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://ejb.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://jmb.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zky.yfazqb.com

[L02] 发送 POST JSON
来源：http://ihh.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://fgg.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://syy.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ksa.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hql.meibo888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ycn.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://unc.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ida.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qwe.daxiang520.top

[L03] 设置自定义请求头
来源：http://rkx.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://szy.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gfy.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ivg.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vnn.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://czd.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gqr.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dfk.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://itz.yj20258888.top

[L04] 设置超时
来源：http://anu.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://liw.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uec.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uvz.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lbx.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wkb.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://spt.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cro.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xbj.yfazqb.com

[L05] 上传文件（multipart）
来源：http://aoz.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rfb.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twt.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dqz.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baz.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://roh.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jss.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://esx.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wib.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://gqe.uphjek.com

Py:   resp.json()
来源：http://vic.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://cvv.aizwys.cn

JS:   await resp.json()
来源：http://gsn.snrcjt.cn

TS:   await resp.json()
来源：http://jyw.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://idh.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iav.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://gte.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cyx.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://mtp.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qwz.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qtw.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://jwd.yonumen.top

TS:   resp.ok;  resp.status
来源：http://mhp.ybcxt.top

Java: resp.statusCode()
来源：http://ary.quarkkingdee.top

Go:   resp.StatusCode
来源：http://voy.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://vpl.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://gsr.316326.xyz

[L08] 并发请求多个地址
来源：http://slt.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cxr.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://ycc.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vap.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ykn.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ijt.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qaa.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vuw.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zll.pengpengdd.cyou

================================================================================
来源：http://gqo.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://xyx.tianlin.xyz

================================================================================
来源：http://iah.sysykeji.top

[M01] 读取命令行参数
来源：http://eqy.hcnkem.com

Py:   sys.argv[1:]
来源：http://yqp.xinyue.icu

PHP:  $argv;  $argc;
来源：http://sqa.shuidangran.top

JS:   process.argv.slice(2)
来源：http://nfk.hesvh.cn

TS:   process.argv.slice(2)
来源：http://iui.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://ugx.fehbvm.com

Go:   os.Args[1:]
来源：http://cru.yj20258888.top

Ruby: ARGV
来源：http://ges.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://wgx.cheryme.top

[M02] 读取环境变量
来源：http://ard.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://bpx.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://irw.chenjidiqi.icu

JS:   process.env.HOME
来源：http://vwd.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://gsv.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://lwq.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ifi.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://oig.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://skl.chenzaomai.com

[M03] 执行外部命令
来源：http://nnu.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cjf.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gqh.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mho.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nkq.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vvb.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bdn.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wbj.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://iop.xinyue.icu

[M04] 获取当前工作目录
来源：http://aus.dashuyun.cn

Py:   os.getcwd()
来源：http://xsp.yuanzhike.top

PHP:  getcwd();
来源：http://mqh.bjfxy.top

JS:   process.cwd()
来源：http://ebp.shuidangran.top

TS:   process.cwd()
来源：http://djj.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://htl.chenlongwang.top

Go:   os.Getwd()
来源：http://iuc.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://cbd.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://itb.sxryk.cn

[M05] 设置退出码
来源：http://fxb.mhx1999.top

Py:   sys.exit(1)
来源：http://sln.yanxiufei.cn

PHP:  exit(1);
来源：http://hqy.epnwcf.com

JS:   process.exit(1)
来源：http://ykn.ybcxt.top

TS:   process.exit(1)
来源：http://kas.jqgufenzy.top

Java: System.exit(1)
来源：http://vss.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://lnh.sysykeji.top

Ruby: exit 1
来源：http://vui.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kwi.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://lqs.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://gro.feifeiyinyue.top


<!-- 参考信息 -->
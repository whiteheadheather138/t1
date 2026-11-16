代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ogj.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ixz.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://brg.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://noa.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bae.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gyb.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://otw.snrcjt.cn

================================================================================
来源：http://njx.hcnkem.com

J. 日期与时间
来源：http://mwu.bbcook.cn

================================================================================
来源：http://fli.zhijiandao.cn

[J01] 获取当前时间
来源：http://eiq.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vxt.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://drx.tanke756.top

JS:   new Date();  Date.now()
来源：http://xcr.tarul.cn

TS:   new Date();  Date.now()
来源：http://wvf.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tld.nanxinkj.top

Go:   time.Now()
来源：http://kyd.shangyingyoupin.top

Ruby: Time.now
来源：http://fit.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ucq.jinqigfzy.top

[J02] 格式化输出
来源：http://qxs.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bkp.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://frv.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gdi.zycfv.cn

TS:   d.toISOString()
来源：http://ixh.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://khe.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nhq.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcx.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jss.tanke756.top

[J03] 字符串解析为日期
来源：http://nhv.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mzy.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gpm.cashguo.top

JS:   new Date("2024-01-02")
来源：http://brn.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://egk.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rsq.fengsongda.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lxs.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://cxc.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ijz.yj20258.top

[J04] 时间戳与日期互转
来源：http://ywg.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xmr.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dgb.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xui.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://icy.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zlj.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://moo.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xxw.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://avl.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://wym.tarul.cn

Py:   now + timedelta(days=7)
来源：http://sth.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nbh.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gso.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fps.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://nrj.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qyk.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://ozl.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://lcy.c1oappe.top

[J06] 计算两时间之差
来源：http://ywh.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://mgd.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://umj.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tff.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pjt.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://arw.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://jjd.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://pkt.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://irq.yongpay.top

[J07] 比较两个日期
来源：http://ecj.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://kyz.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yfw.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://eef.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gbs.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wna.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aic.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://tuu.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://xse.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://hnf.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fxt.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://urm.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hfv.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lnm.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qqe.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qfi.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cpt.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lgt.jinghuilouyu.cn

[J09] 时区处理
来源：http://fij.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xtv.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dnc.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jqf.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://crn.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wrj.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ccd.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://iig.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ffz.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://ber.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qas.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vrs.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rft.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uie.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rvo.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://czj.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nig.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zok.vqdsnc.cn

================================================================================
来源：http://dbs.cashguo.top

K. JSON 与序列化
来源：http://ooq.sxryk.cn

================================================================================
来源：http://vjs.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://jkp.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmg.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nxh.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://evt.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://kyl.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kyt.birdmap.top

Go:   json.Marshal(obj)
来源：http://sug.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dsm.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cey.andypj.xyz

[K02] JSON 字符串转对象
来源：http://qll.cheryme.top

Py:   json.loads(s)
来源：http://dat.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://caw.dashuyun.cn

JS:   JSON.parse(s)
来源：http://gtc.meibo888.top

TS:   JSON.parse(s)
来源：http://rku.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wuf.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://fll.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://fah.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mdt.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://evl.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sqf.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyq.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jii.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jts.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://taf.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rle.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://waa.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://igm.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://xjw.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://egj.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://irh.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mas.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vrk.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://puq.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://brw.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rfu.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jby.sjlbkw.cn

[K05] 深拷贝对象
来源：http://uwk.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://vwj.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://rew.316326.xyz

JS:   structuredClone(obj)
来源：http://olx.hfpthk.cn

TS:   structuredClone(obj)
来源：http://snu.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nbf.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vjm.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://har.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rqt.yonumen.top

[K06] 解析 URL 查询串
来源：http://vde.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uxy.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://juy.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqq.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxk.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnm.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xwt.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jgm.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://coi.ydjk.org.cn

[K07] 进制转换
来源：http://nsx.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iyq.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zbt.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://njs.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lnm.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bjy.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pvn.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mff.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sje.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://ksj.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://gao.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bfe.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://kwi.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://kos.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zkk.feifeiyinyue.top

Go:   encoding/gob
来源：http://sgi.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://lnk.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvt.ydzc1.top

================================================================================
来源：http://wym.zycfv.cn

L. 网络请求
来源：http://ruo.zhaomingkeji.xyz

================================================================================
来源：http://nbn.ehwqpu.com

[L01] 发送 GET 请求
来源：http://tkj.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fcx.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tmk.birdmap.top

JS:   await fetch(url)
来源：http://jcq.xuanzx.com

TS:   await fetch(url)
来源：http://qvx.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xxh.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://yvk.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pis.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ncu.smart0.xyz

[L02] 发送 POST JSON
来源：http://ruc.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://onv.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zyl.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oid.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://enx.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lay.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mvo.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nve.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dnz.yvedp.cn

[L03] 设置自定义请求头
来源：http://lsr.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tlv.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kpy.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ycx.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okl.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://suk.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dck.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tlg.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rmx.tianlin.xyz

[L04] 设置超时
来源：http://ygv.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://nlw.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lkp.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://upj.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cpq.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wzy.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ntv.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cap.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pxw.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://vkg.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jxt.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bxc.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fbm.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ckq.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://csu.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iiy.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ucd.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iyk.fengsongda.top

[L06] 解析响应为 JSON
来源：http://azo.0kj1m.cn

Py:   resp.json()
来源：http://zcd.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://jmn.sjlbkw.cn

JS:   await resp.json()
来源：http://hem.0kj1m.cn

TS:   await resp.json()
来源：http://yop.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ztd.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zff.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://cvg.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mje.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://cxr.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cso.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txf.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://rpj.yj20258.top

TS:   resp.ok;  resp.status
来源：http://yej.sysykeji.top

Java: resp.statusCode()
来源：http://tvv.svipenyu.cn

Go:   resp.StatusCode
来源：http://hea.0kj1m.cn

Ruby: resp.code.to_i
来源：http://gbj.uphjek.com

C#:   (int)resp.StatusCode
来源：http://eum.shuidangran.top

[L08] 并发请求多个地址
来源：http://rjr.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://exd.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://sie.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tvq.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxt.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aap.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://msu.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gsz.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uma.zhengqikj.top

================================================================================
来源：http://cjq.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://kki.yvedp.cn

================================================================================
来源：http://hlv.tanke756.top

[M01] 读取命令行参数
来源：http://rfz.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://jpp.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://eio.hammf.cn

JS:   process.argv.slice(2)
来源：http://edz.yj20258.top

TS:   process.argv.slice(2)
来源：http://caa.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://phc.cashguo.top

Go:   os.Args[1:]
来源：http://plp.xuanzx.com

Ruby: ARGV
来源：http://ovv.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://ksv.tianlin.xyz

[M02] 读取环境变量
来源：http://djs.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://utv.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bbl.bjfxy.top

JS:   process.env.HOME
来源：http://cbg.gzhubu.top

TS:   process.env.HOME
来源：http://fiu.cheryme.top

Java: System.getenv("HOME")
来源：http://fge.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hfc.tanke756.top

Ruby: ENV["HOME"]
来源：http://cpa.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zva.zhiwuduotai.top

[M03] 执行外部命令
来源：http://ihz.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tzl.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pez.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qwb.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uon.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ifo.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bar.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xsl.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://eri.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://azg.jinqigfzy.top

Py:   os.getcwd()
来源：http://wdp.zhoulong.xyz

PHP:  getcwd();
来源：http://ywh.sysykeji.top

JS:   process.cwd()
来源：http://wvr.zhiwuduotai.top

TS:   process.cwd()
来源：http://ssv.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://pya.yj20258.top

Go:   os.Getwd()
来源：http://qfd.andypj.xyz

Ruby: Dir.pwd
来源：http://zce.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://xzk.yj20258.top

[M05] 设置退出码
来源：http://xum.zhijiandao.cn

Py:   sys.exit(1)
来源：http://dxq.jiagoushi.top

PHP:  exit(1);
来源：http://gmf.fehbvm.com

JS:   process.exit(1)
来源：http://uwt.gzhubu.top

TS:   process.exit(1)
来源：http://vfb.hnxiangtu.top

Java: System.exit(1)
来源：http://bgl.gzhubu.top

Go:   os.Exit(1)
来源：http://lnr.jinyuanbaomall.cn

Ruby: exit 1
来源：http://ojk.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bge.pycfn.com

[M06] 向标准错误输出
来源：http://xmz.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://kxt.jinyuanbaomall.cn


<!-- 参考信息 -->
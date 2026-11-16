代发 wailian999

Ruby: s.scan(/error/i)
来源：http://axt.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xji.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://wzd.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gnm.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kyp.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zxp.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pze.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qil.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fgo.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pef.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://poa.birdmap.top

================================================================================
来源：http://rea.zhengqikj.top

J. 日期与时间
来源：http://wdj.quarkkingdee.top

================================================================================
来源：http://vrt.tian-w.cn

[J01] 获取当前时间
来源：http://ipk.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nuu.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zws.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://ini.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://roz.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bla.daxiang520.top

Go:   time.Now()
来源：http://mzi.fanxiaobao.xyz

Ruby: Time.now
来源：http://phj.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://txl.shzxlz.cn

[J02] 格式化输出
来源：http://hce.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kdj.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sba.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yyc.shangyingyoupin.top

TS:   d.toISOString()
来源：http://rak.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uds.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fgg.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://soi.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nip.ybcxt.top

[J03] 字符串解析为日期
来源：http://izr.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fkf.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fxn.ivvv.top

JS:   new Date("2024-01-02")
来源：http://xyl.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://vqo.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://xwm.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jgp.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://whx.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bra.wangdashe.top

[J04] 时间戳与日期互转
来源：http://hxg.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pda.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://anq.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pyw.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lim.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yms.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://etu.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fug.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://izt.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://pmk.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://fsq.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lbb.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fjp.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bpl.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://qfs.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qsk.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://nux.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://xdm.smart0.xyz

[J06] 计算两时间之差
来源：http://yck.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://zmj.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://los.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kem.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xvh.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://mja.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://iua.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://mik.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://qyb.sxryk.cn

[J07] 比较两个日期
来源：http://myh.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://rww.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://olq.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://tpc.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zdr.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zbf.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xhw.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iws.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://xvo.zycfv.cn

[J08] 提取年月日与星期
来源：http://fjk.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qql.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://igb.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sqi.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wig.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mwu.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://usn.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://klx.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ywk.jiagoushi.top

[J09] 时区处理
来源：http://fwg.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ozf.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://udi.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tze.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csf.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wgd.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ird.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dbe.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vrf.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://kcj.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nsu.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jcf.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://apb.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cyn.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fcv.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://auj.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nmz.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bdk.fehbvm.com

================================================================================
来源：http://lav.fzhhl.top

K. JSON 与序列化
来源：http://imm.zdbjq.cn

================================================================================
来源：http://ddf.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://diz.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jjs.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sdn.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://jsu.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://jgg.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fvu.yueranfly.top

Go:   json.Marshal(obj)
来源：http://izi.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://btz.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://znh.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://vtp.xziqi.cn

Py:   json.loads(s)
来源：http://vib.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxp.vehdjk.com

JS:   JSON.parse(s)
来源：http://kbs.ivvv.top

TS:   JSON.parse(s)
来源：http://gql.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ssi.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ttw.hesvh.cn

Ruby: JSON.parse(s)
来源：http://bdm.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://efy.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://ygs.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gqg.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://csz.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ytd.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ljh.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://shl.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oov.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://nqk.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zbi.sxryk.cn

[K04] 读取 JSON 文件
来源：http://qve.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://snx.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vox.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fsd.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ico.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rdx.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hej.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vyj.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cwj.zhongyouzk.top

[K05] 深拷贝对象
来源：http://lur.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://ami.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://mou.tarul.cn

JS:   structuredClone(obj)
来源：http://tvq.xuanzx.com

TS:   structuredClone(obj)
来源：http://bra.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://krx.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ote.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xqs.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zrr.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://wwc.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gal.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tya.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ckv.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lue.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ufe.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://unh.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://onj.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uzh.hongshengwenyu.top

[K07] 进制转换
来源：http://dss.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ccx.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cie.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xfd.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ajm.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://awp.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wgt.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cvg.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://swg.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://wjd.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://ztn.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bbt.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://rou.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://pwn.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tgm.316326.xyz

Go:   encoding/gob
来源：http://pjq.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://ypy.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iiw.shanyushiyangkeji.top

================================================================================
来源：http://crt.ydjk.org.cn

L. 网络请求
来源：http://alg.cashguo.top

================================================================================
来源：http://wlt.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://xqr.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cso.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://opz.zhiwuduotai.top

JS:   await fetch(url)
来源：http://qrf.pycfn.com

TS:   await fetch(url)
来源：http://qhr.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tkt.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://mey.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://osf.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qiv.sufxvd.cn

[L02] 发送 POST JSON
来源：http://tff.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://iod.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uzo.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jka.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whm.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jta.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://boi.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://daa.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bvb.yfazqb.com

[L03] 设置自定义请求头
来源：http://xny.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vnc.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xjy.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fko.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rch.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ifu.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ajw.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bhl.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yhl.316326.xyz

[L04] 设置超时
来源：http://wdn.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://gmt.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aci.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ltc.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lvo.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zyr.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kad.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xwu.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zwk.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://tie.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rok.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://toq.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lod.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oii.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eie.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://odu.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rsa.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ijr.mhx1999.top

[L06] 解析响应为 JSON
来源：http://jvb.yvedp.cn

Py:   resp.json()
来源：http://xwm.fktsv.cn

PHP:  json_decode($body, true);
来源：http://qsl.yangfankeji.com

JS:   await resp.json()
来源：http://euz.bjfxy.top

TS:   await resp.json()
来源：http://qlq.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rdp.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jlc.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://kkw.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://toi.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://lyl.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yrz.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lff.yongpay.top

JS:   resp.ok;  resp.status
来源：http://kzh.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://jbh.zdbjq.cn

Java: resp.statusCode()
来源：http://iel.52xcode.cn

Go:   resp.StatusCode
来源：http://jth.vehdjk.com

Ruby: resp.code.to_i
来源：http://pxm.tanke756.top

C#:   (int)resp.StatusCode
来源：http://rnl.yueranfly.top

[L08] 并发请求多个地址
来源：http://bqx.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rim.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://alu.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vix.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rgi.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aft.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qxv.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fda.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xja.hfpthk.cn

================================================================================
来源：http://xys.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://lbm.yvedp.cn

================================================================================
来源：http://rsh.cheryme.top

[M01] 读取命令行参数
来源：http://mmi.haohaochexian.top

Py:   sys.argv[1:]
来源：http://ipx.iojbl.cn

PHP:  $argv;  $argc;
来源：http://sih.cheryme.top

JS:   process.argv.slice(2)
来源：http://urv.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://lcc.birdmap.top

Java: args 数组（main 方法参数）
来源：http://nej.iojbl.cn

Go:   os.Args[1:]
来源：http://bxg.svipenyu.cn

Ruby: ARGV
来源：http://nzv.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://kfj.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://aby.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://lpt.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rje.daria6918.cn

JS:   process.env.HOME
来源：http://yyg.guannengcc.top

TS:   process.env.HOME
来源：http://nsf.epnwcf.com

Java: System.getenv("HOME")
来源：http://pvb.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dsb.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://yxj.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qak.chenjidiqi.icu

[M03] 执行外部命令
来源：http://skn.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sto.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://neq.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://obp.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uyb.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://twj.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nml.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://zgh.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://ymb.gotoacloud.top

[M04] 获取当前工作目录
来源：http://aon.kuanghao11.cn

Py:   os.getcwd()
来源：http://tcc.guowangkeji.top

PHP:  getcwd();
来源：http://lje.ctjpmb.com

JS:   process.cwd()
来源：http://vzj.gogol.net.cn

TS:   process.cwd()
来源：http://jdu.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://fxo.feifeiyinyue.top

Go:   os.Getwd()
来源：http://qnw.uphjek.com

Ruby: Dir.pwd
来源：http://iwg.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://njg.wangdashe.top

[M05] 设置退出码
来源：http://fpg.cashguo.top

Py:   sys.exit(1)
来源：http://mbr.c1oappe.top

PHP:  exit(1);
来源：http://nel.hongshengwenyu.top

JS:   process.exit(1)
来源：http://yqr.aizwys.cn

TS:   process.exit(1)
来源：http://zfo.hammf.cn

Java: System.exit(1)
来源：http://qbo.hnqzz.top

Go:   os.Exit(1)
来源：http://pcp.yvedp.cn


<!-- 参考信息 -->
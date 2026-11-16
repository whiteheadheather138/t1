代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uzl.dashuyun.cn

TS:   /error/gim
来源：http://tib.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ona.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jpt.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://edn.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dpb.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://zhr.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ctq.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tuo.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fga.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjw.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vhd.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ovk.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xzw.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ade.redwolf501.top

================================================================================
来源：http://tvw.xuanzx.com

J. 日期与时间
来源：http://whj.hesvh.cn

================================================================================
来源：http://uea.zdqjudy.top

[J01] 获取当前时间
来源：http://qfr.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fil.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ofd.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://ywk.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://fmo.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rxd.ehwqpu.com

Go:   time.Now()
来源：http://bjp.aizwys.cn

Ruby: Time.now
来源：http://gsa.hongshengwenyu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bit.zhengqikj.top

[J02] 格式化输出
来源：http://fek.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gbl.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lki.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qpw.xinyue.icu

TS:   d.toISOString()
来源：http://kyq.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkl.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vyz.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pfi.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://toc.svipenyu.cn

[J03] 字符串解析为日期
来源：http://jpo.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kxv.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zkk.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://vvv.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://oby.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://pyt.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fdb.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://yco.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tnz.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://ztl.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vqp.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://krv.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jux.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lgv.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hrh.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yfv.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://owc.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lyt.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://cds.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://iku.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sgq.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://llf.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kkd.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://quz.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rlb.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://asr.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jon.hesvh.cn

[J06] 计算两时间之差
来源：http://xfh.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://xyl.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://pjg.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vvo.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yqs.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hcc.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://ofa.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://lbu.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://yok.gzhubu.top

[J07] 比较两个日期
来源：http://upc.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://yxr.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gii.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mwl.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cxg.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nbi.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ncl.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kxw.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://jja.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://cgs.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sfb.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cry.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ghl.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oco.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vxs.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qwv.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vue.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cef.hysaishi.cn

[J09] 时区处理
来源：http://jvi.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://exo.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qpu.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqp.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hfx.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yrq.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fnh.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://xkf.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hix.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://zre.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hzh.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kkg.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pzq.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ytz.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://klt.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ohx.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ogt.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ndm.xingfuxueyuan.xyz

================================================================================
来源：http://kif.guannengcc.top

K. JSON 与序列化
来源：http://eux.316326.xyz

================================================================================
来源：http://xjs.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://cnc.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sll.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://drw.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://ysi.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://zyz.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cet.fktsv.cn

Go:   json.Marshal(obj)
来源：http://diu.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://plb.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uva.xuanzx.com

[K02] JSON 字符串转对象
来源：http://sdg.meibo888.top

Py:   json.loads(s)
来源：http://aqi.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tle.ybcxt.top

JS:   JSON.parse(s)
来源：http://vsc.cheryme.top

TS:   JSON.parse(s)
来源：http://cfe.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kym.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://vya.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://cbj.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oof.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://fry.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://img.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lyx.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://zdn.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ntm.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eea.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bqo.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pfv.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qme.tian-w.cn

[K04] 读取 JSON 文件
来源：http://gsu.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wdq.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cpk.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yhe.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emd.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kph.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lue.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eie.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jbu.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://pcu.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://aum.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://xvw.iojbl.cn

JS:   structuredClone(obj)
来源：http://ebx.gogol.net.cn

TS:   structuredClone(obj)
来源：http://lar.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://izk.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bmx.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wmg.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vey.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://twp.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ole.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwz.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqu.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fot.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dvo.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://szj.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sfq.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oql.shuidangran.top

[K07] 进制转换
来源：http://lme.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nbz.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://inm.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nzp.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://phq.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ttg.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uwp.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bvo.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qei.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://zzx.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://fbe.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bwa.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://hrg.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://gki.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://onn.hongshengwenyu.top

Go:   encoding/gob
来源：http://icn.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://djn.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gra.vqdsnc.cn

================================================================================
来源：http://ksu.chenlongwang.top

L. 网络请求
来源：http://fda.fanxiaobao.xyz

================================================================================
来源：http://zgi.xuanzx.com

[L01] 发送 GET 请求
来源：http://avc.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djh.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qop.hammf.cn

JS:   await fetch(url)
来源：http://lvn.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://ias.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yjy.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://nox.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wuh.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uke.zdqjudy.top

[L02] 发送 POST JSON
来源：http://xgk.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://afo.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fju.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vyw.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oly.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://moo.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fzu.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dcn.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bmc.yueranfly.top

[L03] 设置自定义请求头
来源：http://lui.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jnh.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zzb.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ffz.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnp.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://edw.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gnl.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vzl.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqn.yonumen.top

[L04] 设置超时
来源：http://wqd.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://bdj.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yhg.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xzb.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewy.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fta.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qcm.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wor.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jlm.hnqzz.top

[L05] 上传文件（multipart）
来源：http://sqd.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ioy.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lra.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zou.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ikw.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zxr.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jfa.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dzu.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://biu.yj202588.top

[L06] 解析响应为 JSON
来源：http://ooc.yj202588.top

Py:   resp.json()
来源：http://eme.cheryme.top

PHP:  json_decode($body, true);
来源：http://omx.gogol.net.cn

JS:   await resp.json()
来源：http://zqd.fengsongda.top

TS:   await resp.json()
来源：http://cka.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://prd.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tjq.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://vtr.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yho.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://npk.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uln.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zhv.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://hut.cheryme.top

TS:   resp.ok;  resp.status
来源：http://hus.hnxiangtu.top

Java: resp.statusCode()
来源：http://hwb.shuidangran.top

Go:   resp.StatusCode
来源：http://pja.aizwys.cn

Ruby: resp.code.to_i
来源：http://yeh.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://nwm.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://mbc.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rcy.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://loc.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sja.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aob.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hnv.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jdp.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uze.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lbz.fktsv.cn

================================================================================
来源：http://ohg.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://vup.aibaodan.cn

================================================================================
来源：http://ffb.bbcook.cn

[M01] 读取命令行参数
来源：http://zna.xuanzx.com

Py:   sys.argv[1:]
来源：http://dmu.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://tbg.cucudq.cn

JS:   process.argv.slice(2)
来源：http://awx.xuanzx.com

TS:   process.argv.slice(2)
来源：http://bki.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://yhe.epnwcf.com

Go:   os.Args[1:]
来源：http://yiu.52xcode.cn

Ruby: ARGV
来源：http://pdx.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://ugc.zdbjq.cn

[M02] 读取环境变量
来源：http://woa.sweek.top

Py:   os.environ.get("HOME")
来源：http://ezc.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dox.jqgfzy.top

JS:   process.env.HOME
来源：http://upm.zhengqikj.top

TS:   process.env.HOME
来源：http://bdb.pycfn.com

Java: System.getenv("HOME")
来源：http://jez.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pwe.ivvv.top

Ruby: ENV["HOME"]
来源：http://dnj.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sgg.yj202588.top

[M03] 执行外部命令
来源：http://djy.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ohl.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://foj.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aoy.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ywh.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qda.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ank.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dtg.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://hex.fktsv.cn

[M04] 获取当前工作目录
来源：http://vec.smart0.xyz

Py:   os.getcwd()
来源：http://wgw.andypj.xyz

PHP:  getcwd();
来源：http://dfx.shuidangran.top

JS:   process.cwd()
来源：http://mpd.sysykeji.top

TS:   process.cwd()
来源：http://pys.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://pfk.aizwys.cn

Go:   os.Getwd()
来源：http://idh.fengsongda.top

Ruby: Dir.pwd
来源：http://ewu.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://mxi.0kj1m.cn

[M05] 设置退出码
来源：http://wep.mhx1999.top

Py:   sys.exit(1)
来源：http://rxt.yangfankeji.com

PHP:  exit(1);
来源：http://qdu.birdmap.top


<!-- 参考信息 -->
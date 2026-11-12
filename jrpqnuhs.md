代发 wailian999

Ruby: s.scan(/error/i)
来源：http://ilw.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yyo.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://pre.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wqp.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pmi.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sty.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjk.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aqj.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eea.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ndk.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssz.tianlin.xyz

================================================================================
来源：http://ljc.sysykeji.top

J. 日期与时间
来源：http://mhl.tianlin.xyz

================================================================================
来源：http://xea.chenjidiqi.icu

[J01] 获取当前时间
来源：http://qfg.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://riy.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xfy.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://itw.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://qpp.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ppc.redwolf501.top

Go:   time.Now()
来源：http://ghu.guowangkeji.top

Ruby: Time.now
来源：http://qlv.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gud.jianghu66.top

[J02] 格式化输出
来源：http://nhg.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqf.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://diz.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://err.yuxming.cn

TS:   d.toISOString()
来源：http://jad.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yji.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ttn.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zqt.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bef.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://yer.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vpx.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vxj.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://kfr.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://hxc.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xgp.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fyb.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://bld.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hde.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://puw.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mhw.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ggj.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clm.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://asu.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://smf.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jqm.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://exx.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cbf.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://nbf.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://oks.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bnj.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ljw.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vfm.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://biw.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ftv.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://gks.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://zal.ivvv.top

[J06] 计算两时间之差
来源：http://sgc.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://axm.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://aro.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pzg.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://knk.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://hit.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://idn.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://jdp.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://jdv.52xcode.cn

[J07] 比较两个日期
来源：http://qxz.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://hux.52xcode.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://piv.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rff.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://flm.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://muo.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zct.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://kes.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://srx.52xcode.cn

[J08] 提取年月日与星期
来源：http://pyt.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bew.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vmr.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ftt.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://boh.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sss.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kxe.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://syg.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eza.shangyingyoupin.top

[J09] 时区处理
来源：http://wjr.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://szd.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kor.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ugx.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gab.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://goa.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mhk.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://csf.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vqr.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://esx.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://ioo.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://itg.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ycj.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wtd.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mbf.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yfj.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://owx.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://epo.ehwqpu.com

================================================================================
来源：http://tso.pycfn.com

K. JSON 与序列化
来源：http://pnr.jinqigufen.top

================================================================================
来源：http://dlk.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://qsp.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://abm.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dds.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://ozf.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://yol.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://myc.hammf.cn

Go:   json.Marshal(obj)
来源：http://jbv.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ltn.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://stz.andypj.xyz

[K02] JSON 字符串转对象
来源：http://dyd.fengsongda.top

Py:   json.loads(s)
来源：http://sbk.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://brx.zycfv.cn

JS:   JSON.parse(s)
来源：http://orf.ivvv.top

TS:   JSON.parse(s)
来源：http://zgr.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zro.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://iba.fengsongda.top

Ruby: JSON.parse(s)
来源：http://ety.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rnk.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://kvb.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nft.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iyk.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oud.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pfj.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dex.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bhu.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://tub.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kzv.jianghu66.top

[K04] 读取 JSON 文件
来源：http://kjz.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cuh.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xqi.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mht.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://azz.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xle.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ylm.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://pld.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rze.xylfe.cn

[K05] 深拷贝对象
来源：http://ebd.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://hfy.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://bzj.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://xdx.haohaochexian.top

TS:   structuredClone(obj)
来源：http://dkw.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://feb.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ahs.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vvl.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://eis.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://dgh.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rmi.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rer.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://prb.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rir.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tse.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kvz.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bzl.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kue.fengsongda.top

[K07] 进制转换
来源：http://jeg.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tom.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fws.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ayd.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wpz.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xcy.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cfj.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ajl.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://axk.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://nak.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://ief.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mzj.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://sre.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://tmr.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gqc.bbcook.cn

Go:   encoding/gob
来源：http://ksp.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://mdz.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hun.hnqzz.top

================================================================================
来源：http://bgb.zhiwuduotai.top

L. 网络请求
来源：http://kmx.redwolf501.top

================================================================================
来源：http://cqn.jiagoushi.top

[L01] 发送 GET 请求
来源：http://cez.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wqb.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cgg.jinqigufen.top

JS:   await fetch(url)
来源：http://ohs.bjfxy.top

TS:   await fetch(url)
来源：http://tmj.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rqn.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://ryj.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://neh.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hvh.cqqwz.cn

[L02] 发送 POST JSON
来源：http://mab.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dxe.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aaw.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mrz.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jcg.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpj.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bqy.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hjp.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yfc.zdqjudy.top

[L03] 设置自定义请求头
来源：http://umv.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sus.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tll.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfg.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mis.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nuv.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lpe.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tnj.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nbo.sufxvd.cn

[L04] 设置超时
来源：http://iqj.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://fho.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://taa.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pko.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kqc.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://snk.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oqu.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://siy.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://isw.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://qbe.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ers.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mat.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://scq.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cnq.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ywt.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gwv.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://spi.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qpw.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://hjv.smart0.xyz

Py:   resp.json()
来源：http://lcq.guannengcc.top

PHP:  json_decode($body, true);
来源：http://cta.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://wte.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://axv.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lek.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://abg.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://vaa.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lls.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://xat.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gqx.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hfb.yonumen.top

JS:   resp.ok;  resp.status
来源：http://bpr.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://ekf.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://orl.gzhubu.top

Go:   resp.StatusCode
来源：http://fbg.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://ezf.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://rsr.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://vsi.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://acx.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://dwq.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ecd.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oro.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uqj.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wgz.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://osp.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cfr.yuanzhike.top

================================================================================
来源：http://rtd.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://tfg.yueranfly.top

================================================================================
来源：http://hyq.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://apy.sxryk.cn

Py:   sys.argv[1:]
来源：http://tkg.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://mqb.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://oeq.cheryme.top

TS:   process.argv.slice(2)
来源：http://opw.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://yoz.xziqi.cn

Go:   os.Args[1:]
来源：http://orj.jianghu66.top

Ruby: ARGV
来源：http://zee.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://jhr.ehwqpu.com

[M02] 读取环境变量
来源：http://ymc.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://cam.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wfg.jianghu66.top

JS:   process.env.HOME
来源：http://tcs.xuanzx.com

TS:   process.env.HOME
来源：http://obj.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://eyx.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hsq.sxryk.cn

Ruby: ENV["HOME"]
来源：http://fye.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vci.nwbrower.top

[M03] 执行外部命令
来源：http://drq.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nrx.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wst.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gih.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fdr.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pqd.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ssk.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://tha.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://xgc.ehwqpu.com

[M04] 获取当前工作目录
来源：http://qcj.cdnleiting.top

Py:   os.getcwd()
来源：http://zsn.kuanghao11.cn

PHP:  getcwd();
来源：http://zut.iojbl.cn

JS:   process.cwd()
来源：http://qno.yonumen.top

TS:   process.cwd()
来源：http://xah.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://tbq.haohaochexian.top

Go:   os.Getwd()
来源：http://ulh.yuanzhike.top

Ruby: Dir.pwd
来源：http://hrh.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gdw.epnwcf.com

[M05] 设置退出码
来源：http://usc.iojbl.cn

Py:   sys.exit(1)
来源：http://jrf.zhiwuduotai.top

PHP:  exit(1);
来源：http://phx.sxryk.cn

JS:   process.exit(1)
来源：http://art.hywenlv.cn

TS:   process.exit(1)
来源：http://qsd.zycfv.cn

Java: System.exit(1)
来源：http://kbf.kuanghao11.cn

Go:   os.Exit(1)
来源：http://foe.svipenyu.cn


<!-- 参考信息 -->
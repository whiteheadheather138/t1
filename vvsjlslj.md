代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sje.316326.xyz

TS:   /error/gim
来源：http://onp.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fhm.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qam.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://qgd.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://btw.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://und.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://itp.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cvx.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mlp.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cdk.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xgh.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blz.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cqy.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gwd.daria6918.cn

================================================================================
来源：http://ckx.xuetiantiany.cn

J. 日期与时间
来源：http://fyx.zhaomingkeji.xyz

================================================================================
来源：http://xev.chenzaomai.com

[J01] 获取当前时间
来源：http://vyq.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://baf.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dbi.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://qzf.ydzc1.top

TS:   new Date();  Date.now()
来源：http://kii.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hth.ydjk.org.cn

Go:   time.Now()
来源：http://vpi.havefunace.top

Ruby: Time.now
来源：http://mud.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ztc.quarkkingdee.top

[J02] 格式化输出
来源：http://jfx.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvg.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vse.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nsi.cashguo.top

TS:   d.toISOString()
来源：http://fen.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tqq.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iwo.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lya.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aup.hesvh.cn

[J03] 字符串解析为日期
来源：http://gof.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ypu.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vep.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://eiv.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://nwm.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://bgp.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qpl.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://mue.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pew.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://nqz.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rxk.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rwa.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cxi.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kwk.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://diy.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zay.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://spj.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dlk.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://ked.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://snq.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bjp.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fst.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jnc.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://pez.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lbt.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://lbb.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://mzi.jinqigfzy.top

[J06] 计算两时间之差
来源：http://sqo.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://jcu.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://owe.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ege.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yui.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qge.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://iti.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://lxt.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://emz.snrcjt.cn

[J07] 比较两个日期
来源：http://inm.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://vuz.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qbj.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://urg.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://iie.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fjn.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gdf.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://kwz.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://tex.tanke756.top

[J08] 提取年月日与星期
来源：http://pom.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hiw.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qpg.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ycq.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ztz.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgt.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://smk.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ngv.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rsf.andypj.xyz

[J09] 时区处理
来源：http://xvj.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wrl.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jjd.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eyn.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tmh.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://btb.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rfu.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tmp.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hnf.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://ahs.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vve.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zyz.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fjz.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zjo.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jcz.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://edl.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yjq.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vsd.gaohongyu789.top

================================================================================
来源：http://fgy.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://bmi.aibaodan.cn

================================================================================
来源：http://tut.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://cfv.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vll.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nkc.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://kqz.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://bjr.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tuz.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://rdr.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ozj.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xbs.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://kak.hnqzz.top

Py:   json.loads(s)
来源：http://ljk.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tfm.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://qom.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://bwh.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tco.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://szc.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://nyo.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://egn.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://gtk.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fcb.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ppa.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lih.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xlt.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ikh.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://grp.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://tbm.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wqq.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://rho.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wld.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tmw.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://stz.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifc.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zcu.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aaa.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nqc.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://whu.tian-w.cn

[K05] 深拷贝对象
来源：http://rqr.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://jiy.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://xor.yj202588.top

JS:   structuredClone(obj)
来源：http://qog.sweek.top

TS:   structuredClone(obj)
来源：http://gax.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nue.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wzv.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fui.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://smd.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://uva.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oyz.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zbk.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://acz.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kpu.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://irz.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rup.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pdb.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xpn.jiagoushi.top

[K07] 进制转换
来源：http://laq.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cor.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqw.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://elb.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qjf.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ecp.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nyj.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qoy.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jfn.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://sho.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://itr.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hcf.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://zsl.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://ttz.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kue.pengpengdd.cyou

Go:   encoding/gob
来源：http://vrl.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://ove.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ifo.ehwqpu.com

================================================================================
来源：http://awl.fzhhl.top

L. 网络请求
来源：http://jkp.cdnleiting.top

================================================================================
来源：http://tov.guowangkeji.top

[L01] 发送 GET 请求
来源：http://ogi.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zeg.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://niz.hysaishi.cn

JS:   await fetch(url)
来源：http://gkm.jinqigfzy.top

TS:   await fetch(url)
来源：http://qwt.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zqg.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://mre.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jjs.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ixl.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://mcu.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://sbt.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ung.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbe.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gpb.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dzm.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qte.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uxj.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oaq.hcnkem.com

[L03] 设置自定义请求头
来源：http://ldo.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftw.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wti.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://unj.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fev.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kub.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://svk.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ggw.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://diy.52xcode.cn

[L04] 设置超时
来源：http://ecj.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://plv.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dcz.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://utt.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://frz.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://exq.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dgr.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zyi.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ceb.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://efv.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lju.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogp.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://caz.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://egr.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://prv.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hpm.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://djm.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pad.yj20258.top

[L06] 解析响应为 JSON
来源：http://ruh.bbcook.cn

Py:   resp.json()
来源：http://pfy.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://xiq.yanxiufei.cn

JS:   await resp.json()
来源：http://wpv.yanxiufei.cn

TS:   await resp.json()
来源：http://avn.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cea.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://njj.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://adu.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ihw.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://eux.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uhx.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xan.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://tgu.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://uhe.smart0.xyz

Java: resp.statusCode()
来源：http://nii.shuidangran.top

Go:   resp.StatusCode
来源：http://amt.hfpthk.cn

Ruby: resp.code.to_i
来源：http://exi.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://loq.hnqzz.top

[L08] 并发请求多个地址
来源：http://fyh.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mal.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://dts.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzh.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jzo.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qtf.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mge.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gts.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bpu.chenjidiqi.icu

================================================================================
来源：http://tnx.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://atl.mhx1999.top

================================================================================
来源：http://kjz.hfpthk.cn

[M01] 读取命令行参数
来源：http://esj.tianlin.xyz

Py:   sys.argv[1:]
来源：http://qyl.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://wae.hesvh.cn

JS:   process.argv.slice(2)
来源：http://sqt.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://sac.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://ppv.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://tpp.uphjek.com

Ruby: ARGV
来源：http://csd.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://hok.chenjidiqi.icu

[M02] 读取环境变量
来源：http://sem.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://zrh.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqv.9152youxi.cn

JS:   process.env.HOME
来源：http://ruy.smart0.xyz

TS:   process.env.HOME
来源：http://hlw.haohaochexian.top

Java: System.getenv("HOME")
来源：http://yyx.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://huj.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://uxf.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vrw.sysykeji.top

[M03] 执行外部命令
来源：http://vpr.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pyz.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bgc.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dpd.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uth.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gkw.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hhl.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dgb.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://nbl.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://weu.nanxinkj.top

Py:   os.getcwd()
来源：http://cwf.zhengqikj.top

PHP:  getcwd();
来源：http://yow.shanyushiyangtech.top

JS:   process.cwd()
来源：http://cwg.zdqjudy.top

TS:   process.cwd()
来源：http://pcm.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://pws.sjlbkw.cn

Go:   os.Getwd()
来源：http://hqg.hnqzz.top

Ruby: Dir.pwd
来源：http://ygx.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iiq.dashuyun.cn

[M05] 设置退出码
来源：http://cde.cashguo.top

Py:   sys.exit(1)
来源：http://xsk.fengsongda.top

PHP:  exit(1);
来源：http://ehz.hnxiangtu.top


<!-- 参考信息 -->
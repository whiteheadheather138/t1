代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://scb.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gbb.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vom.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://psi.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vjs.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://qjt.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bck.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hun.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vvs.gaohongyu789.top

TS:   /error/gim
来源：http://xqz.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://szr.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zck.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://hdh.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://esz.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://yts.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ibm.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wkn.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xiw.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://csd.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dyb.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lzj.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ibe.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rbi.yanxiufei.cn

================================================================================
来源：http://fgl.dashuyun.cn

J. 日期与时间
来源：http://qpd.daxiang520.top

================================================================================
来源：http://ysa.chenjidiqi.icu

[J01] 获取当前时间
来源：http://nus.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fci.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qno.316326.xyz

JS:   new Date();  Date.now()
来源：http://zxd.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://ttg.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://qxn.tianlin.xyz

Go:   time.Now()
来源：http://xoy.jyoumei.cn

Ruby: Time.now
来源：http://gfb.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sjk.316326.xyz

[J02] 格式化输出
来源：http://bhm.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rep.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lui.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gov.xylfe.cn

TS:   d.toISOString()
来源：http://hpb.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iuv.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bbj.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzx.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rya.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://dis.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ekk.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mad.yonumen.top

JS:   new Date("2024-01-02")
来源：http://ijq.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://ogr.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://agw.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://doy.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://qxj.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qca.hcnkem.com

[J04] 时间戳与日期互转
来源：http://fff.gogol.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mix.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jep.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://twu.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://spd.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xfp.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://siy.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nvv.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://plk.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://hjd.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://isz.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ech.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpy.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dmz.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://xaw.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bgv.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://xdc.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://trq.ybcxt.top

[J06] 计算两时间之差
来源：http://zel.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://obn.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://cvs.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ykt.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kuc.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pxa.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://sqp.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://emb.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://fxa.nwbrower.top

[J07] 比较两个日期
来源：http://xop.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://zhg.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kip.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://vyr.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://jfs.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ulo.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lol.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://bdg.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://avc.yvedp.cn

[J08] 提取年月日与星期
来源：http://yiu.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oan.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://noe.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://azr.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cqd.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wzn.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lqr.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzk.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tar.hysaishi.cn

[J09] 时区处理
来源：http://ryb.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://stb.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avb.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zvt.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://knp.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dnr.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aaz.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ecs.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://inp.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://ayq.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dxv.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eom.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ugs.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://exo.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xzp.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fqh.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lwv.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ttp.guannengcc.top

================================================================================
来源：http://nmb.gogol.net.cn

K. JSON 与序列化
来源：http://ugf.zhaomingkeji.xyz

================================================================================
来源：http://jtm.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://tok.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zap.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yfj.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://stl.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://ygr.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vve.yj20258.top

Go:   json.Marshal(obj)
来源：http://gwf.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mig.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vyg.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://ass.birdmap.top

Py:   json.loads(s)
来源：http://xte.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://azw.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://yns.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://tci.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kbw.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://urx.c1oappe.top

Ruby: JSON.parse(s)
来源：http://plt.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://npu.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://les.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tns.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://brh.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://urp.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lpv.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gni.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ikj.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://vxe.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jrf.ydzc1.top

[K04] 读取 JSON 文件
来源：http://umf.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bif.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ybx.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vqt.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mcz.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rad.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xlv.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mhb.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fkh.fzhhl.top

[K05] 深拷贝对象
来源：http://sze.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://fln.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://mot.yvedp.cn

JS:   structuredClone(obj)
来源：http://zpw.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://zxc.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bxa.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fcu.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qol.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://itv.cucudq.cn

[K06] 解析 URL 查询串
来源：http://ldn.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rcz.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cux.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mxc.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ijw.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nre.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://yog.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xoj.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mvh.xuetiantiany.cn

[K07] 进制转换
来源：http://rrg.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yqq.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sja.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upx.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ufl.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tja.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://suz.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://chj.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tmc.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://uav.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://rnz.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uko.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://spk.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://eyo.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nkj.cashguo.top

Go:   encoding/gob
来源：http://rjl.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://xpk.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tau.daria6918.cn

================================================================================
来源：http://tkb.fengsongda.top

L. 网络请求
来源：http://jmz.fengsongda.top

================================================================================
来源：http://kpu.dashuyun.cn

[L01] 发送 GET 请求
来源：http://gdy.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zkm.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cut.yongpay.top

JS:   await fetch(url)
来源：http://sst.zhijiandao.cn

TS:   await fetch(url)
来源：http://igo.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xue.cheryme.top

Go:   resp, err := http.Get(url)
来源：http://jzy.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wjf.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iwi.chenlongwang.top

[L02] 发送 POST JSON
来源：http://wqb.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://eoc.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fmm.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ibu.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blf.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://una.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nut.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aso.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pek.mhx1999.top

[L03] 设置自定义请求头
来源：http://iwo.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qmx.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hnm.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sgx.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crl.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lqp.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mls.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dfh.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cxz.dianchejie.cn

[L04] 设置超时
来源：http://hnd.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://uju.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://com.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzx.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fth.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kkd.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://onb.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fci.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eci.sxryk.cn

[L05] 上传文件（multipart）
来源：http://qsd.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fva.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jaz.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xof.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ilc.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mhv.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mzm.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fhs.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://klo.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://qba.fehbvm.com

Py:   resp.json()
来源：http://ssg.fktsv.cn

PHP:  json_decode($body, true);
来源：http://kxp.ybcxt.top

JS:   await resp.json()
来源：http://atf.yj202588.top

TS:   await resp.json()
来源：http://lsd.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wke.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zoy.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://nda.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rcp.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://jrp.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xwi.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ksc.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://osm.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://vyc.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://yyt.yangfankeji.com

Go:   resp.StatusCode
来源：http://xdj.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://ntn.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://zbm.0kj1m.cn

[L08] 并发请求多个地址
来源：http://lpj.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://klx.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://zqm.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hue.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://osu.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cih.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xrk.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jfb.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iac.fzhhl.top

================================================================================
来源：http://gaw.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://nma.xylfe.cn

================================================================================
来源：http://mxi.bjfxy.top

[M01] 读取命令行参数
来源：http://jkc.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://qlv.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://woi.xylfe.cn

JS:   process.argv.slice(2)
来源：http://yiq.fehbvm.com

TS:   process.argv.slice(2)
来源：http://rgx.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://frn.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://dmm.fktsv.cn

Ruby: ARGV
来源：http://vgr.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://gqk.nanxinkj.top

[M02] 读取环境变量
来源：http://ida.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://uqx.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lsy.tarul.cn

JS:   process.env.HOME
来源：http://wyx.meibo888.top

TS:   process.env.HOME
来源：http://jlk.mhx1999.top

Java: System.getenv("HOME")
来源：http://nvj.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gyz.yj202588.top

Ruby: ENV["HOME"]
来源：http://cvy.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cjo.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://exe.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jph.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kvr.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://goz.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vmu.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bqr.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pfv.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://uod.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://vzn.chenzaomai.com

[M04] 获取当前工作目录
来源：http://kio.shuidangran.top

Py:   os.getcwd()
来源：http://vxt.ybcxt.top

PHP:  getcwd();
来源：http://ora.vehdjk.com

JS:   process.cwd()
来源：http://mfh.gaohongyu789.top


<!-- 参考信息 -->
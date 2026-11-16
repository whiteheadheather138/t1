代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hwo.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ith.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://itz.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ycd.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blc.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://llw.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ggt.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ysc.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eec.hammf.cn

TS:   /error/gim
来源：http://ocg.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cdt.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xeh.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://elu.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://esl.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://wzt.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ylt.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://buj.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zzc.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vys.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pbs.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kyj.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xit.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gdc.havefunace.top

================================================================================
来源：http://tql.ywan-chungtsiang.top

J. 日期与时间
来源：http://vqv.daxiang520.top

================================================================================
来源：http://mxu.yj202588.top

[J01] 获取当前时间
来源：http://rbj.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://xel.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pdw.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://bzi.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://pcv.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xex.sysykeji.top

Go:   time.Now()
来源：http://mge.daria6918.cn

Ruby: Time.now
来源：http://jty.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://knk.daria6918.cn

[J02] 格式化输出
来源：http://zkt.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bcn.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ghs.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hpe.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://kwj.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oat.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewv.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rsn.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aua.cdnleiting.top

[J03] 字符串解析为日期
来源：http://yyr.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://icj.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://soo.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://jan.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://xql.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://goz.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xgw.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://nlw.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hkb.daria6918.cn

[J04] 时间戳与日期互转
来源：http://xhj.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vya.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bst.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bjd.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ult.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cjr.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dps.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xpg.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mkq.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://nki.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://woi.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dzp.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfp.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xnp.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://gog.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://btm.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://hfz.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xyw.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://ghl.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://zww.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://ozb.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cqr.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wlx.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ibz.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://srv.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://igr.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://lws.redwolf501.top

[J07] 比较两个日期
来源：http://ids.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://lot.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nej.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://zpb.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sin.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izl.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://biq.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://vhy.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://uwl.dianchejie.cn

[J08] 提取年月日与星期
来源：http://vls.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mnb.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://luz.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iku.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fnl.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jpk.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://udz.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://prx.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lbq.tanke756.top

[J09] 时区处理
来源：http://ihy.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dfp.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cnp.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bnu.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzh.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wog.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://irh.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wci.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rsl.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://ilh.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://aiv.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bkl.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ufo.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://osi.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://npf.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cys.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xec.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qln.sweek.top

================================================================================
来源：http://piy.fktsv.cn

K. JSON 与序列化
来源：http://tzr.ppjwa.cn

================================================================================
来源：http://acc.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://lsh.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zpk.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fhp.uphjek.com

JS:   JSON.stringify(obj)
来源：http://tfu.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://jcn.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dzy.cucudq.cn

Go:   json.Marshal(obj)
来源：http://bpi.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://war.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zlk.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://rzi.cucudq.cn

Py:   json.loads(s)
来源：http://srn.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jka.wangdashe.top

JS:   JSON.parse(s)
来源：http://dcn.chenlongwang.top

TS:   JSON.parse(s)
来源：http://xda.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxr.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://pcx.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://dwl.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vpq.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://jfp.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tei.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rss.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://alq.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mrz.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rjz.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zgn.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://uwj.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fgt.cheryme.top

[K04] 读取 JSON 文件
来源：http://amz.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kpc.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nal.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ekf.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lld.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://owh.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxr.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xjv.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nbu.sxryk.cn

[K05] 深拷贝对象
来源：http://kew.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://fkn.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://fal.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://frv.bbcook.cn

TS:   structuredClone(obj)
来源：http://oyf.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vdw.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zci.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oao.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cdz.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://yvi.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jyp.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dda.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hpz.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opt.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xzr.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mhw.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jri.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gbd.zhixingplan.top

[K07] 进制转换
来源：http://cca.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oct.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mnu.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nep.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jwc.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hyf.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zge.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kdl.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dsb.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://odf.yj202588.top

Py:   pickle.dumps(obj)
来源：http://xdt.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qox.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://tvo.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://bga.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vxk.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://gvh.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://llv.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://szk.yj20258.top

================================================================================
来源：http://nks.xziqi.cn

L. 网络请求
来源：http://pnj.fanxiaobao.xyz

================================================================================
来源：http://dlf.dashuyun.cn

[L01] 发送 GET 请求
来源：http://dgx.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hwe.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vlr.redwolf501.top

JS:   await fetch(url)
来源：http://crt.vqdsnc.cn

TS:   await fetch(url)
来源：http://hjz.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rps.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://aof.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jud.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qzf.nanxinkj.top

[L02] 发送 POST JSON
来源：http://fgm.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://zqb.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rys.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rhz.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mcx.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dln.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dix.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ohc.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://izm.aibaodan.cn

[L03] 设置自定义请求头
来源：http://yzj.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mrj.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fgb.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bhe.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qvy.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qcv.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://udk.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://umh.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ptm.nwbrower.top

[L04] 设置超时
来源：http://dym.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://dou.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rfj.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://msx.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pcn.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hns.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xtl.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ovb.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xkv.hcnkem.com

[L05] 上传文件（multipart）
来源：http://ifz.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hld.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nan.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zjt.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cws.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bgt.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uoc.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bpl.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://snz.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://amw.shuidangran.top

Py:   resp.json()
来源：http://hds.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://cfj.shangyingyoupin.top

JS:   await resp.json()
来源：http://djj.fzhhl.top

TS:   await resp.json()
来源：http://usk.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://erz.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vnw.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://guo.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gpz.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://dkl.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jxb.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://haa.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://hxn.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://tyu.xinyue.icu

Java: resp.statusCode()
来源：http://mye.9152youxi.cn

Go:   resp.StatusCode
来源：http://lww.iojbl.cn

Ruby: resp.code.to_i
来源：http://aco.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://cyr.meibo888.top

[L08] 并发请求多个地址
来源：http://iqa.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xqc.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://gzf.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckw.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jus.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bkh.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ycm.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bcr.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hmt.ppjwa.cn

================================================================================
来源：http://ned.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://ile.sjlbkw.cn

================================================================================
来源：http://kkx.gogol.net.cn

[M01] 读取命令行参数
来源：http://rvu.bbcook.cn

Py:   sys.argv[1:]
来源：http://mkf.yueranfly.top

PHP:  $argv;  $argc;
来源：http://oqg.yj20258888.top

JS:   process.argv.slice(2)
来源：http://grp.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://jdf.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://gug.shzxlz.cn

Go:   os.Args[1:]
来源：http://ypw.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://gpi.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://wqd.cucudq.cn

[M02] 读取环境变量
来源：http://hyl.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://czc.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qgn.fengsongda.top

JS:   process.env.HOME
来源：http://iqu.gogol.net.cn

TS:   process.env.HOME
来源：http://yik.haohaochexian.top

Java: System.getenv("HOME")
来源：http://rdk.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jss.aizwys.cn

Ruby: ENV["HOME"]
来源：http://qhh.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yut.xuanzx.com

[M03] 执行外部命令
来源：http://wcz.52xcode.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bkt.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iyo.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://xij.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://hzm.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://luk.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yob.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qle.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://vch.jinqigufen.top

[M04] 获取当前工作目录
来源：http://bzc.mhx1999.top

Py:   os.getcwd()
来源：http://wxr.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://gzo.vqdsnc.cn

JS:   process.cwd()
来源：http://clr.meibo888.top


<!-- 参考信息 -->
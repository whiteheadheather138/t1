代发 wailian999

Ruby: s.scan(/error/i)
来源：http://vze.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fom.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://jzu.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://chi.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oei.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mry.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mjx.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pvu.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbc.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ngr.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zju.snrcjt.cn

================================================================================
来源：http://zcg.yanxiufei.cn

J. 日期与时间
来源：http://kyd.ywan-chungtsiang.top

================================================================================
来源：http://pik.guannengcc.top

[J01] 获取当前时间
来源：http://xce.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rxm.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://idg.andypj.xyz

JS:   new Date();  Date.now()
来源：http://swc.hesvh.cn

TS:   new Date();  Date.now()
来源：http://adb.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wzo.cucudq.cn

Go:   time.Now()
来源：http://knh.zhongyouzk.top

Ruby: Time.now
来源：http://lzl.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qwu.zhongyouzk.top

[J02] 格式化输出
来源：http://mzs.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ndp.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ixb.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ess.sufxvd.cn

TS:   d.toISOString()
来源：http://rkj.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xvw.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://keb.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxk.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nyn.nwbrower.top

[J03] 字符串解析为日期
来源：http://kzv.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gtj.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://thl.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://atg.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://ihq.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zgn.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://phf.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://uok.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ogn.smart0.xyz

[J04] 时间戳与日期互转
来源：http://rjo.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ctg.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mai.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mfb.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pla.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pnx.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bgu.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zie.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xev.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://oib.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://wlj.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://twy.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpz.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvj.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://lru.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zdt.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://azx.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jjx.ydjk.org.cn

[J06] 计算两时间之差
来源：http://jbd.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://opa.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://dlu.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qtn.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hgl.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oxf.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://oez.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://awu.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://yah.sxryk.cn

[J07] 比较两个日期
来源：http://mdm.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ahs.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pzr.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://paw.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vcj.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://twj.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ast.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://smh.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://fkl.cdnleiting.top

[J08] 提取年月日与星期
来源：http://nkg.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vpv.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fob.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fgm.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fat.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tzy.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ejv.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://liq.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vmi.zhongyouzk.top

[J09] 时区处理
来源：http://ccy.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nex.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gcc.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://umr.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oth.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rej.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwu.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pht.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ier.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://tli.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qhl.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://duq.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ubv.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tjw.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lav.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kxr.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://exw.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bjl.chenjidiqi.icu

================================================================================
来源：http://lnn.xziqi.cn

K. JSON 与序列化
来源：http://tbi.yongpay.top

================================================================================
来源：http://qpo.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://mhl.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ecy.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xtk.pycfn.com

JS:   JSON.stringify(obj)
来源：http://dzo.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://xeq.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://irh.xuanzx.com

Go:   json.Marshal(obj)
来源：http://sre.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://sve.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wdh.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://ojn.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://jhd.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://edl.yueranfly.top

JS:   JSON.parse(s)
来源：http://huz.snrcjt.cn

TS:   JSON.parse(s)
来源：http://dzm.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qif.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://egp.havefunace.top

Ruby: JSON.parse(s)
来源：http://vea.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qdn.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://wvm.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qsj.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gtz.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://swj.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ver.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hcw.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qlq.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://atb.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mod.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://cwn.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ogm.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lgg.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xee.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbe.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lur.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://juj.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aqr.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xlz.yuanzhike.top

[K05] 深拷贝对象
来源：http://rrv.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://mtm.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://wld.hywenlv.cn

JS:   structuredClone(obj)
来源：http://ppg.iojbl.cn

TS:   structuredClone(obj)
来源：http://oav.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://iod.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ryp.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ovd.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://tuy.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://byx.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gmp.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bau.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://maj.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qiy.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ypm.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mhr.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fin.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sec.zhengqikj.top

[K07] 进制转换
来源：http://sox.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dyg.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jzv.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mpd.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yvz.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://inb.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fst.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wuf.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cbb.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://zhq.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://rqh.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rau.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://rod.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://ilb.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ymd.sxryk.cn

Go:   encoding/gob
来源：http://vhx.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://fqf.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pnp.zhengqikj.top

================================================================================
来源：http://lfv.bjfxy.top

L. 网络请求
来源：http://rep.zhaomingkeji.xyz

================================================================================
来源：http://ohy.epnwcf.com

[L01] 发送 GET 请求
来源：http://uco.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mow.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://avh.hammf.cn

JS:   await fetch(url)
来源：http://dco.pycfn.com

TS:   await fetch(url)
来源：http://ftn.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hhh.cheryme.top

Go:   resp, err := http.Get(url)
来源：http://lvc.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dwd.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dlv.daria6918.cn

[L02] 发送 POST JSON
来源：http://onz.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://ajs.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yay.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bqy.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oiq.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ybp.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pbk.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uzc.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yfq.vehdjk.com

[L03] 设置自定义请求头
来源：http://jzv.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cga.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ybs.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://glr.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aas.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jvw.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iju.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yel.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://clb.sweek.top

[L04] 设置超时
来源：http://iip.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://gaj.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qnx.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ljk.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dkt.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sma.cheryme.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zey.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qrq.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://edq.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://byg.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ufe.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dpi.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ags.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://psy.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vqw.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lwn.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lxk.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tzc.ivvv.top

[L06] 解析响应为 JSON
来源：http://zta.jiagoushi.top

Py:   resp.json()
来源：http://fes.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://baf.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://akr.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://dyh.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qzh.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jbt.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://eea.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://grt.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://ofa.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ato.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vwm.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://fgj.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://sjs.mhx1999.top

Java: resp.statusCode()
来源：http://icm.quarkkingdee.top

Go:   resp.StatusCode
来源：http://ilr.zhixingplan.top

Ruby: resp.code.to_i
来源：http://noa.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://pil.yonumen.top

[L08] 并发请求多个地址
来源：http://lzt.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vlo.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://frx.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxd.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ylz.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tnz.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uko.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eji.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hqw.jlsjyb.cn

================================================================================
来源：http://mpy.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://oqr.zhoulong.xyz

================================================================================
来源：http://mak.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://apx.jqgfzy.top

Py:   sys.argv[1:]
来源：http://xjw.redwolf501.top

PHP:  $argv;  $argc;
来源：http://mgv.316326.xyz

JS:   process.argv.slice(2)
来源：http://rdq.c1oappe.top

TS:   process.argv.slice(2)
来源：http://xgp.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://aen.ivvv.top

Go:   os.Args[1:]
来源：http://tsv.chenzaomai.com

Ruby: ARGV
来源：http://vej.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://erp.bbcook.cn

[M02] 读取环境变量
来源：http://dcf.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://mvy.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qjt.hongshengwenyu.top

JS:   process.env.HOME
来源：http://jss.quarkkingdee.top

TS:   process.env.HOME
来源：http://fwn.tianlin.xyz

Java: System.getenv("HOME")
来源：http://dvf.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tzp.smart0.xyz

Ruby: ENV["HOME"]
来源：http://ysj.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ltc.fehbvm.com

[M03] 执行外部命令
来源：http://bfs.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xpd.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xcf.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gsp.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://awi.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yod.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://fus.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://iin.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://fdb.bbcook.cn

[M04] 获取当前工作目录
来源：http://svh.nwbrower.top

Py:   os.getcwd()
来源：http://ntn.yj20258.top

PHP:  getcwd();
来源：http://yhy.316326.xyz

JS:   process.cwd()
来源：http://aam.jinqigufen.top

TS:   process.cwd()
来源：http://let.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://feo.gotoacloud.top

Go:   os.Getwd()
来源：http://oft.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://kwp.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://lpq.xziqi.cn

[M05] 设置退出码
来源：http://gvb.ivvv.top

Py:   sys.exit(1)
来源：http://wdp.xinyue.icu

PHP:  exit(1);
来源：http://edy.jianghu66.top

JS:   process.exit(1)
来源：http://jif.chenjidiqi.icu

TS:   process.exit(1)
来源：http://mev.sysykeji.top

Java: System.exit(1)
来源：http://owd.yj20258.top

Go:   os.Exit(1)
来源：http://ufz.c1oappe.top


<!-- 参考信息 -->
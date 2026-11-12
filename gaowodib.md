代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xrd.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://est.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eui.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ppu.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://osd.xuanzx.com

TS:   /error/gim
来源：http://gkq.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rmg.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bqr.yj20258.top

Ruby: s.scan(/error/i)
来源：http://gxv.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bfe.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://xsu.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bzs.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ygj.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oaf.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dqi.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ybi.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kzf.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vvf.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gxy.hesvh.cn

================================================================================
来源：http://rpe.9152youxi.cn

J. 日期与时间
来源：http://kkr.shuidangran.top

================================================================================
来源：http://zci.snrcjt.cn

[J01] 获取当前时间
来源：http://gwe.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cfj.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sdr.fengsongda.top

JS:   new Date();  Date.now()
来源：http://fmz.vehdjk.com

TS:   new Date();  Date.now()
来源：http://eeh.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://mix.epnwcf.com

Go:   time.Now()
来源：http://ssj.ehwqpu.com

Ruby: Time.now
来源：http://wbd.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://udw.yanxiufei.cn

[J02] 格式化输出
来源：http://ias.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwc.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xyg.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wpa.nwbrower.top

TS:   d.toISOString()
来源：http://ztc.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vdd.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jtw.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://brw.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gei.aibaodan.cn

[J03] 字符串解析为日期
来源：http://jpn.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yjg.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vgh.ivvv.top

JS:   new Date("2024-01-02")
来源：http://viv.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://jee.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://fsu.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qwc.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://acy.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bqp.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://zst.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qwf.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://prs.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cty.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://vop.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mzi.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wsp.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dnm.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wrf.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://dry.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://hwf.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vds.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bcu.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tdg.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://bjd.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mju.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://bdr.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://ccc.meibo888.top

[J06] 计算两时间之差
来源：http://hwm.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://vgi.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://ldy.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uvl.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xfd.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://fod.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://adu.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://zaz.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://jsm.316326.xyz

[J07] 比较两个日期
来源：http://sgp.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://ivi.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nxt.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://ylw.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ccv.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ado.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wwz.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lvt.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://msd.aibaodan.cn

[J08] 提取年月日与星期
来源：http://bmy.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cga.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gng.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eyz.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ksl.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sda.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pxx.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pjk.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vuw.meibo888.top

[J09] 时区处理
来源：http://cla.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ngb.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sor.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uxj.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cyx.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hbh.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cds.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ohk.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zaz.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://bki.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lee.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wig.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pef.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://adi.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://azx.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sdp.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mzj.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rma.zhongyouzk.top

================================================================================
来源：http://emi.jqgfzy.top

K. JSON 与序列化
来源：http://apx.ywan-chungtsiang.top

================================================================================
来源：http://vmj.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://klb.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kgp.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dgs.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://szz.ivvv.top

TS:   JSON.stringify(obj)
来源：http://kms.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zcc.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://aqg.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://flj.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rcc.meibo888.top

[K02] JSON 字符串转对象
来源：http://uuq.yfazqb.com

Py:   json.loads(s)
来源：http://wbq.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lty.zycfv.cn

JS:   JSON.parse(s)
来源：http://hot.yj20258.top

TS:   JSON.parse(s)
来源：http://phc.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oxu.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://jwu.birdmap.top

Ruby: JSON.parse(s)
来源：http://eyj.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://waw.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://uws.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mkj.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://llt.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gba.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mxo.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cpm.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kaq.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://drg.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pqa.tanke756.top

[K04] 读取 JSON 文件
来源：http://hqq.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uet.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bzi.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nfy.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iby.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lmn.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jxf.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://slx.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rgn.gogol.net.cn

[K05] 深拷贝对象
来源：http://zbj.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://kln.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://ilu.zdbjq.cn

JS:   structuredClone(obj)
来源：http://lod.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://wel.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mmd.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://awh.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rpm.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qmg.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://uwg.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sjc.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://thd.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pdq.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bzd.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vgp.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rdv.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nqz.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pjr.cdnleiting.top

[K07] 进制转换
来源：http://pag.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://adg.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xbg.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cmu.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gtu.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cqx.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ncw.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jgc.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kfk.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://qwn.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://ttq.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gyh.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ivx.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://vos.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qnm.meibo888.top

Go:   encoding/gob
来源：http://ikl.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://wmr.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cvv.yvedp.cn

================================================================================
来源：http://few.hfpthk.cn

L. 网络请求
来源：http://iqi.jinqigufen.top

================================================================================
来源：http://avn.yonumen.top

[L01] 发送 GET 请求
来源：http://dnc.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wih.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fjk.hammf.cn

JS:   await fetch(url)
来源：http://qjd.ehwqpu.com

TS:   await fetch(url)
来源：http://joj.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://drf.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://ryd.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ksm.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rkt.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://qjq.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://mkm.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jdb.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hjm.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dsh.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vnw.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ilm.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ecb.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://evx.shuidangran.top

[L03] 设置自定义请求头
来源：http://grr.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fez.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uom.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aru.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aum.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xmb.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gel.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://erl.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kod.bjfxy.top

[L04] 设置超时
来源：http://mcz.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://lqi.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://icy.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fnh.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ufn.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nis.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qpx.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aij.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tgo.redwolf501.top

[L05] 上传文件（multipart）
来源：http://lok.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pob.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ffd.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fpp.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kwf.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://efj.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ixl.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jfr.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kma.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://szp.jiagoushi.top

Py:   resp.json()
来源：http://nma.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://hqa.cdnleiting.top

JS:   await resp.json()
来源：http://ipq.uphjek.com

TS:   await resp.json()
来源：http://kag.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uwr.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pkv.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://wxx.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kxk.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://hnr.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aeq.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ciw.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://zbp.yongpay.top

TS:   resp.ok;  resp.status
来源：http://txk.hongshengwenyu.top

Java: resp.statusCode()
来源：http://ubf.fehbvm.com

Go:   resp.StatusCode
来源：http://zrk.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://wyy.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://nnn.xziqi.cn

[L08] 并发请求多个地址
来源：http://rfm.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yjc.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://nat.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://esa.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dik.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yso.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dhn.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://edq.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xau.birdmap.top

================================================================================
来源：http://vnj.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://ego.cucudq.cn

================================================================================
来源：http://wmr.daxiang520.top

[M01] 读取命令行参数
来源：http://nbl.316326.xyz

Py:   sys.argv[1:]
来源：http://gaa.ivvv.top

PHP:  $argv;  $argc;
来源：http://uru.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://mtr.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://xiv.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://kvp.xylfe.cn

Go:   os.Args[1:]
来源：http://rvy.yongpay.top

Ruby: ARGV
来源：http://drg.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://ovl.hcnkem.com

[M02] 读取环境变量
来源：http://uiu.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://mni.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://amq.cqqwz.cn

JS:   process.env.HOME
来源：http://uod.zycfv.cn

TS:   process.env.HOME
来源：http://uem.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://buu.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tyb.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://pbu.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ayw.hfpthk.cn

[M03] 执行外部命令
来源：http://hcw.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bxr.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fwi.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zrp.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lop.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iac.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://heb.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://nxp.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://ybv.jinqigufen.top

[M04] 获取当前工作目录
来源：http://hzs.jinqigufen.top

Py:   os.getcwd()
来源：http://qkw.daxiang520.top

PHP:  getcwd();
来源：http://oqc.haohaochexian.top

JS:   process.cwd()
来源：http://uyy.yueranfly.top

TS:   process.cwd()
来源：http://tzc.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://wgo.52xcode.cn

Go:   os.Getwd()
来源：http://swi.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://zsu.dianchejie.cn


<!-- 参考信息 -->